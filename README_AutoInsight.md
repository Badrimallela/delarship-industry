
# AutoInsight – Intelligent Vehicle Repository System

**AutoInsight** is a centralized and AI-powered platform designed for managing vehicle data, customer records, and inventory operations for the automotive industry. Built using Python with both SQL and NoSQL integrations, it offers a scalable and intelligent solution for dealerships and manufacturers.

---

## 🚀 Key Features

- **Vehicle Inventory Management**: Add, edit, track vehicle details with full VIN mapping.
- **Customer & Sales Management**: Handle customer profiles, purchase history, and transactions.
- **Document Storage**: Securely manage insurance, registration, and warranty documents.
- **AI-Powered Search**: Natural language queries like "Show SUVs under $30K."
- **Power BI Integration**: Real-time analytics and visual dashboards.
- **Role-Based Access Control**: Secure login for admins, sales reps, and managers.

---

## 🛠️ Tech Stack

- **Backend**: Python (FastAPI)
- **Databases**: 
  - SQL (MySQL/PostgreSQL for structured data)
  - NoSQL (MongoDB for document storage)
- **Cloud**: Azure SQL, Azure Blob Storage, Azure Synapse
- **Analytics**: Power BI
- **AI/LLM**: Custom endpoint for natural language inventory search

---

## 📁 Project Structure

```
AutoInsight/
│
├── backend/
│   ├── main.py                # FastAPI app
│   ├── db_sql.py              # SQL integration
│   ├── db_nosql.py            # MongoDB setup
│   └── models.py              # Data models
│
├── data/
│   ├── vehicles.csv
│   ├── customers.csv
│
├── docs/
│   ├── README.md
│   ├── AutoInsight_Code_Section.docx
│
└── scripts/
    └── load_data.py
```

---

## 📦 API Endpoints (Sample)

```http
GET /vehicles/
POST /vehicles/
PUT /vehicles/{vin}
GET /customers/
POST /query-ai   # Natural language vehicle search
```

---

## 🧪 Getting Started

1. Clone the repository:
```bash
git clone https://github.com/yourusername/autoinsight.git
cd autoinsight
```

2. Create virtual environment & install dependencies:
```bash
python -m venv venv
source venv/bin/activate  # Windows: venv\Scripts\activate
pip install -r requirements.txt
```

3. Run the app:
```bash
uvicorn backend.main:app --reload
```

---

## 📊 Power BI & Analytics

Use the view `VehicleSalesDashboard` from SQL to connect to Power BI for real-time dashboards.

---

## 🤖 AI Integration

A minimal LLM integration is available in `/query-ai` for smart queries. Extend with OpenAI API or train custom LLMs using Databricks.

---

## 📄 License

This project is licensed under the MIT License.
