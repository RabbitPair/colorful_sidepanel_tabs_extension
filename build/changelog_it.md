# Changelog

Tutte le modifiche rilevanti a questo progetto saranno documentate in questo file.

Questo progetto aderisce al [Versionamento Semantico](https://semver.org/).

----

## [Non rilasciato]

- **Snapshot programmati**: Salva automaticamente gli snapshot a intervalli specificati. Questa funzione garantisce che il tuo lavoro venga periodicamente salvato, fornendo una rete di sicurezza contro la perdita di dati.

----
## [2.11.0] - 2024-10-07
### Aggiunto
- **Menu Tab**: Sono stati aggiunti nuovi menu:
  - **Rinomina Titolo Tab**: Consente di cambiare il titolo del tab. Per impostazione predefinita, l'opzione per ricordare le impostazioni dell'URL è selezionata, quindi il titolo verrà aggiornato automaticamente la prossima volta che apri l'URL.
  - **Sposta Tab in Nuova Finestra**: Consente di spostare il tab in una nuova finestra.
  - **Sposta Tab in un'Altra Finestra**: Consente di spostare il tab in un'altra finestra esistente.
  - **Rimuovi Tab dal Gruppo**: Consente di rimuovere il tab dal gruppo corrente.

- **Impostazioni Tab**: Sono state aggiunte nuove opzioni alle impostazioni dei tab:
  - **Numero Massimo di Linee Mostrate per il Titolo del Tab**: Imposta il numero massimo di linee da visualizzare per i titoli dei tab. Le linee aggiuntive verranno nascoste.
  - **Numero Massimo di Linee Mostrate per il Titolo del Gruppo**: Imposta il numero massimo di linee da visualizzare per i titoli dei gruppi. Le linee aggiuntive verranno nascoste.
  - **Larghezza del Titolo del Gruppo Collassato**: Quando il gruppo è collassato, imposta la larghezza del titolo del gruppo.
  - **Mostra Conteggio Tab del Gruppo**: Mostra il numero di tab in ogni gruppo accanto al nome del gruppo.

- **Impostazioni del Sito**: Sono state aggiunte nuove opzioni alle impostazioni del sito:
  * **Mantieni Attiva la Pagina**: Quando abilitato, il tab sarà consentito di essere scartato dal browser. Se abiliti le impostazioni di prestazione e imposti un tempo per scartare i tab inattivi, il tab verrà scartato dopo il tempo specificato. Se disabilitato, il tab non verrà scartato.
  * **Unione Automatica al Gruppo**: Quando abilitato, il sito creerà automaticamente o si unirà al gruppo specificato.
  * **Modalità Incognito**: Quando abilitato, puoi scegliere di cancellare automaticamente i dati di navigazione alla visita del sito. Questo include diverse opzioni configurabili: Cookie, Cronologia, CacheStorage, FileSystems, IndexedDB, LocalStorage, ServiceWorkers e WebSQL. Nota che il permesso browsingData non viene utilizzato per evitare di richiedere permessi aggiuntivi.
  * **Aggiornamento Automatico**: Nelle impostazioni di configurazione del link, puoi specificare URL da aggiornare automaticamente, con supporto per espressioni regolari.

### Modificato
- **Picture-in-Picture Avanzato**: Aggiunto supporto universale per i sottotitoli per il lettore plyr.
- **Mantieni Attiva la Pagina**: Funzionalità migliorata per mantenere attivi i tab.
- **Stile dei Tab del Gruppo**: Modificato lo stile dei tab all'interno dei gruppi.
- **Ordine del Menu**: Regolato l'ordine degli elementi nel menu dei tab.

### Risolto
- **Picture-in-Picture**: Risolto un problema in cui il titolo non cambiava dopo aver cambiato video nel lettore Picture-in-Picture.
- **Assegnazioni Personalizzate dei Gruppi**: Risolto un problema in cui le modifiche alle assegnazioni personalizzate dei gruppi per i siti web non avevano effetto immediato quando l'opzione "Ricorda raggruppamento del sito" era abilitata nelle impostazioni dei Gruppi di Tab Avanzati. Questo è stato risolto per applicare le modifiche istantaneamente senza richiedere un riavvio.

----

## [2.10.2] - 2024-10-07

- Risolto il problema in cui i danmaku (commenti a proiettile) si fermavano o scomparivano su alcuni siti web dopo il cambio di pagina (evento di nascondimento della pagina)
- Nascosti i controlli video HTML5

----
## [2.10.1] - 2024-10-05

### Risolto
- Risolto il problema in cui gli eventi di scorciatoia venivano attivati ripetutamente durante la riproduzione consecutiva di più video
- Risolto un problema in cui il lettore non riusciva a ripristinarsi in determinate situazioni
- Risolto il problema in cui la barra di avanzamento della riproduzione non funzionava correttamente quando si utilizzava la modalità Picture-in-Picture
- Risolto il problema in cui il cambio di scheda attivava un toast di rilevamento Picture-in-Picture dopo aver navigato da una pagina con un video a una pagina senza video nella stessa scheda
- Risolto il problema in cui la finestra Picture-in-Picture non si chiudeva quando si usciva dalla modalità Picture-in-Picture utilizzando jwPlayer
- Risolto il problema in cui un indirizzo errato causava il crash della pagina durante l'impostazione di un'immagine di sfondo

----
## [2.10.0] - 2024-10-01

### Aggiunto
- **Documento Picture-in-Picture**: Introduzione di Advanced Picture-in-Picture, disponibile per una prova gratuita prima del rilascio ufficiale della versione premium dell'estensione. Quando abilitato, ha la precedenza sul Picture-in-Picture standard. Se la pagina corrente non lo supporta, verrà utilizzata la modalità standard. Advanced Picture-in-Picture presenta un lettore video personalizzato con funzionalità come:
  * **Riproduci/Pausa video** (Spazio o K)
  * **Regola volume** (Freccia su/giù)
  * **Disattiva/Attiva audio video** (M)
  * **Avanzamento rapido/Indietro video** (Freccia sinistra/destra o Rotella del mouse)
  * **Avanzamento rapido/Indietro video di 5 secondi** (Freccia sinistra/destra)
  * **Avanzamento rapido/Indietro video di 10 secondi** (J/L)
  * **Riproduci il video successivo** (Shift + N)
  * **Riproduci il video precedente** (Shift + P)
  * **Mostra sottotitoli** (supportato su alcuni siti web come youtube.com, vimeo.com, tver.jp, ecc.) (C)
  * **Mostra commenti** (supportato su alcuni siti web come nicovideo.jp, bilibili.com, ecc.) (D)
  * **Esci da Picture-in-Picture** (Esc)
  * **Alterna nascondi/mostra video e riproduci/pausa** (Q)
  * **Alterna schermo intero** (F)
  * **Regola velocità di riproduzione** ( > o <)
  * **Vai all'inizio/fine del video** (Home/End)
  * **Vai a una percentuale del video** (0-9)
  * **Adatta finestra alle dimensioni del video** (W)
  * **Alterna Picture-in-Picture dalla pagina principale** (Alt + P)
  
  > Se i siti web che visiti frequentemente supportano sottotitoli o commenti, puoi inviare un [problema: Advanced Picture-in-Picture](https://github.com/RabbitPair/colorful_sidepanel_tabs_extension/issues/new?assignees=&labels=&projects=&template=Advanced-Picture-in-Picture.md&title=), e lo adatteremo il prima possibile. Si prega di notare che alcuni siti web possono avere restrizioni regionali, richiedendo informazioni aggiuntive.
- **Scorciatoia per Picture-in-Picture**: È stata aggiunta una nuova scorciatoia da tastiera Alt+P per attivare rapidamente la modalità Picture-in-Picture. Questo consente agli utenti di passare facilmente i video alla visualizzazione Picture-in-Picture senza usare il mouse, migliorando la produttività e le capacità di multitasking.
- **Alterna Picture-in-Picture nella Barra di Navigazione Inferiore**: Ora puoi aggiungere un'opzione di attivazione Picture-in-Picture alla barra di navigazione inferiore. Questo può essere configurato nelle impostazioni di aspetto sotto "Mostra barra di navigazione inferiore" - "Configura".
- **Ordina Schede per URL**: È stata aggiunta una nuova opzione di menu "Ordina Schede per URL" al menu "Altro".
- **Comportamento di Collasso del Gruppo di Schede**: È stata aggiunta una nuova opzione "Comportamento di Collasso del Gruppo di Schede" al menu "Gruppo di Schede Avanzato". Puoi modificare il comportamento del collasso dei gruppi di schede nel browser. Le opzioni includono: 'Mostra gruppo corrente e collassa altri gruppi', 'Espandi tutti i gruppi' e 'Usa impostazioni predefinite del browser'.
- **Impostazioni del Sito**: Sono state aggiunte tre nuove opzioni alle impostazioni del sito:
  * **Azione di Restrizione Picture-in-Picture**: Configura l'azione per le restrizioni di Picture-in-Picture.
  * **Entra automaticamente in Picture-in-Picture**: Entra automaticamente in modalità Picture-in-Picture quando è presente un video all'ingresso nella pagina.
  * **Impostazioni dei Sottotitoli**: Configura i selettori CSS per l'elemento dei sottotitoli e il suo elemento padre nella pagina.

### Modificato
- Quando la scheda del pannello laterale non è aperta, se "Picture-in-Picture al Cambio di Scheda" è abilitato (abilitato per impostazione predefinita), entrerà automaticamente in modalità Picture-in-Picture (Promemoria importante: è richiesta l'interazione dell'utente, come fare clic sulla pagina che riproduce il video per attivare l'interazione dell'utente).
- Quando si chiude la barra laterale della pagina, ora viene rimossa invece di essere nascosta. Riapparirà solo dopo aver aggiornato la pagina.

### Risolto
- Risolto il problema per cui l'elenco di Accesso Rapido non gestiva più URL.

----

## [2.9.0] - 2024-09-15
- Aggiunto **Cancella Schede**: Salva uno snapshot e chiudi tutte le schede tranne quella attiva. Ripristinale dalle schede chiuse di recente o dagli snapshot.
- Aggiunto **Attivazione Automatica Raggruppamento Schede**: Crea automaticamente un nuovo gruppo quando si apre una nuova scheda. Le schede successive aperte da questa scheda si uniranno al gruppo.
- Aggiunto **Spaziatura Verticale Elenco**: Nuova opzione nelle impostazioni del Gruppo Schede Avanzato per regolare la spaziatura verticale degli elementi dell'elenco.
- Aggiunto **Aggiungi Più URL a Accesso Rapido**: Consente di aggiungere gruppi e selezionare più schede da salvare in Accesso Rapido.
- Aggiunto **Spaziatura Elementi Accesso Rapido**: Imposta la spaziatura verticale/orizzontale per gli elementi di Accesso Rapido nella pagina delle opzioni.

---
## [2.8.0] - 2024-09-12

### Aggiunto
- Aggiunto **Cronologia schede**: Ora puoi facilmente vedere quali siti web sono stati aperti sotto lo stesso tab. Clicca con il tasto sinistro per aprire il sito web nel tab corrente, clicca con il tasto centrale o Ctrl+clic sinistro per aprire il sito web in un nuovo tab. Per ulteriori dettagli, consulta la pagina delle opzioni.
- Aggiunto **Nomi gruppi personalizzati**: Nella pagina delle opzioni - Gruppo schede avanzato, puoi aggiungere qui alcuni gruppi predefiniti, in modo da poterli selezionare rapidamente quando devi aggiungere schede a un gruppo. Abbiamo già preimpostato alcuni nomi di gruppo, che puoi modificare o eliminare secondo le tue esigenze.
- Aggiunto **Usa nome cartella segnalibri come nome gruppo**: Nella pagina delle opzioni - Gruppo schede avanzato, è stata aggiunta una nuova opzione. Se il sito web aperto è un segnalibro, verrà automaticamente aggiunto al gruppo e il nome del gruppo utilizzerà il nome della cartella dei segnalibri.
- Aggiunto **Indice scheda**: Nella pagina delle opzioni, quando abilitato, l'indice scheda verrà visualizzato accanto al titolo, rendendo facile attivare la scheda usando [Ctrl+numero] su Windows o [cmd+numero] su Mac. Esempio: 1. stackoverflow.com 2. youtube, in modo che sia facile fare Ctrl + 2 su Windows o cmd + 2 su Mac per andare su youtube
- **Impostazioni sito ottimizzate**: Migliorata l'opzione per impostare il colore di sfondo e il colore del testo per i siti.

### Modificato
- Quando si controllano i segnalibri, consentire l'aggiornamento degli URL reindirizzati. Se l'URL non è accessibile, visualizzare i codici di errore: Risposte di successo (200 – 299), Messaggi di reindirizzamento (300 – 399), Risposte di errore del client (400 – 499), Risposte di errore del server (500 – 599). Per ulteriori dettagli, consulta: https://developer.mozilla.org/en-US/docs/Web/HTTP/Status

### Risolto
- Risolto il problema in cui il popup di modifica del segnalibro non scompariva

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
