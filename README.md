<<<<<<< HEAD
<<<<<<< HEAD

# 🧠 AO Analysis & Chat Agent

Ce projet est une **application complète** basée sur **Flask (Backend)** et **React (Frontend)** permettant de :

- Scraper des **appels d’offres marocains**.
- Analyser automatiquement les **documents (PDF, Word, Images)**.
- Générer des **réponses intelligentes** grâce à l’API **Groq**.
- Gérer les données via une **base SQLite**.
- Fournir une **API REST** pour communiquer avec le frontend.

---

## 1. Installation du projet

### ⚙️ Prérequis

Avant de commencer, assurez-vous d’avoir installé :

- **Python 3.10+**
- **Node.js (version 18 ou plus)**
- **Google Chrome** + **ChromeDriver**
- **Tesseract OCR**
- **Poppler**

---

## 2. Installation du Frontend

### Étape 1 : Installer Node.js

Télécharger Node.js depuis :  
🔗 [https://nodejs.org/](https://nodejs.org/)

Vérifier l’installation :

```bash
node -v
npm -v
```

### Étape 2 : Démarrer le frontend

```bash
cd ./frontend
npm install
npm run dev
```

---

## 3. Installation du Backend

### Étape 1 : Accéder au dossier

```bash
cd ./back_end
```

### Étape 2 : Installer les dépendances

```bash
python -m venv venv
venv\Scripts\activate      # Windows
source venv/bin/activate     # Linux/Mac

pip install -r requirements.txt
```

## 3. Configuration OCR et Poppler

### 🟣 Installation de Tesseract OCR

#### Windows :

- Télécharger : [https://github.com/UB-Mannheim/tesseract/wiki](https://github.com/UB-Mannheim/tesseract/wiki)
- Ajouter `tesseract.exe` au PATH
- Vérifier :
  ```bash
  tesseract --version
  ```

#### Linux :

```bash
sudo apt install tesseract-ocr
```

#### macOS :

```bash
brew install tesseract
```

---

### 🟢 Installation de Poppler

#### Windows :

- Télécharger : [http://blog.alivate.com.au/poppler-windows/](http://blog.alivate.com.au/poppler-windows/)
- Extraire et ajouter `bin/` au PATH

#### Linux :

```bash
sudo apt install poppler-utils
```

#### macOS :

```bash
brew install poppler
```

---

## 4. Configuration du projet

Créer `config.py` dans `back_end/src` :

```python
GROK_API_KEY = "ta_clé_API_groq"
```

## 5. Lancer l’application complète

**Étape 1 : Lancer le backend**

```bash
cd ./back_end/src
python app.py
```

**Étape 2 : Lancer le frontend**

```bash
cd ./frontend
npm run dev
```

**Étape 3 : Accéder à l’application**

```bash
Frontend → http://localhost:5173

Backend API → http://localhost:5000
```

```text
Back_end/
│
├── src/ # Code source principal
│ ├── configs/ # Configurations globales
│ │ └── agent_config.yaml
│ │
│ ├── agent/ # Comportement et logique de l'agent
│ │ ├── init.py
│ │ ├── base.py # Classe de base (Agent, ToolUser, etc.)
│ │ ├── planner.py # Planification des actions
│ │ ├── executor.py # Exécution des tâches
│ │ ├── memory.py # Gestion mémoire
│ │ ├── tools.py # Outils utilisés par l’agent
│ │ ├── analyse_ao.py # Analyse des appels d’offres
│ │ ├── reponse_ao.py # Gestion des réponses globales
│ │ ├── chat_agent.py # Agent de chat
│ │ └── reponse_agent/ # Réponses modulaires (structurées)
│ │ ├── init.py
│ │ ├── intro_agent.py
│ │ ├── entreprise_agent.py
│ │ ├── finance_agent.py
│ │ ├── methodology_agent.py
│ │ ├── risques_agent.py
│ │ ├── valeur_agent.py
│ │ └── conclusion_agent.py
│
├── docker/
│ ├── Dockerfile
│ ├── docker-compose.yml
│ └── requirements.txt
│
├── docs/
│ ├── README.md
│ ├── api.md
│ ├── setup.md
│ └── architecture.md
│
├── .env
├── .gitignore
├── LICENSE
└── README.md
```

## 👨‍💻 Auteur

**MOHAMMED-AMINE EL HOUSSNI**  
Projet d’analyse d’appels d’offres et agent IA intelligent.  
Développé avec **Flask**, **React**, et **Groq API**.
=======
=======
<<<<<<< HEAD

# 🧠 AO Analysis & Chat Agent

Ce projet est une **application complète** basée sur **Flask (Backend)** et **React (Frontend)** permettant de :

- Scraper des **appels d’offres marocains**.
- Analyser automatiquement les **documents (PDF, Word, Images)**.
- Générer des **réponses intelligentes** grâce à l’API **Groq**.
- Gérer les données via une **base SQLite**.
- Fournir une **API REST** pour communiquer avec le frontend.

---

## 1. Installation du projet

### ⚙️ Prérequis

Avant de commencer, assurez-vous d’avoir installé :

- **Python 3.10+**
- **Node.js (version 18 ou plus)**
- **Google Chrome** + **ChromeDriver**
- **Tesseract OCR**
- **Poppler**

---

## 2. Installation du Frontend

### Étape 1 : Installer Node.js

Télécharger Node.js depuis :  
🔗 [https://nodejs.org/](https://nodejs.org/)

Vérifier l’installation :

```bash
node -v
npm -v
```

### Étape 2 : Démarrer le frontend

```bash
cd ./frontend
npm install
npm run dev
```

---

## 3. Installation du Backend

### Étape 1 : Accéder au dossier

```bash
cd ./back_end
```

### Étape 2 : Installer les dépendances

```bash
python -m venv venv
venv\Scripts\activate      # Windows
source venv/bin/activate     # Linux/Mac

pip install -r requirements.txt
```

## 3. Configuration OCR et Poppler

### 🟣 Installation de Tesseract OCR

#### Windows :

- Télécharger : [https://github.com/UB-Mannheim/tesseract/wiki](https://github.com/UB-Mannheim/tesseract/wiki)
- Ajouter `tesseract.exe` au PATH
- Vérifier :
  ```bash
  tesseract --version
  ```

#### Linux :

```bash
sudo apt install tesseract-ocr
```

#### macOS :

```bash
brew install tesseract
```

---

### 🟢 Installation de Poppler

#### Windows :

- Télécharger : [http://blog.alivate.com.au/poppler-windows/](http://blog.alivate.com.au/poppler-windows/)
- Extraire et ajouter `bin/` au PATH

#### Linux :

```bash
sudo apt install poppler-utils
```

#### macOS :

```bash
brew install poppler
```

---

## 4. Configuration du projet

Créer `config.py` dans `back_end/src` :

```python
GROK_API_KEY = "ta_clé_API_groq"
```

## 5. Lancer l’application complète

**Étape 1 : Lancer le backend**

```bash
cd ./back_end/src
python app.py
```

**Étape 2 : Lancer le frontend**

```bash
cd ./frontend
npm run dev
```

**Étape 3 : Accéder à l’application**

```bash
Frontend → http://localhost:5173

Backend API → http://localhost:5000
```

```text
Back_end/
│
├── src/ # Code source principal
│ ├── configs/ # Configurations globales
│ │ └── agent_config.yaml
│ │
│ ├── agent/ # Comportement et logique de l'agent
│ │ ├── init.py
│ │ ├── base.py # Classe de base (Agent, ToolUser, etc.)
│ │ ├── planner.py # Planification des actions
│ │ ├── executor.py # Exécution des tâches
│ │ ├── memory.py # Gestion mémoire
│ │ ├── tools.py # Outils utilisés par l’agent
│ │ ├── analyse_ao.py # Analyse des appels d’offres
│ │ ├── reponse_ao.py # Gestion des réponses globales
│ │ ├── chat_agent.py # Agent de chat
│ │ └── reponse_agent/ # Réponses modulaires (structurées)
│ │ ├── init.py
│ │ ├── intro_agent.py
│ │ ├── entreprise_agent.py
│ │ ├── finance_agent.py
│ │ ├── methodology_agent.py
│ │ ├── risques_agent.py
│ │ ├── valeur_agent.py
│ │ └── conclusion_agent.py
│
├── docker/
│ ├── Dockerfile
│ ├── docker-compose.yml
│ └── requirements.txt
│
├── docs/
│ ├── README.md
│ ├── api.md
│ ├── setup.md
│ └── architecture.md
│
├── .env
├── .gitignore
├── LICENSE
└── README.md
```

## 👨‍💻 Auteur

**Abdenour TRARI**  
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

```

```

> > > > > > > 29c075eaf8c1e47c237808fee3ff2112424bfb9a
>>>>>>> 23d985bcb6cfa0a830d6a59a2841d3330c8dbc84
