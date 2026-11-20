# Dichiarazioni e Attestazioni negli Atti Contabili — Guida Operativa PA

Sito web interattivo di documentazione tecnica e contabile per la Pubblica Amministrazione, pronto per la pubblicazione automatica su **GitHub Pages** tramite **GitHub Actions**.

---

## 📁 Struttura del repository

```text
├── .github/
│   └── workflows/
│       └── deploy.yml    # Workflow GitHub Actions per deploy automatico su GitHub Pages
├── index.html            # Applicazione web interattiva completa (HTML/CSS/JS)
├── .gitignore            # File e directory esclusi dal versionamento
└── README.md             # Guida alla configurazione e pubblicazione
```

---

## 🚀 Guida alla Pubblicazione su GitHub Pages

### 1. Creare un nuovo repository su GitHub
1. Accedi al tuo account [GitHub](https://github.com/).
2. Clicca su **New repository** (o Nuovo repository).
3. Assegna un nome (es. `dichiarazioni-atti-contabili`).
4. Scegli se renderlo **Public** (consigliato per GitHub Pages gratuito) o **Private**.
5. Lascia deselezionate le opzioni "Add a README file" e ".gitignore" (sono già presenti nel pacchetto).
6. Clicca su **Create repository**.

---

### 2. Caricare il codice dal tuo computer

Apri il terminale (o Prompt dei comandi / PowerShell) all'interno della cartella estratta dal pacchetto ed esegui i seguenti comandi:

```bash
# Inizializza il repository locale
git init -b main

# Aggiungi tutti i file
git add .

# Esegui il commit iniziale
git commit -m "feat: rilascio iniziale sito interattivo atti contabili"

# Collega il repository remoto (sostituisci USERNAME e REPO-NAME con i tuoi dati)
git remote add origin https://github.com/USERNAME/REPO-NAME.git

# Esegui il push sul branch main
git push -u origin main
```

---

### 3. Configurare GitHub Pages con GitHub Actions

1. Nel tuo repository su GitHub, vai nella scheda **Settings** (Impostazioni).
2. Nel menu a sinistra, clicca su **Pages** (sotto la voce *Code and automation*).
3. Nella sezione **Build and deployment**:
   - Alla voce **Source**, seleziona dal menu a tendina: **GitHub Actions**.
4. Salva la configurazione se richiesto.

---

### 4. Verifica del Deploy

1. Vai nella scheda **Actions** del tuo repository.
2. Vedrai in esecuzione il workflow `Deploy to GitHub Pages`.
3. Al termine dell'esecuzione (in circa 30-60 secondi, spunta verde), clicca sulla run del workflow o torna in **Settings > Pages**: troverai il link pubblico del sito (ad esempio: `https://USERNAME.github.io/REPO-NAME/`).

---

## 💻 Visualizzazione e Test in Locale

Per testare il sito sul tuo computer prima di pubblicarlo:
- Puoi aprire direttamente il file `index.html` con qualsiasi browser web (Chrome, Edge, Firefox, Safari).
- Oppure avviare un server locale leggero con Python:
  ```bash
  python3 -m http.server 8000
  ```
  e aprire nel browser l'indirizzo: `http://localhost:8000`.

---

## 📄 Note e Crediti
- Realizzato secondo le linee guida operative e le direttive contabili della Ragioneria Generale.
