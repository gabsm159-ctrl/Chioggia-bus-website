# 📦 Guida Pubblicazione su GitHub Pages

## Passaggi per Pubblicare il Sito Web Permanentemente

### 1. Crea un Account GitHub (se non lo hai)
- Vai su [github.com](https://github.com)
- Clicca "Sign up"
- Completa la registrazione

### 2. Crea un Nuovo Repository

1. Accedi a GitHub
2. Clicca il "+" in alto a destra → "New repository"
3. Compila i dettagli:
   - **Repository name**: `chioggia-bus-website`
   - **Description**: "Sito web ufficiale Bus Chioggia - Orari autobus urbani"
   - **Public**: Seleziona questa opzione
   - **Initialize with README**: NO (lo abbiamo già)
4. Clicca "Create repository"

### 3. Carica i File

Hai due opzioni:

#### Opzione A: Via Web (Più Semplice)
1. Nel repository appena creato, clicca "Add file" → "Upload files"
2. Trascina i file nella zona di upload:
   - `index.html`
   - `sitemap.xml`
   - `robots.txt`
   - `README.md`
3. Clicca "Commit changes"

#### Opzione B: Via Git (Più Avanzato)
```bash
cd /home/ubuntu/chioggia-bus-website
git remote add origin https://github.com/TUO_USERNAME/chioggia-bus-website.git
git branch -M main
git push -u origin main
```

### 4. Abilita GitHub Pages

1. Nel repository, vai in **Settings** (Impostazioni)
2. Nella sidebar sinistra, clicca **Pages**
3. Sotto "Build and deployment":
   - **Source**: Seleziona "Deploy from a branch"
   - **Branch**: Seleziona "main" (o "master")
   - **Folder**: Seleziona "/ (root)"
4. Clicca "Save"

### 5. Attendi il Deploy

GitHub Pages farà il deploy automaticamente. Dopo 1-2 minuti, il sito sarà disponibile su:

```
https://TUO_USERNAME.github.io/chioggia-bus-website/
```

### 6. (Opzionale) Usa un Dominio Personalizzato

Per usare un dominio personalizzato (es. `bus-chioggia.it`):

1. Registra il dominio presso un registrar (GoDaddy, Namecheap, ecc.)
2. Nel repository Settings → Pages
3. Sotto "Custom domain", inserisci il tuo dominio
4. Configura i DNS del registrar per puntare a GitHub Pages

---

## Verifica che Tutto Funzioni

Dopo la pubblicazione, verifica che:

- ✅ Il sito è accessibile dall'URL
- ✅ Tutte le sezioni si caricano correttamente
- ✅ La ricerca delle linee funziona
- ✅ I link ai contatti sono attivi
- ✅ Il sito è responsive su mobile

---

## Aggiornamenti Futuri

Per aggiornare il sito in futuro:

1. Modifica i file locali
2. Carica i file aggiornati su GitHub
3. GitHub Pages farà il deploy automatico entro 1-2 minuti

---

## Supporto

Se hai problemi:
- Leggi la [documentazione ufficiale di GitHub Pages](https://docs.github.com/en/pages)
- Verifica che il repository sia pubblico
- Controlla che `index.html` sia nella root del repository
