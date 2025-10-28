# Project Flow
 
 Here is a description of the project workflow:
 
 1.  **GitHub Desktop - GIT Versioning (like Google Docs History):** Version control is managed using GitHub Desktop.
 2.  **Firebase Studio - Frontend HTML CSS Mastery (like Paint / W3Schools):** The frontend is developed using Firebase Studio, focusing on HTML and CSS.
 3.  **Markup Language - README and FlowCharts using Mermaid (like PowerPoint):** Documentation, including this README and flowcharts, is created using Markdown and Mermaid.
 4.  **Database Management - Supabase SQL Tables (like Excel):** Supabase is used for database management with SQL tables.
 5.  **AI Tools - Gemini / Jules / Windsurf / CODEX (like JavaScript Backend):** AI tools are leveraged for backend development and automation.
 6.  The process then cycles back to step 1, with continued development and versioning.
 
+## Tech Stack Flowchart
+
+```mermaid
+flowchart LR
+    GitHub["GitHub Desktop
GIT Versioning"] --> Firebase["Firebase Studio
Frontend HTML & CSS"]
+    Firebase --> Markup["Markup Language
Markdown & Mermaid"]
+    Markup --> Supabase["Supabase SQL Tables
Database Management"]
+    Supabase --> AI["AI Tools
Gemini / Jules / Windsurf / CODEX"]
+    AI --> GitHub
+```
+
 ## Legend
 
 *   **GitHub:** Version History like Google Docs
 *   **Firebase:** Frontend Design like Paint
 *   **Markup:** Documentation like PowerPoint
 *   **Supabase:** Database like Excel
 *   **AI Tools:** Backend Automation replacing IT staff
 
 # Web App Flowchart: Company Software Tracker
 
 | Step | Action | Description |
 |---|---|---|
 | 1 | **Access App** | The user opens the web application in their browser. |
 | 2 | **Enter Company Details** | The user is presented with a form to enter the company's name and address. |
 | 3 | **Enter Software Details** | The user enters the expiry dates for software licenses: 365, NordVPN, McAfee Antivirus, Adobe, and ChatGPT. |
 | 4 | **Save Data** | The user submits the form. The data is sent to the backend and stored in a Supabase database. |
 | 5 | **View Tracked Data** | The application displays a table of all tracked companies and their software license information. |
 
 # Dummy Data
 
 | Company Name | Address | 365 Expiry | NordVPN Expiry | McAfee Antivirus Expiry | Adobe Expiry | ChatGPT Expiry |
 |---|---|---|---|---|---|---|
 | Acme Inc. | 123 Main St, Anytown, USA | 2024-12-31 | 2025-06-15 | 2024-10-20 | 2025-01-31 | 2024-11-30 |
 | Globex Corp. | 456 Oak Ave, Sometown, USA | 2025-03-22 | 2024-09-01 | 2025-02-28 | 2024-08-14 | 2025-05-19 |
 | Stark Industries | 789 Pine Ln, Yourtown, USA | 2024-07-11 | 2025-04-05 | 2024-12-01 | 2025-03-10 | 2024-09-25 |
