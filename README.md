# 🧠 AO Analysis & Chat Agent

Ce projet est une **application complète** basée sur **Flask (Backend)** et **React (Frontend)** permettant de :

* Scraper des **appels d’offres marocains**
* Analyser automatiquement des **documents (PDF, Word, Images)**
* Générer des **réponses intelligentes** grâce à l’API **Groq**
* Gérer les données via une **base SQLite**
* Fournir une **API REST** pour le frontend

---

## ⚙️ Prérequis

Avant de commencer, assurez-vous d’avoir installé :

* **Python 3.10+**
* **Node.js (version 18 ou plus)**
* **Google Chrome + ChromeDriver**
* **Tesseract OCR**
* **Poppler**

---

## 🚀 Installation du projet

### 1️⃣ Frontend (React)

```bash
cd frontend
npm install
npm run dev
```

Frontend accessible sur :
👉 `http://localhost:5173`

---

### 2️⃣ Backend (Flask)

```bash
cd back_end
python -m venv venv
venv\Scripts\activate      # Windows
source venv/bin/activate  # Linux / macOS
pip install -r requirements.txt
```

---

## 🔍 Configuration OCR & Poppler

### Tesseract OCR

**Windows**

* Télécharger : [https://github.com/UB-Mannheim/tesseract/wiki](https://github.com/UB-Mannheim/tesseract/wiki)
* Ajouter `tesseract.exe` au PATH

**Linux**

```bash
sudo apt install tesseract-ocr
```

**macOS**

```bash
brew install tesseract
```

---

### Poppler

**Windows**

* Télécharger : [http://blog.alivate.com.au/poppler-windows/](http://blog.alivate.com.au/poppler-windows/)
* Ajouter `bin/` au PATH

**Linux**

```bash
sudo apt install poppler-utils
```

**macOS**

```bash
brew install poppler
```

---

## 🔑 Configuration de l’API Groq

Créer le fichier `config.py` dans `back_end/src` :

```python
GROK_API_KEY = "votre_cle_api_groq"
```

---

## ▶️ Lancer l’application

### Backend

```bash
cd back_end/src
python app.py
```

Backend API :
👉 `http://localhost:5000`

---

### Frontend

```bash
cd frontend
npm run dev
```

---

## 🗂️ Structure du projet

```text
back_end/
├── src/
│   ├── configs/
│   │   └── agent_config.yaml
│   ├── agent/
│   │   ├── base.py
│   │   ├── planner.py
│   │   ├── executor.py
│   │   ├── memory.py
│   │   ├── tools.py
│   │   ├── analyse_ao.py
│   │   ├── reponse_ao.py
│   │   ├── chat_agent.py
│   │   └── reponse_agent/
│   ├── app.py
│
├── docker/
│   ├── Dockerfile
│   ├── docker-compose.yml
│   └── requirements.txt
│
├── docs/
│   ├── README.md
│   ├── api.md
│   ├── setup.md
│   └── architecture.md
│
├── .env
├── .gitignore
├── LICENSE
└── README.md
```

## 👨‍💻 Auteur

**Mohammed-Amine El Houssni**
Projet d’analyse d’appels d’offres et agent IA intelligent
Développé avec **Flask**, **React**, et **Groq API**
