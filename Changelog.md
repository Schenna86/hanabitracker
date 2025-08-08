## 🟢 1.5 — *08/08/2025*  

### Nuove funzionalità  
- **Pressione lunga su una carta (≥ 1 secondo)**:  
  - Apre un **overlay rapido** per impostare direttamente **colore** o **numero**.  
  - Funziona sia su **desktop** che su **mobile**.  
  - Click breve continua a funzionare come selezione/deselezione.  

### Miglioramenti UI/UX  
- **Overlay colori**:  
  - Mostra **solo i pallini** dei colori disponibili (senza testo), con tooltip al passaggio del mouse.  
- **Reset carta**:  
  - Non attiva più accidentalmente la pressione lunga.  
- Tutte le funzionalità della **1.4** (probabilità, due colonne, negazioni, ecc.) restano invariate.  

### Correzioni  
- Eliminati possibili falsi trigger del long-press durante altre azioni.  

---

## 🟣 1.4 — *06/08/2025*

### Probabilità colori e numeri sotto ogni carta

- **Ogni carta mostra ora, sotto ogni pallino e ogni numero:**
  - La **percentuale di probabilità** che la carta sia di quel colore (in base alle residue e alle negazioni).
  - La **percentuale di probabilità** che la carta sia di quel numero (in base alle residue e alle negazioni).
- Il calcolo delle probabilità è **dinamico**: ogni volta che cambia una negazione o una carta residue, le percentuali vengono aggiornate in tempo reale.
- I conteggi ora escludono automaticamente le carte certe già in mano ai giocatori.
- Percentuali normalizzate sui soli colori/numeri possibili per quella carta.

### Nuova homepage e setup partita

- La **homepage** ora permette di selezionare:
  - Il **numero di giocatori** (2, 3, 4, 5).
  - Se il **colore Arcobaleno** è attivo.
  - La **modalità di reset** della carta (sinistra, destra, sostituisci).
- Il numero di carte in mano viene **calcolato automaticamente**:
  - 2–3 giocatori: 5 carte a testa.
  - 4–5 giocatori: 4 carte a testa.
- I parametri vengono **trasmessi in automatico** al tracker tramite URL.

### Nuova visualizzazione ottimizzata

- Sotto ogni carta, la visualizzazione di **colori e numeri** con relative probabilità è stata **riorganizzata su due colonne** (colonna colori e colonna numeri) per una migliore leggibilità sia su desktop che su mobile.

### Migliorie tecniche e UX

- **Parametri di setup** ora completamente automatici: il tracker calcola tutto il necessario sulla base di giocatori, arcobaleno e reset.
- **Grafica mobile** ottimizzata per la nuova visualizzazione percentuali e countdown residue.
- **Negazioni automatiche** e tutte le funzionalità precedenti restano perfettamente integrate.

---

## 🟢 1.3 — *04/08/2025* 

### Pallini colorati e numeri sotto ogni carta

- Ogni carta ora mostra:
  - Una riga di **pallini colorati** (Rosso, Giallo, Blu, Verde, Bianco, Arcobaleno).
  - Una riga di **numeri da 1 a 5**.
- Gli indicatori si **spengono** (opacità ridotta) quando ricevono una **negazione**.

### Correzioni

- Bug minori risolti.

---

## 🔵 1.2 — *03/08/2025* 

- **Wake Lock**: lo schermo resta attivo su mobile, con flag dedicato e salvataggio della preferenza in `localStorage`.
- **Persistenza dati**: lo stato del gioco resta salvato anche dopo il refresh della pagina.
- **Ottimizzazione mobile**: larghezza minima delle carte ridotta da **140px** a **120px**.

---

## 🟡 1.1 — *30/07/2025*

### Funzionalità nuove e miglioramenti

- **Negazioni automatiche separate**:
  - Le negazioni da "Genera Negazioni" sono mostrate come `notColorAuto` e `notNumberAuto` sotto ogni carta (opacità ridotta).
- **Logica colore/arcobaleno migliorata**:
  - Se selezioni **più carte**, quelle selezionate possono essere del **colore indicato o Arcobaleno**.
  - Le altre ricevono **negazioni** sia del colore che dell’arcobaleno.
  - Se selezioni **una sola carta**, tutte le altre ricevono **entrambe le negazioni**.
- **Esclusione carte residue dallo storico (Undo)**:
  - I click sulle carte residue **non vengono più tracciati** nello storico.

### Miglioramenti UX

- **Indizi inutili prevenuti**: gli indizi non vengono applicati se nessuna carta è selezionata.
- **Modalità Arcobaleno via URL**: se disattivata, il colore arcobaleno viene escluso anche nei casi di doppio colore.
- **Nuove modalità di reset**: `sinistra`, `destra` o `sostituisci`, impostabili tramite parametro URL.
- **Pulsante "Torna alla Home"** con doppia conferma per evitare reset accidentali.

---

## 🔴 1.0 — *29/07/2025*

### Hanabi Tracker

Strumento digitale per aiutare i giocatori a tenere traccia delle carte e degli indizi in partite a Hanabi, con supporto a regole avanzate e modalità competitiva.

### Funzionalità principali

- **Gestione mano**:
  - Scelta tra 4 o 5 carte.
  - Clic per selezionare.
  - Visualizzazione di indizi noti (colore/numero) e negazioni.

- **Indizi**:
  - Seleziona carte → clic su colore/numero.
  - Se nessuna carta è selezionata, non viene applicato nulla.

- **Negazioni automatiche**:
  - Il pulsante "Genera Negazioni" esclude:
    - Numeri non più presenti per un colore noto.
    - Colori non più disponibili per un numero noto.
  - Basato sulle carte residue oscurate.

- **Reset e sostituzione carte**:
  - Ogni carta ha un pulsante ✕.
  - La carta viene rimossa e sostituita per mantenere la mano.

- **Undo**:
  - Fino a 100 azioni annullabili.

- **Carte Residue**:
  - Visualizzazione delle carte rimaste nel mazzo.
  - Supporto visivo anche per il colore Arcobaleno (gradiente).

- **Salvataggio automatico**:
  - Stato salvato in `localStorage`, anche dopo chiusura browser.
