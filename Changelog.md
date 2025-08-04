1.3
Pallini colorati e numeri sotto ogni carta
Ogni carta ora mostra:
Una riga di pallini che rappresentano i colori possibili (Rosso, Giallo, Blu, Verde, Bianco, Arcobaleno).
Una riga di numeri da 1 a 5.
Questi indicatori si “spengono” (con opacità bassa) quando ricevono una negazione.

Correzione bug minori

1.2
Wake Lock: lo schermo resta attivo su mobile, con flag dedicato e salvataggio preferenza in localStorage.
Persistenza dati: lo stato del gioco resta salvato anche dopo il refresh della pagina.
Larghezza minima delle carte ridotta da 140px a 120px per una migliore compatibilità con dispositivi mobili.

1.1
30/07/2025
🔧 Funzionalità nuove e miglioramenti:
Separazione delle negazioni automatiche generate dal pulsante "Genera Negazioni":
Ora notColorAuto e notNumberAuto vengono visualizzate separatamente sotto ogni carta con un'opacità ridotta.
Gestione della logica colore/arcobaleno migliorata:
Quando si selezionano più carte e si dà un indizio di colore, le carte selezionate potranno essere di quel colore o arcobaleno.
Le carte non selezionate ricevono una negazione sia del colore indicato che dell’arcobaleno.
Se viene selezionata una sola carta, le altre ricevono la negazione sia del colore indicato che dell’arcobaleno, perché l’arcobaleno non può essere segnalato con un solo indizio.
Esclusione del tracciamento delle carte residue nello storico (Undo):
Ora cliccare sulle carte residue non viene più registrato nello stack di undo, così da non inquinare la cronologia delle modifiche reali.

💡 Miglioramenti UX:
Prevenzione indizi inutili:
Il sistema blocca l’assegnazione di indizi colore/numero se nessuna carta è selezionata.

Modalità Arcobaleno gestita dinamicamente via URL:
Se disattivata, il colore arcobaleno viene escluso anche nei casi di doppio colore.
Nuova logica per il reset delle carte:
La modalità di reset può essere sinistra, destra, o sostituisci, impostata tramite parametro URL.
Pulsante “Torna alla Home” con doppia conferma:
Previene il ritorno accidentale e il reset dello stato salvato.

1.0
🎴 Hanabi Tracker 29/07/2025 Hanabi Tracker è uno strumento digitale pensato per aiutare i giocatori a tenere traccia delle proprie carte e delle informazioni ricevute durante una partita a Hanabi, specialmente in modalità competitiva o con regole avanzate.
⚙️ Funzionalità Principali 🔢 Gestione delle carte in mano Possibilità di scegliere una mano da 4 o 5 carte.
Le carte possono essere selezionate toccandole o cliccandole.
Ogni carta mostra:
Numero noto o colore noto
Indizi negativi (numeri e colori esclusi)

🎨 Indizi I pulsanti colorati assegnano indizi di colore:

Seeziona le carte a cui si applica → clicca sul colore.
I pulsanti numerici assegnano indizi di numero:
Seleziona le carte a cui si applica → clicca sul numero.
Se nessuna carta è selezionata, nessun indizio viene applicato.

🚫 Negazioni automatiche Il pulsante "Genera Negazioni" esclude automaticamente:
I numeri non più presenti per un colore noto.
I colori non più disponibili per un numero noto.
Funziona in base alle carte residue oscurate.

♻️ Reset e sostituzione carte Ogni carta ha un pulsante ✕ per essere resettata.
Quando una carta viene resettata:
Viene rimossa.
Una nuova carta vuota viene inserita in fondo, mantenendo sempre 4 o 5 carte.
🧠 Undo Il pulsante Undo permette di annullare l’ultima azione (fino a 100 passaggi).
🃏 Carte Residue Rappresentazione visuale delle carte ancora disponibili nel mazzo.
Ogni carta può essere oscurata (clic) per simulare che sia uscita.
Supporta anche il colore Arcobaleno, con visualizzazione a gradiente.

💾 Salvataggio automatico Lo stato della partita viene salvato automaticamente in localStorage.
Puoi chiudere e riaprire il browser senza perdere nulla.
