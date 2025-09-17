# PII Detection & Masking Application (SIH 2024)

## 📌 Project Overview
This project is a **full-stack application** designed for detecting and redacting **Personally Identifiable Information (PII)** from multiple document formats such as PDF, DOCX, TXT, and image files (JPG/PNG).  
The system ensures **privacy preservation, compliance support, and accuracy** in handling sensitive information such as Aadhaar, PAN, Date of Birth, Driving License, Mobile Number, Email, Virtual ID (VID), and Addresses.

- **Backend:** FastAPI  
- **Frontend:** React (Vite)  
- **OCR Support:** Tesseract OCR + Poppler  
- **PII Validation:** Regex + Verhoeff checksum for Aadhaar  
- **Export Options:** PDF, DOCX, PNG  

🔗 **GitHub / Demo URL:** [PII Detector Repository](https://github.com/nanditapanchal/PII-Detector-and-Redaction)

---

## 🚀 Features
- Automatic detection & redaction of Indian PII:
  - Aadhaar (with Verhoeff checksum validation)
  - PAN Number
  - Date of Birth (DOB)
  - Driving License (DL)
  - Mobile Number
  - Email Address
  - Virtual ID (VID)
  - Residential Address
- OCR support for scanned PDFs and images
- High-accuracy PII detection with **regex + checksum validation**
- Preservation of **document layout and formatting** after redaction
- Interactive UI with:
  - Drag & Drop Upload
  - Real-time preview
  - Color-coded PII highlighting
- Export sanitized files in multiple formats (PDF, DOCX, PNG)

---

## 🛠️ System Architecture
```
extractor/   → Extracts text from PDF, DOCX, TXT, Images (OCR)
detector/    → Regex + checksum-based PII detection
redactor/    → Masks or removes detected PII while preserving layout
frontend/    → React-based interactive UI
backend/     → FastAPI for APIs, file handling, and processing
```

---

## 👩‍💻 Role & Contributions
- Designed and implemented the **full-stack application** with FastAPI (backend) and React/Vite (frontend).
- Built **modular pipelines** (`extractor/`, `detector/`, `redactor/`) ensuring scalability and maintainability.
- Integrated **Tesseract OCR & Poppler** for handling scanned documents and low-quality inputs.
- Developed **interactive upload UI** with live preview, highlighting, and export support.
- Optimized **OCR preprocessing** to improve Aadhaar & DOB detection accuracy.
- Solved **format preservation challenges** for PDF and DOCX redaction.

---

## 🧩 Challenges Solved
- Preserved **original formatting** while masking sensitive information in PDFs & DOCX.
- Improved **OCR accuracy** on noisy scans and multi-page PDFs.
- Balanced **performance & accuracy** by implementing **page-wise processing** for large files.
- Implemented **confidence-based filtering** to reduce false positives in detection.

---

## 📊 Impact
- Reduced manual compliance workload by **up to 80%** in testing scenarios.
- Improved Aadhaar & DOB detection accuracy by **~30%** with OCR preprocessing.
- Delivered a **privacy-preserving redaction tool** extendable for enterprise-grade compliance and security.

---

## ⚡ Installation & Setup

### Backend (FastAPI)
```bash
git clone https://github.com/nanditapanchal/PII-Detector-and-Redaction.git
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

### Frontend (React + Vite)
```bash
cd frontend
npm install
npm run dev
```

---

## 📌 Usage
1. Upload a PDF, DOCX, TXT, or Image file through the frontend.
2. System extracts text (OCR if needed).
3. PII elements are detected & highlighted.
4. Masked document can be previewed & downloaded in preferred format.


---

## 👥 Contributors
- **Nandita Panchal** – Full-stack development, OCR integration, PII detection & redaction pipeline, UI/UX

---
