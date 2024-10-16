# Laboratorio Termodinamica

In questa repository vengono caricati i materiali (dati, relazioni, ecc...) del corso di laboratorio di Termodinamica, tenuto dal prof. Daniele Del Re del dipartimento di Fisica dell'università La Spienza (Rm). Il gruppo di laboratorio che gestisce e contribuisce a questo repository è formato da A. Cipriano, M.Cingolo, P.Corrado.

## Indice
1. [Descrizione](#descrizione)
2. [Installazione](#installazione)
2. [Inizializzazione](#inizializzazione)

## Descrizione
Il corso si compone di 6 esercitazione, per ognuna di esse è stata creata una folder,
ogni folder è strutturata nel segunete modo:

- **xx.nome_esercitazione/**
    - **analisi_dati/** 
        contiene gli script python, i notebook jupter usati per l'analisi dei dati
        e i grafici prodotti.
    - **dati/**
        contiene i dati raccolti durante l'esercitazione.
    - **manuali/**
        contiene eventuali manuali di strumenti adoperati per la raccolta delle misure.
    - **note_esercitazione/**
        contiene le note dell'esercitazione fornita dal prof, piu eventuali materiali teorici
        pratici o di qualunque natura che possano essere utili alla stesura della relazione
        o alla comprensione del fenomeno fisico analizzato.
    - **relazione/**
        contiene i modelli latex delle realazioni.


## Installazione
Per interagire con il repository su github e mantenere aggiornati i materiali per tutto il gruppo,
è necessario installare sul propio computer Visual Studio Code, un editor di codice sorgente
che permette di gestire piu task in maniera agevole dalla stessa interfaccia e git che è uno strumento per la gestione
delle versioni del codice (più info sui vari siti):

### Installazione di Visual Studio Code

Per iniziare a utilizzare questo progetto, assicurati di avere installato **Visual Studio Code** sul tuo computer. Puoi seguire le istruzioni per l'installazione qui sotto:

#### Windows
1. Visita la [pagina di download di Visual Studio Code per Windows](https://code.visualstudio.com/download).
2. Scarica il programma di installazione e segui le istruzioni per completare l'installazione.

### macOS
1. Visita la [pagina di download di Visual Studio Code per macOS](https://code.visualstudio.com/download).
2. Scarica il file `.dmg` e segui le istruzioni per completare l'installazione.


### Installazione git
#### Windows

1. **Scarica il programma di installazione di Git**:
   - Visita la [pagina di download di Git per Windows](https://git-scm.com/download/win).
   - Il download dovrebbe iniziare automaticamente. In caso contrario, clicca sul link per scaricare manualmente l'ultima versione.

2. **Esegui il programma di installazione**:
   - Una volta completato il download, apri il file `.exe` scaricato.
   - Segui le istruzioni nella procedura guidata di installazione. Puoi accettare le impostazioni predefinite o personalizzarle secondo le tue preferenze.

4. **Verifica l'installazione**:
   - Puoi verificare che Git sia stato installato correttamente aprendo il terminale (Git Bash) e digitando:
     ```bash
     git --version
     ```

#### macOS

1. **Installa Git tramite Homebrew** (se non hai Homebrew installato, puoi installarlo seguendo le istruzioni su [brew.sh](https://brew.sh)):
   - Apri il terminale e digita:
     ```bash
     brew install git
     ```

2. **Scarica il programma di installazione di Git** (se non vuoi usare Homebrew):
   - Visita la [pagina di download di Git per macOS](https://git-scm.com/download/mac).
   - Scarica il file `.dmg` e segui le istruzioni per completare l'installazione.

4. **Verifica l'installazione**:
   - Puoi verificare che Git sia stato installato correttamente aprendo il terminale e digitando:
     ```bash
     git --version
     ```










## Inizializzazione del Progetto

Segui questi passaggi per clonare e inizializzare il progetto in locale e poter contribuire al repository.

### 1. Clona il Repository

Per iniziare, clona questo repository sul tuo computer locale utilizzando Git. Apri il terminale o Git Bash e digita il seguente comando:

```bash
git clone https://github.com/tuo-utente/tuo-repository.git
```

Dato che questo repository è privato, dovrai autenticarti per clonarlo e lavorarci. 
Quando esegui il comando `git clone`, Git ti chiederà di inserire le tue credenziali GitHub (nome utente e password). 
Il comando git clone scaricherà in automatico tutti i files e le drectory presenti su questo repository sul tuo computer personale


### 2. Naviga nella Cartella del Progetto

Dopo aver clonato il repository, spostati nella cartella del progetto:

```bash
cd nome-della-cartella-del-repository
```

Sostituisci `nome-della-cartella-del-repository` con il nome corretto della cartella del progetto.

### 3. Crea un Branch per Lavorare sulle Tue Modifiche

Prima di iniziare a lavorare, crea un nuovo branch per isolare le tue modifiche dal branch principale:

```bash
git checkout -b nome-del-tuo-branch
```

Sostituisci `nome-del-tuo-branch` con un nome descrittivo per il tuo branch.

### 4. Collegamento con il Repository Remoto (in caso di fork)

Se hai fatto il fork del repository e vuoi collegare la tua copia locale al repository originale per mantenere aggiornato il progetto, puoi aggiungere un **remote upstream**:

```bash
git remote add upstream https://github.com/tuo-utente/tuo-repository.git
```

Verifica che il collegamento sia stato aggiunto correttamente:

```bash
git remote -v
```

### 5. Invia le Tue Modifiche

Dopo aver fatto le modifiche al codice, segui questi passaggi per inviarle al repository:

1. Aggiungi i file modificati allo stage:
   ```bash
   git add .
   ```

2. Crea un commit con una descrizione delle tue modifiche:
   ```bash
   git commit -m "Descrizione delle modifiche"
   ```

3. Invia (push) il tuo branch al repository remoto:
   ```bash
   git push origin nome-del-tuo-branch
   ```

### 6. Sincronizzare il Progetto con il Repository Remoto

Se altre persone hanno apportato modifiche al repository mentre stavi lavorando, è consigliabile sincronizzare il tuo branch con il branch principale (`main` o `master`). Puoi farlo eseguendo un pull dal repository remoto:

```bash
git pull upstream main
```

Oppure, se il branch principale è `master`:

```bash
git pull upstream master
```

### 7. Crea una Pull Request

Dopo aver inviato le tue modifiche, puoi creare una **Pull Request** su GitHub per proporre le tue modifiche al progetto principale.

1. Vai sul repository su GitHub.
2. Clicca su **Pull Requests**.
3. Clicca su **New Pull Request** e seleziona il branch su cui hai lavorato.
4. Descrivi le modifiche e invia la Pull Request.






