import { useState } from 'react';
import DOMPurify from 'dompurify';
import ReactMarkdown from 'react-markdown';
import Asciidoctor from 'asciidoctor';
import { Card, CardContent, CardHeader, CardTitle } from '@/components/ui/card';
import { Button } from '@/components/ui/button';

export default function MarkupViewer() {
  const [input, setInput] = useState('');
  const [language, setLanguage] = useState('markdown');
  const asciidoctor = Asciidoctor();

  const renderContent = () => {
    if (language === 'markdown') {
      return <ReactMarkdown>{input}</ReactMarkdown>;
    } else if (language === 'asciidoc') {
      const html = asciidoctor.convert(input);
      return <div dangerouslySetInnerHTML={{ __html: DOMPurify.sanitize(html) }} />;
    } else if (language === 'html') {
      return <div dangerouslySetInnerHTML={{ __html: DOMPurify.sanitize(input) }} />;
    }
  };

  return (
    <div className="grid grid-cols-1 md:grid-cols-2 gap-4 p-6">
      <Card>
        <CardHeader>
          <CardTitle>Markup Editor</CardTitle>
        </CardHeader>
        <CardContent>
          <select
            className="border rounded p-2 mb-3 w-full"
            value={language}
            onChange={(e) => setLanguage(e.target.value)}
          >
            <option value="markdown">Markdown</option>
            <option value="asciidoc">AsciiDoc</option>
            <option value="html">HTML</option>
          </select>
          <textarea
            value={input}
            onChange={(e) => setInput(e.target.value)}
            className="w-full h-96 border rounded p-2 font-mono"
            placeholder="Type or paste your markup here..."
          />
          <Button
            className="mt-3"
            onClick={() => navigator.clipboard.writeText(input)}
          >
            Copy Source
          </Button>
        </CardContent>
      </Card>

      <Card>
        <CardHeader>
          <CardTitle>Preview</CardTitle>
        </CardHeader>
        <CardContent>
          <div className="prose max-w-none dark:prose-invert">
            {renderContent()}
          </div>
        </CardContent>
      </Card>
    </div>
  );
}
