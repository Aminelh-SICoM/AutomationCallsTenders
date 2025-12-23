
# 🧠 AO Analysis & Chat Agent

**AO Analysis & Chat Agent** est une **application complète full-stack** basée sur **Flask (Backend)** et **React (Frontend)**, conçue pour automatiser l’analyse des **appels d’offres marocains** et assister l’utilisateur à l’aide d’un **agent IA intelligent**.

## ✨ Fonctionnalités principales

* 📡 Scraping automatique des **appels d’offres marocains**
* 📄 Analyse intelligente de documents (**PDF, Word, Images**)
* 🤖 Génération de **réponses assistées par IA** via l’API **Groq**
* 🗄️ Gestion des données avec **SQLite**
* 🔌 Exposition d’une **API REST** pour le frontend
* 💬 Agent conversationnel pour l’assistance à la rédaction

---

## ⚙️ Prérequis

Avant de commencer, assurez-vous d’avoir installé :

* **Python 3.10 ou supérieur**
* **Node.js (version 18 ou plus)**
* **Google Chrome + ChromeDriver**
* **Tesseract OCR**
* **Poppler**

---

## 🚀 Installation du projet

### 1️⃣ Installation du Frontend (React)

```bash
cd frontend
npm install
npm run dev
```

Frontend disponible sur :
👉 `http://localhost:5173`

---

### 2️⃣ Installation du Backend (Flask)

```bash
cd back_end
python -m venv venv
venv\Scripts\activate      # Windows
source venv/bin/activate  # Linux / macOS
pip install -r requirements.txt
```

---

## 🔍 Configuration OCR & Poppler

### 🟣 Tesseract OCR

**Windows**

* Télécharger : [https://github.com/UB-Mannheim/tesseract/wiki](https://github.com/UB-Mannheim/tesseract/wiki)
* Ajouter `tesseract.exe` au PATH
* Vérifier :

```bash
tesseract --version
```

**Linux**

```bash
sudo apt install tesseract-ocr
```

**macOS**

```bash
brew install tesseract
```

---

### 🟢 Poppler

**Windows**

* Télécharger : [http://blog.alivate.com.au/poppler-windows/](http://blog.alivate.com.au/poppler-windows/)
* Ajouter le dossier `bin/` au PATH

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

API Backend :
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
│   │       ├── intro_agent.py
│   │       ├── entreprise_agent.py
│   │       ├── finance_agent.py
│   │       ├── methodology_agent.py
│   │       ├── risques_agent.py
│   │       ├── valeur_agent.py
│   │       └── conclusion_agent.py
│   └── app.py
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

---

## 👨‍💻 Auteur

**MOHAMMED-AMINE EL HOUSSNI**  
Projet d’analyse d’appels d’offres et agent IA intelligent.  
Développé avec **Flask**, **React**, et **Groq API**.
=======

# Appels d'Offres Maroc

Application Flask de scraping d'appels d'offres marocains.

## Installation du projet

git clone https://github.com/HOLOKIATEAM/APPEL_OFFRE

cd appels-offres

pip install -r docker/requirements.txt

python -m src.interfaces.web_ui

## 📚 Documentation

Voir [docs/](docs/README.md)
