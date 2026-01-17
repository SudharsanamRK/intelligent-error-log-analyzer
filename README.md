# Intelligent Error Log Analyzer for Developers

A web-based application that helps developers **analyze large log files**, **detect errors**, **group similar error patterns**, and **visualize error trends** using Machine Learning (TF-IDF + Cosine Similarity).

---

## Project Overview
Modern applications generate huge volumes of logs. Manually finding the root cause of errors is time-consuming and inefficient.  
This project automatically:
- parses raw logs
- extracts error entries
- clusters similar errors into groups
- ranks them by frequency/severity
- shows insights through a dashboard
- exports reports for debugging

---

## Key Features (MVP)
- Upload `.log / .txt / .json` files
- Parse logs into structured format (timestamp, level, message, stack trace)
- Detect and filter error logs
- Cluster similar errors using **TF-IDF + Cosine Similarity**
- Dashboard summary (Total logs, Total errors, Total clusters)
- Error frequency graph (errors over time)
- Cluster details view (sample log + stack trace)
- Export report as **TXT / CSV**

---

## Tech Stack
### Backend
- Python (FastAPI)

### ML / Intelligence
- scikit-learn (TF-IDF Vectorizer + Cosine Similarity)

### Database
- MongoDB

### Frontend
- React

### Charts
- Recharts

---

## Folder Structure
```bash
intelligent-error-log-analyzer/
  backend/
    app/
      main.py
      core/
        config.py
      db/
        mongo.py
      routes/
        upload.py
        analytics.py
      services/
        parser.py
        clustering.py
        export.py
      models/
        schemas.py
    requirements.txt

  frontend/
    src/
      pages/
        Upload.jsx
        Dashboard.jsx
        ClusterDetails.jsx
      components/
        Navbar.jsx
        StatsCards.jsx
        ClusterTable.jsx
        ErrorChart.jsx
      api/
        client.js
      App.jsx
      main.jsx
    package.json

  docs/
    SRS.md
    Architecture.md

  sample_logs/
    sample1.log
    sample2.log

  .gitignore
  README.md
```
## Output Screens

Upload Page

Dashboard Page

Cluster Details Page

Export Report Output