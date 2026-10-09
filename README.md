# SwasthyaSetu 

### One Patient. One Health History. Anywhere.

SwasthyaSetu is a rural-focused digital healthcare platform designed to organize patient medical records in one place and help authorized doctors understand a patient's medical history more efficiently.

Patients can access their health records, reports, prescriptions, and health trends, while doctors can review medical history through a structured timeline and AI-assisted summaries.

##  Problem Statement

Patients in rural areas often visit multiple healthcare facilities, including primary health centres, clinics, and district hospitals. Their medical records may be scattered across paper documents and different institutions.

This can make it difficult for doctors to understand a patient's complete medical history, review previous reports, and track changes in health over time.

##  Our Solution

SwasthyaSetu aims to provide a unified digital interface for organizing medical records and improving continuity of care.

Key goals include:

* Organize patient medical records in a structured timeline.
* Provide separate interfaces for doctors and patients.
* Make reports and prescriptions easier to access.
* Extract relevant information from medical reports using OCR and NLP.
* Generate AI-assisted summaries based on available medical records.
* Visualize historical health measurements and trends.
* Support more informed clinical review by keeping summaries linked to their source records.

##  Key Features

* **Doctor Dashboard:** Search for patients and review their medical history.
* **Patient Portal:** Access personal reports, prescriptions, and health information.
* **Medical Timeline:** View past consultations, reports, and prescriptions chronologically.
* **Report Processing:** Planned OCR and NLP support for extracting information from uploaded reports.
* **AI-Assisted Health Summary:** Help doctors review available records more efficiently.
* **Health Trends:** Visualize historical measurements such as HbA1c, blood glucose, and blood pressure.
* **Digital Prescriptions:** Organize prescriptions as part of the patient's medical history.
* **Privacy-Focused Design:** Intended to support authorized access to sensitive medical records.

## 🛠️ Technology Stack

| Component       | Technology                               |
| --------------- | ---------------------------------------- |
| Frontend        | React, TypeScript, Vite                  |
| Styling         | Tailwind CSS                             |
| Charts          | Recharts                                 |
| Icons           | Lucide React                             |
| Backend         | Python, FastAPI                          |
| Data Validation | Pydantic                                 |
| Database        | Supabase PostgreSQL                      |
| Authentication  | Supabase Auth                            |
| File Storage    | Supabase Storage                         |
| OCR             | Tesseract OCR                            |
| NLP and AI      | Python NLP tools and Hugging Face models |

*Some technologies and features are planned and may not yet be integrated.*

##  System Architecture

The planned architecture is:

1. **Frontend:** Doctor and patient interfaces.
2. **Backend:** FastAPI endpoints for patient information and medical records.
3. **Database:** Structured patient information, reports, and prescriptions.
4. **File Storage:** Private storage for uploaded medical documents.
5. **Processing Pipeline:** OCR extracts text, NLP organizes relevant information, and an AI-assisted component summarizes available history.
6. **Visualization:** Medical timelines and historical health trends.

##  Planned Project Structure

```text
SwasthyaSetu/
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── data/
│   │   └── types/
│   └── package.json
├── backend/
│   ├── app/
│   │   ├── routes/
│   │   ├── schemas/
│   │   ├── services/
│   │   └── main.py
│   └── requirements.txt
├── .gitignore
└── README.md
```

*The structure may change as development progresses.*

##  Getting Started

### Prerequisites

* Node.js and npm
* Python 3.11 or a compatible version
* Git

### Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

### Backend Setup

Open a separate terminal:

```bash
cd backend
python -m venv .venv
```

Activate the virtual environment.

**Windows PowerShell:**

```powershell
.venv\Scripts\Activate.ps1
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Start the FastAPI server:

```bash
uvicorn app.main:app --reload
```

The backend will normally be available at `http://127.0.0.1:8000`.

API documentation: `http://127.0.0.1:8000/docs`

*These instructions apply once the corresponding frontend and backend files have been created.*

##  Privacy and Responsible AI

* Use synthetic data for development and demonstrations.
* Restrict access to medical records according to user roles and permissions.
* Keep medical documents in private storage.
* Do not commit passwords, API keys, or environment files.
* AI-generated summaries are intended to assist medical-history review, not replace clinical judgment.
* The system is not intended to independently diagnose diseases or prescribe treatment.

##  Project Scope

SwasthyaSetu is being developed as a healthcare technology prototype for the WhyCode.4U hackathon.

The initial focus is on patient record organization, doctor and patient interfaces, and AI-assisted medical-history review.

Future possibilities include multilingual access, offline support, and interoperability with India's digital health ecosystem, including ABDM/ABHA standards.

##  Future Scope

* Improved OCR for scanned medical documents.
* Multilingual user interfaces.
* More comprehensive health trend visualization.
* Secure interoperability with participating healthcare systems.
* Better support for low-connectivity rural environments.

##  Contributions

Contributions, suggestions, and feedback are welcome. Please open an issue to discuss significant changes before submitting a pull request.

##  Disclaimer

SwasthyaSetu is a prototype and is not a substitute for professional medical advice, diagnosis, or treatment. Features described as planned may not yet be implemented.

---

**SwasthyaSetu — One Patient. One Health History. Anywhere.**
