# 🤖 AI Knowledge Management Agent (DITA XML & EKM Auditor)

A full-stack, offline-first AI agent that automatically converts raw documentation drafts, support tickets, and email threads into **IXIASOFT DITA XML** topics conforming to strict corporate EKM Style Guidelines.

### 🛠️ Tech Stack
![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Gemini AI](https://img.shields.io/badge/Gemini%20AI-4285F4?style=for-the-badge&logo=google&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind%20CSS-38B2AC?style=for-the-badge&logo=tailwindcss&logoColor=white)
![JSON Database](https://img.shields.io/badge/JSON_Database-000000?style=for-the-badge&logo=json&logoColor=white)

---

### 🌟 Key Features
*   **📂 Multi-Format Ingestion**: Parses PDFs, Word Docs (.docx), and Plain Text (.txt) on-the-fly.
*   **🧠 Strict EKM Formatting**: Deterministic AI output (`temp: 0.0`) wraps UI terms in `<uicontrol>`, navigation paths in `<menucascade>`, and automatically strips time-sensitive dates or version notes.
*   **📊 SharePoint-to-KM Pipeline Dashboard**: Visualizes article progress through 4 workflow stages (SharePoint Queue ➔ Draft in Progress ➔ SME Review ➔ Published).
*   **🔍 EKM Compliance KPI Auditor**: Dynamically audits opened DITA XML documents, calculating a compliance score (0-100%) and detailing styling action items.
*   **💾 100% Offline-First Persistence**: Uses a local JSON-file storage backend—removing all external database dependencies and setups.

---

### 🔄 Project Pipeline Flow
```mermaid
graph LR
    A[SharePoint Request] ➔ B[AI Drafting] ➔ C[SME Review] ➔ D[Published to KM]
