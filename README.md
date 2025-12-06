
---

# 🔥 SmartStock AI – Intelligent Inventory Management System

### **AI-Powered • Camera Recognition • Barcode/QR • Predictive Analytics • Voice Control • Luxury UI**

SmartStock AI is a **full-stack, AI-powered inventory management system** built inside **Base44 Vibe Coding**, featuring:

* Real-time camera-based product detection
* Barcode & QR scanning
* AI-driven predictive analytics
* Voice-controlled inventory operations
* Fully responsive luxury UI
* Working LLM assistant
* Seamless CRUD with PostgreSQL (Base44)
* Indian currency (₹) support

This system is designed for **enterprises, warehouses, retail chains, startups**, and **AI-based automation projects**.

---

## 🚀 Live Demo

🔗 **Deployed App:** [https://intelli-stock-ai-eb32a194.base44.app](https://intelli-stock-ai-eb32a194.base44.app)

🔗 **Workspace (Editor Preview):** [https://app.base44.com/apps/68fb9c50bb4bef71eb32a194/editor/preview/dashboard](https://app.base44.com/apps/68fb9c50bb4bef71eb32a194/editor/preview/dashboard)

---

## ⚡ Key Features

### 🏠 **1. Ultra-Luxury Dashboard**

* Dark-mode first premium UI
* Real-time stock overview
* Vibrant, high-contrast cards
* Expiry alerts for perishable items
* Multi-location warehouse dashboard
* Charts powered by **Chart.js & Recharts**
* Critical alerts panel
* Smooth animations using **Framer Motion**

---

### 📦 **2. Full Inventory Management (CRUD)**

* Add / Update / Delete items
* Track UID, Quantity, Weight, Expiry Date
* Indian currency (₹) pricing
* Supplier & category management
* CSV / PDF Export (PapaParse + jsPDF)
* Auto-fill product details via Camera or Barcode
* Multi-location inventory simulation

---

### 🎥 **3. Camera-Based Product Recognition (AI)**

Powered by **TensorFlow.js (COCO-SSD)**

* Real-time object detection
* Bounding box overlays
* Auto-populates inventory fields
* Detect product → "Add to Inventory"
* LLM-powered price/category estimation

---

### 📷 **4. Barcode / QR Code Scanner**

Using **QuaggaJS**

* Detects all major barcode standards
* Quick auto-update of stock
* Works on laptop & mobile camera
* Manual fallback supported

---

### 🧠 **5. AI Chat Assistant**

Integrated using Base44 InvokeLLM

* Answers inventory questions
* Suggests reorder quantities
* Predicts future shortages
* Understands voice commands
* Provides warehouse insights
* Uses **HuggingFace or Claude/ChatGPT** via Base44 proxy

Embedded via iFrame for free models like:
`https://huggingface.co/spaces/bigcode/santacoder`

---

### 🔮 **6. Predictive Analytics**

* 7-day stock forecasting
* Usage-rate analysis
* Recommended reorder list
* Visual forecasting charts
* AI-driven insights

---

### 🎤 **7. Voice Control (Speech-to-Text / Text-to-Speech)**

Using Web Speech API

* Check stock via voice
* Add items by speaking
* Speak AI responses aloud
* Hands-free warehouse management

---

### 📊 **8. Reports & Alerts**

* Automated low-stock alerts
* Expiry-based warnings
* Generate PDF/CSV summary reports
* Top moving items
* Items nearing stockout

---

### ⚙️ **9. Settings**

* Dark/Light mode
* Warehouse switching
* User preferences
* Profile display

---

## 🏛️ System Architecture

```
frontend/
├── Dashboard
├── Inventory Management
├── CameraDetection
├── BarcodeScanner
├── VoiceControl
├── Analytics
├── AIAssistant
├── Reports
└── Settings

components/
├── ui/ (Shadcn)
├── StatsCard
├── AlertPanel
└── InventoryChart

backend (Base44)
├── PostgreSQL with RLS
├── Automatic REST API
├── Authentication (JWT)
├── File Storage
└── AI Integrations (InvokeLLM, Email, File Upload)
```

---

## 🧩 Entity Schema (InventoryItem)

| Field               | Type   | Description                |
| ------------------- | ------ | -------------------------- |
| uid                 | string | Unique ID / RFID simulated |
| name                | string | Product name               |
| quantity            | number | Stock count                |
| weight              | number | Weight (kg)                |
| category            | enum   | 7 product categories       |
| expiry_date         | date   | For perishables            |
| unit_price          | number | Indian currency ₹          |
| supplier            | string | Supplier name              |
| barcode             | string | Barcode value              |
| location            | string | Warehouse location         |
| low_stock_threshold | number | Alert threshold            |
| last_restock_date   | date   | Restock history            |

---

## 🔌 Integrations Used

### Base44 Integrations

* **InvokeLLM** → AI assistant, category suggestion
* **UploadFile** → Images / files
* **SendEmail** → Alerts
* **GenerateImage** → AI image generation
* **ExtractDataFromUploadedFile** → CSV import

### External Libraries

* TensorFlow.js (COCO-SSD)
* QuaggaJS (Barcode scanning)
* Web Speech API
* Chart.js + Recharts
* jsPDF, PapaParse
* TailwindCSS + Shadcn UI
* Framer Motion
* Lucide Icons

---

## 🧠 System Flow (High-Level)

### Camera Flow

1. Start camera
2. Detect items
3. Show bounding boxes
4. Call LLM → suggest name/category/price
5. Auto-fill form
6. Save to DB

### Barcode Flow

1. Scan barcode
2. Lookup product
3. Auto-increase stock OR allow add

### Voice Flow

1. SpeechRecognition → text
2. Send to AI
3. Execute command
4. Speak result

### Forecasting Flow

1. Fetch usage history
2. Predict consumption
3. Highlight risk items
4. Render charts

---

## 🛠️ Tech Stack

### **Frontend**

* React 18
* React Router
* TailwindCSS
* Shadcn UI
* Framer Motion
* Recharts & Chart.js
* TensorFlow.js
* QuaggaJS

### **Backend (Base44)**

* PostgreSQL
* Auto-generated REST API
* RLS Security Policies
* Base44 SDK
* LLM Proxy Integration

---

## 📦 Installation (Local Development)

> ⚠️ Full project runs only inside **Base44 platform**.

### Clone the repo

```sh
git clone https://github.com/yourusername/smartstock-ai.git
cd smartstock-ai
```

### Dependencies

No manual install — Base44 auto-handles builds.

---

## 📸 Screenshots (Add Later)

```
/assets/screenshots/
  dashboard.png
  inventory.png
  camera.png
  barcode.png
  ai-assistant.png
  analytics.png
```

---

## 🏁 Roadmap

* Mobile app (React Native)
* ONNX-based offline detection
* Multi-admin collaborative dashboard
* Real IoT load cell/RFID integration

---

## 🤝 Contributing

Pull requests are welcome!
Please follow standard GitHub guidelines.

---

## 📄 License

MIT License © 2025 SmartStock AI / Base44

---

## 💬 Contact

**Developer: Sathya Seelan**
AI Engineer | Full-Stack Developer
SmartStock AI – Base44 Vibe Coding
---

Just tell me!
