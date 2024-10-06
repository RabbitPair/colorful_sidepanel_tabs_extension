# Changelog

Tutte le modifiche rilevanti a questo progetto saranno documentate in questo file.

Questo progetto aderisce al [Versionamento Semantico](https://semver.org/).

---

## [2.7.0] - 2024-09-05
### Aggiunto
- Aggiunta **gestione dei segnalibri**: Aggiunta funzionalità completa di gestione dei segnalibri
- Aggiunta **barra di navigazione delle schede**: opzioni nell'aspetto, visualizzazione: schede, segnalibri, cronologia, schede chiuse di recente, elenco di lettura e accesso rapido nel pannello laterale
- Aggiunto menu **Aggiungi scheda al gruppo**: aggiungi schede a un nuovo gruppo o a un gruppo esistente
- Aggiunta evidenziazione delle parole chiave di ricerca
- Aggiunta prenotazione Edizione Premium
### Modificato
- Autorizzazioni per Cookie, Elenco di Lettura e segnalibri regolate a autorizzazioni opzionali, richiedendo l'autorizzazione dell'utente per l'uso
### Deprecato
- **Pagina Opzioni - Cronologia - Mostra nel pannello laterale**: Questa opzione è stata sostituita dalla *barra di navigazione delle schede* e sarà presto deprecata

### Risolto
- Risolto il problema per cui il pulsante di espansione del gruppo non appariva al primo clic sul pannello laterale
- Risolto il problema per cui riaprendo il browser e cliccando sull'icona dell'estensione era necessario riselezionare tra popup o pannello laterale
- Risolto il problema per cui le dimensioni delle icone delle schede bloccate e dell'accesso rapido erano incoerenti

---

## [2.6.1] - 2024-08-30

### Modificato
- Metodo di visualizzazione del menu ottimizzato, migliorati i messaggi di errore
- Aggiunta maggiore compatibilità per i browser basati su Chromium


---

## [2.6.0] - 2024-08-28
### Aggiunto
- Aggiunto **Zoom Menu Schede**: È stata aggiunta una funzione di zoom al menu delle schede, che consente di regolare liberamente il livello di zoom dal 1% al 1000%.

### Modificato
- Accesso Rapido è stato spostato in un elemento di menu separato.
- Ordinamento drag-and-drop ottimizzato

### Risolto
- Risolto un problema per cui alcune aree non cambiavano dopo aver modificato il colore del carattere.

### Deprecato
- **Accesso Rapido nel Menu Schede**: Accesso Rapido è stato spostato in un elemento di menu separato. L'opzione nel menu delle schede sarà presto deprecata (la funzionalità rimane la stessa).

### Rimosso
- Rimossa l'opzione di zoom dalle impostazioni del sito perché regolare lo zoom nel menu non forniva un'anteprima intuitiva delle modifiche. La funzione di zoom è stata spostata nel menu delle schede per un'anteprima in tempo reale.

---

## [2.5.2] - 2024-08-27

### Risolto

- Risolto il problema per cui le immagini di sfondo salvate venivano perse dopo il riavvio dell'applicazione
- Risolto il problema per cui la chiusura di tutte le schede dallo stesso sito in tutte le finestre falliva
- Risolto il crash quando si disabilitava DnD

------

## [2.5.0] - 2024-08-25

### Aggiunto

- Supporto per l'ordinamento drag-and-drop delle schede e dei gruppi nell'ordine delle schede, e sincronizzazione con Chrome
- Sincronizzazione dello stato di espansione del gruppo con Chrome

### Risolto
- Risolto il problema per cui il caricamento di un file di immagine di sfondo troppo grande causava un errore di quota superata QUOTA_BYTES
- Risolto il problema per cui la visualizzazione di tutte le schede della finestra causava un errore e il raggruppamento per sito falliva


---

## [2.4.0] - 2024-08-20

### Aggiunto
- aggiunta **Carica Immagine di Sfondo**: Puoi caricare un'immagine dal tuo dispositivo locale da utilizzare come sfondo.
- aggiunta **Colore di Sfondo Personalizzato**: Ora supporta colori di sfondo personalizzati, e puoi anche scegliere un colore per generare un bellissimo gradiente

### Modificato

- **colore del carattere**: Il colore del carattere cambierà automaticamente in nero o bianco in base al colore dominante dello sfondo o dell'immagine di sfondo. Se l'immagine è grande, potrebbe volerci del tempo per applicare lo sfondo, il che è normale.

### Risolto
- Risolto il problema per cui alcune aree non cambiavano dopo aver modificato il colore del carattere

### Deprecato
- **Stile di sfondo dell'elenco**: Questa funzione imposta lo stile di sfondo per ogni elenco, con alcuni colori sfumati integrati. Tuttavia, con il rilascio dei colori di sfondo personalizzati, la sua missione è stata completata e sarà presto rimossa.

---

## [2.3.0] - 2024-08-16

### Aggiunto
- aggiunta **Barra Laterale Sulle Pagine**: La barra laterale della pagina ti consente di iniettare una barra laterale nelle pagine web che stai navigando senza aprire la barra laterale del browser per gestire le schede. Questa è una funzione molto utile per gli utenti con risoluzioni dello schermo più piccole che trovano la barra laterale del browser troppo larga e non regolabile. Tuttavia, a causa di alcune restrizioni, la barra laterale della pagina offre solo funzionalità molto limitate. Quando questa funzione è abilitata, puoi usare il mouse per passare sopra il bordo della finestra per far apparire la barra laterale.

### Rimosso
- rimosso **Pallina Fluttuante**

---

## [2.2.0] - 2024-08-14

### Aggiunto
- Nuovo menu delle schede **Mantieni Scheda Attiva**: Mantieni la scheda attiva in modo che non venga automaticamente scartata.

### Modificato
- Ottimizzate le prestazioni e ridotte le dimensioni del pacchetto.

---

## [2.1.0] - 2024-08-10

### Aggiunto
- Salva automaticamente le istantanee di finestre, gruppi e schede. Dopo aver riavviato il browser, se è aperta solo una finestra e sono aperte meno di 5 nuove schede, un toast ti inviterà a ripristinare l'ultima finestra e le informazioni sulle schede salvate quando viene aperta la barra laterale.

### Modificato
- Ottimizzati i dati di archiviazione per l'accesso rapido per velocizzare i tempi di accesso.

### Risolto
- Risolti altri problemi minori.

---

## [2.0.1] - 2024-08-09

### Risolto
- Risolto il formato del messaggio per l'importazione riuscita dell'istantanea.
- Risolto il problema per cui le importazioni duplicate causavano voci di accesso rapido ripetute.

---

## [2.0.0] - 2024-08-08

### Modificato
- Rinominata l'estensione da "Colorful Side Panel Tabs" a **"VertiTab - Side Panel Vertical Tabs"**.

### Aggiunto
- Istantanee: Aggiunta una funzione di salvataggio istantaneo delle schede del browser con un solo clic. Puoi salvare le istantanee prima di chiudere il browser e ripristinarle rapidamente la prossima volta che lo apri. Attualmente, è possibile salvare fino a 50 istantanee.
- Barra di Navigazione Inferiore Potenziata: Accedi a più funzionalità dalla barra di navigazione inferiore, come segnalibri, cronologia, schede chiuse di recente, elenco di lettura, accesso rapido, apri nuova scheda, crea istantanea, cerca, comprimi gruppi, ecc.
- Funzionalità di Importazione/Esportazione Aggiornata: Migliorate le opzioni di importazione ed esportazione per gestire meglio le schede su diversi dispositivi.

### Risolto
- Correzioni di bug e miglioramenti della stabilità.

---

## [1.3.3] - 2022-08-04

### Aggiunto
- **Impostazioni dei link**: Le impostazioni del sito ora includono una nuova opzione che ti consente di aggiungere regole per controllare se i link del sito si aprono nella scheda corrente o in una nuova scheda.

---

## [1.3.2] - 2024-08-02

### Risolto
- Risolto il problema per cui il clic con il pulsante centrale del mouse per chiudere la scheda non funzionava.

---

## [1.3.1] - 2024-08-01

### Modificato
- Ottimizzato il layout dell'accesso rapido e aggiunto il supporto per l'ordinamento drag-and-drop.
- Migliorata la logica per espandere tutti i gruppi e ricordare il loro stato.

### Risolto
- Risolto il problema per cui l'importazione dei dati di accesso rapido falliva quando il pannello laterale non era aperto.
- Risolto il problema per cui le icone erano disallineate nella vista del gruppo.
- Risolti altri problemi minori.

---

## [1.3.0] - 2024-07-30

### Aggiunto
- **Importa/Esporta**: Esporta le preferenze utente, l'accesso rapido, le impostazioni del sito web e i dati delle schede chiuse di recente, e importali in un altro browser per sincronizzare i dati dell'estensione.
- **Seleziona accesso rapido dalla cronologia**: Puoi cercare i siti web più visitati dalla cronologia e aggiungerli all'accesso rapido.
- **Più opzioni nella barra degli strumenti**: Aggiungi più opzioni alla barra degli strumenti. Puoi nascondere l'etichetta nella barra degli strumenti e controllare quali icone vengono visualizzate nella barra degli strumenti.

### Modificato
- **Casella di ricerca**: La casella di ricerca ora supporta il tasto Invio per cercare parole chiave in una nuova scheda. Se non ci sono schede o cronologia corrispondenti dopo aver inserito la parola chiave, puoi premere Invio per cercare utilizzando il motore di ricerca predefinito.
- **Inizializzazione dei dati**: Regola il timing dell'inizializzazione dei dati e ottimizza il rendering ripetuto causato dalle modifiche ai dati.
- **URL del changelog**: Aggiorna l'URL del changelog all'URL di rilascio su GitHub.
- **Ottimizzazione del layout**: Ottimizza le modifiche al layout quando cambia la dimensione della finestra.
- **Registrazione dei log degli errori**: Usa Sentry per raccogliere i log degli errori. Stai tranquillo, questa funzione non raccoglierà i tuoi dati privati.

### Risolto
- **Errore di posizione del tooltip**: Risolto il problema per cui il tooltip lampeggiava quando si cambiavano temi e viste nella barra degli strumenti.
- **Navigazione inferiore**: Risolto il problema per cui la navigazione inferiore bloccava l'elenco quando erano aperte molte schede.

---
## [1.2.3] - 2024-07-23

### Risolto
- Risolto il calcolo errato dell'altezza di scorrimento dell'elenco quando le schede bloccate e le icone di accesso rapido superano 1 riga.

### Modificato
- Modificato lo scarto delle schede inattive per escludere le schede bloccate.
- Modificata la chiusura di tutte le schede scartate per escludere le schede bloccate.
- Regolata la dimensione delle icone bloccate e di accesso rapido.

---

## [1.2.2] - 2024-07-19

### Aggiunto
- Aggiungi accesso rapido: Puoi impostare una scheda per apparire in Accesso rapido in modo che sia facile da trovare. Basta fare clic con il pulsante destro del mouse (o premere a lungo) e selezionare Aggiungi a Accesso rapido. Rimuovila quando non ne hai più bisogno facendo clic con il pulsante destro del mouse (o premendo a lungo) e selezionando Elimina da Accesso rapido. La differenza rispetto alle schede bloccate è che Accesso rapido salva l'URL e apre una nuova scheda ogni volta che viene cliccato.

### Modificato
- Le schede bloccate mostrano solo le icone per evitare che vengano cliccate accidentalmente e poi sbloccate.
- Modificata la dimensione delle icone delle schede bloccate.

---

## [1.2.1] - 2022-07-17

### Aggiunto
- Aggiungi nuovo menu alla navigazione inferiore: scarta schede inattive.
- Aggiungi nuovo menu alla navigazione inferiore: chiudi tutte le schede scartate.

### Modificato
- Le modifiche al menu di navigazione inferiore "Raggruppa per sito" influenzano solo la finestra corrente.

### Risolto
- Risolto il problema per cui l'interfaccia utente saltava a causa dell'incoerenza dell'altezza quando si cambiavano le schede attive nell'elenco.

---

## [1.2.0] - 2024-07-16

### Aggiunto
- Aggiungi Configurazioni del sito: Personalizza le impostazioni specifiche del sito, come disabilitare la modalità Picture-in-Picture, disabilitare la modalità di scarto automatico e altro ancora.

### Risolto
- Risolto il problema di creazione o unione automatica del gruppo dello stesso dominio: Risolto un problema per cui la creazione o l'unione automatica dei gruppi dello stesso dominio non funzionava quando una scheda veniva aggiornata.
- Risolto il problema per cui la pagina non riceveva i messaggi di aggiornamento della configurazione: Assicurato che le pagine ricevano correttamente i messaggi di aggiornamento della configurazione.
- Risolti altri bug: Risolti vari altri bug per migliorare la stabilità e le prestazioni.

### Modificato
- Aggiungi opzione per mostrare il pulsante di chiusura al passaggio del mouse: Aggiunta un'opzione per visualizzare il pulsante di chiusura solo quando si passa il mouse su una scheda.

---

## [1.1.0] - 2024-07-13

### Aggiunto
- Aggiungi Opzioni di Prestazioni: Introduci nuove impostazioni di prestazioni per personalizzare e migliorare la tua esperienza di navigazione.
- Aggiungi Icona di Scorrimento alla Scheda Attiva: Naviga facilmente alla scheda attiva con una nuova icona di scorrimento alla scheda attiva.
- Aggiungi Ordina Schede per Dominio: Organizza le tue schede per dominio con una nuova funzione di ordinamento.
- Disattiva Tutte le Schede che Riproducono Suoni: Disattiva rapidamente tutte le schede che stanno riproducendo suoni per un'esperienza di navigazione più silenziosa.

### Modificato
- Rimuovi Icona di Ripristino: L'icona di ripristino è stata rimossa e sostituita con l'opacità del testo dell'elenco impostata a 0,5 per un aspetto più pulito.

### Deprecato
- Rimuovi Ordinamento Drag-and-Drop: La soluzione attuale per l'ordinamento drag-and-drop ha problemi di prestazioni ed è stata temporaneamente rimossa.

---

## [1.0.4] - 2024-07-09

### Aggiunto
- Ordinamento Drag-and-Drop per le Schede: Riorganizza facilmente le tue schede con la funzionalità di drag-and-drop.

### Modificato
- Ottimizza la Velocità di Caricamento della Pagina: Ulteriormente migliorata la velocità di caricamento della pagina per un'esperienza di navigazione ancora più fluida.

---

## [1.0.3] - 2024-07-05

### Risolto
- Risolto Errore del Menu Vista Mista: Risolto un problema per cui il menu vista mista visualizzava errori.

### Modificato
- Ottimizza il Menu del Dominio del Gruppo di Schede: Migliorato il menu del dominio del gruppo di schede per una migliore organizzazione e usabilità.
- Ottimizza il Padding delle Schede: Regolato il padding delle schede per un layout più snello e visivamente accattivante.

---

## [1.0.2] - 2024-07-04

### Aggiunto
- Indicatore della Scheda Attiva Corrente: Identifica facilmente la scheda attiva con un nuovo indicatore visivo.
- Colore del Carattere Personalizzato: Personalizza la tua interfaccia impostando un colore del carattere personalizzato.

### Modificato
- Ottimizza la Velocità di Caricamento: Migliorata la velocità di caricamento per un'esperienza utente più veloce e fluida.

### Impostazioni Predefinite
- Imposta Predefinito per Non Usare la Modalità Colore: L'impostazione predefinita ora utilizza la modalità a colore singolo per un aspetto semplificato.

---

## [1.0.1] - 2024-07-02

### Aggiunto
- Registro Completo della Cronologia per Intervallo di Tempo: Accedi e gestisci la tua cronologia di navigazione con registri dettagliati ordinati per intervallo di tempo.
- Modalità a Colore Singolo per l'Elenco: Introduci una modalità a colore singolo per un aspetto dell'elenco semplificato e coerente.

### Modificato
- Aggiorna il Timing della Barra di Progresso Audio: Migliorata l'accuratezza degli aggiornamenti della barra di progresso audio per un'esperienza multimediale più fluida.
- Ottimizzato il Metodo di Acquisizione delle Icone dell'Elenco: Migliorato il metodo per acquisire le icone dell'elenco, risultando in un caricamento delle icone più veloce e affidabile.

### Risolto
- Risolto il Problema di Visualizzazione dello Stato di Attivazione Errato in Più Finestre: Risolto un problema per cui lo stato di attivazione veniva visualizzato in modo errato quando erano aperte più finestre.

---

## [1.0.0] - 2024-06-29

### Aggiunto
- Interruttore Modalità Chiaro/Scuro: Scegli tra modalità di visualizzazione chiara e scura per adattarsi alle tue preferenze.
- Dimensione del Carattere Personalizzabile: Regola la dimensione del carattere per un'esperienza di lettura più confortevole.
- Layout dell'Interfaccia Personalizzabile: Personalizza il layout dell'interfaccia in base alle tue abitudini di utilizzo.
- Opzioni di Personalizzazione: Aggiungi sfondi colorati e immagini di sfondo per rendere unico il tuo pannello laterale.
- Gestione Avanzata delle Schede: Anteprime delle miniature, opzioni di ordinamento e visualizzazione ricche e un menu di azioni completo per una gestione efficiente delle schede.
- Funzionalità di Ricerca: Cerca rapidamente le schede chiuse di recente o sfoglia la tua cronologia per trovare ciò di cui hai bisogno.
- Modalità Picture-in-Picture: Passa senza problemi alla modalità Picture-in-Picture quando cambi scheda o scorri le pagine.
- Raggruppamento Automatico: Crea o unisci automaticamente gruppi basati sullo stesso dominio per una migliore organizzazione.
- Barra di Progresso di Lettura: Tieni traccia del tuo progresso di lettura in tempo reale per sapere quanto hai letto.
- Barra di Progresso della Riproduzione: Controlla la riproduzione multimediale con opzioni per avanzamento rapido, riavvolgimento, controllo del volume e regolazione della velocità di riproduzione.
