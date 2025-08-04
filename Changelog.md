🟢 1.3 04/08/2025
🔴 Pallini colorati e numeri sotto ogni carta
Ogni carta ora mostra:

Una riga di pallini colorati (Rosso, Giallo, Blu, Verde, Bianco, Arcobaleno).

Una riga di numeri da 1 a 5.
🔸 Gli indicatori si “spengono” (opacità ridotta) quando ricevono una negazione.

🛠️ Correzione bug minori
🔵 1.2 03/08/2025
🌙 Wake Lock: lo schermo resta attivo su mobile, con flag dedicato e salvataggio della preferenza in localStorage.

💾 Persistenza dati: lo stato del gioco resta salvato anche dopo il refresh della pagina.

📱 Ottimizzazione mobile: larghezza minima delle carte ridotta da 140px a 120px.

🟡 1.1 — 30/07/2025
🔧 Funzionalità nuove e miglioramenti
✳️ Negazioni automatiche separate:
Le negazioni da "Genera Negazioni" ora compaiono sotto forma di notColorAuto e notNumberAuto sotto ogni carta, con opacità ridotta.

🌈 Gestione migliorata colore/arcobaleno:

Se selezioni più carte, le carte selezionate possono essere del colore indicato o Arcobaleno.

Le altre ricevono negazioni sia del colore che dell’Arcobaleno.

Se selezioni una sola carta, tutte le altre ricevono negazioni complete, perché non è possibile indicare l’Arcobaleno con un solo indizio.

🔄 Esclusione delle carte residue dallo storico (Undo):

I click sulle carte residue non inquinano più lo stack di undo.

💡 Miglioramenti UX
❌ Prevenzione indizi inutili:
Blocca l’assegnazione di indizi se nessuna carta è selezionata.

🌐 Modalità Arcobaleno da URL:
Se disattivata via URL, il colore Arcobaleno viene completamente escluso.

🔁 Nuove modalità di reset delle carte:

sinistra, destra o sostituisci → impostabile da URL.

🏠 Pulsante "Torna alla Home":

Ora con doppia conferma, per evitare reset accidentali.

🔴 1.0 — 29/07/2025
🎴 Hanabi Tracker
Strumento digitale per aiutare i giocatori a tenere traccia delle proprie carte e delle informazioni ricevute durante una partita a Hanabi (competitivo o avanzato).

⚙️ Funzionalità Principali
🔢 Gestione mano:

Scegli tra 4 o 5 carte.

Clicca per selezionare una carta.

Visualizza numero/colore noti e negazioni.

🎨 Indizi:

Seleziona carte → clicca un colore o numero per assegnare l'indizio.

Nessuna carta selezionata = nessun indizio applicato.

🚫 Negazioni automatiche:

Il pulsante "Genera Negazioni" esclude:

Numeri non più presenti per un colore noto.

Colori non più disponibili per un numero noto.

Funziona in base alle carte residue oscurate.

♻️ Reset e sostituzione carte:

Pulsante ✕ per rimuovere una carta.

Viene inserita una nuova carta vuota mantenendo la mano completa.

🧠 Undo:

Annulla l’ultima azione (fino a 100 passaggi).

🃏 Carte Residue:

Visualizza le carte disponibili nel mazzo.

Clic per oscurare → simula l’uscita dal gioco.

Supporto per Arcobaleno (gradiente).

💾 Salvataggio automatico:

Tutto lo stato viene salvato in localStorage.

Puoi chiudere e riaprire la pagina senza perdere nulla.
