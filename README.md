# Velora

**Scarica e organizza video sul tuo Mac, con un’interfaccia nativa e compatta.**

Incolla un link, scegli la qualità e salva il video nella tua cartella. Se il sito usa un player incorporato, puoi aprirlo nel browser di Velora e cercare i video disponibili nella pagina.

[**Scarica Velora per Mac ↓**](https://github.com/fraprili-code/Velora-updates/releases/latest/download/Velora.dmg) · [Novità e versioni](https://github.com/fraprili-code/Velora-updates/releases) · [Segnala un problema](https://github.com/fraprili-code/Velora-updates/issues)

**Apple Silicon · macOS 14 o successivo · Interfaccia in italiano**

## Cosa puoi fare

| Funzione | Come ti aiuta |
| --- | --- |
| **Link singoli o multipli** | Incolla con ⌘V, trascina i link nella finestra o prepara più download insieme. |
| **Qualità originale, anche 4K** | Conserva la migliore qualità disponibile dal sito. Quando il sito fornisce i dettagli, scegli una sorgente precisa e consulta risoluzione, FPS, HDR e dimensioni. |
| **MP4, MOV e MKV** | Scegli il contenitore del file, mantenendo i codec originali quando compatibili. |
| **Browser integrato** | Apri una pagina, avvia il player e scegli fra i video e le varianti rilevate. Il browser ha una finestra separata. |
| **Playlist** | Esamina gli elementi e seleziona soltanto quelli che vuoi scaricare. |
| **Audio e sottotitoli** | Scegli le lingue e i sottotitoli messi a disposizione dal sito. È disponibile anche il profilo Solo audio. |
| **Coda di download** | Pausa, riprendi, riordina e gestisci più elementi. Imposta download simultanei, limite di velocità e recupero automatico facoltativo. |
| **Libreria locale** | Cerca i video, filtra per sito o periodo, aprili, mostrali nel Finder e rinomina i file. **Pulisci** svuota la cronologia senza eliminare i file, con **Annulla** per ripristinare le voci. |
| **Conversione facoltativa** | Crea una copia in un altro contenitore oppure una copia H.264/AAC compatibile, conservando sempre l’originale. |
| **Integrazione con il Mac** | Modalità mini, barra dei menu, Servizio “Scarica con Velora”, estensione Condividi e notifiche facoltative. |

L’interfaccia segue il tema chiaro o scuro del Mac, permette di cambiare il colore d’accento e rispetta le opzioni Riduci movimento e Riduci trasparenza. Su macOS 26 e successivi usa Liquid Glass; sui sistemi precedenti usa i materiali traslucidi di macOS.

## Installazione

1. Scarica **[Velora.dmg](https://github.com/fraprili-code/Velora-updates/releases/latest/download/Velora.dmg)**.
2. Apri il file e trascina **Velora** nella cartella **Applicazioni**.
3. Avvia l’app da Applicazioni e incolla il primo link.

Il pacchetto include gli strumenti necessari: **non occorre installare Homebrew, Python o FFmpeg separatamente**. Puoi installarlo su più Mac compatibili; ciascun Mac conserva le proprie impostazioni e la propria libreria.

L’estensione Condividi e le notifiche possono richiedere l’abilitazione nelle impostazioni di macOS.

La versione attuale richiede **Apple Silicon** — M1, M2, M3 o successivi — e **macOS 14+**. Non è una build per Mac Intel.

> **Primo avvio:** questa distribuzione personale è firmata localmente, ma non è ancora notarizzata da Apple né firmata con un certificato Developer ID. macOS può quindi bloccarne inizialmente l’apertura. Per valutare l’avviso e autorizzare consapevolmente l’app, consulta la [guida ufficiale Apple](https://support.apple.com/it-it/102445).

## Come si usa

1. Incolla uno o più link nel campo principale; per più video, usa un link per riga.
2. Attendi l’anteprima e scegli qualità e formato. **Qualità originale** include il 4K quando il sito lo offre.
3. Apri **Opzioni del video** per le qualità, le lingue audio e i sottotitoli disponibili.
4. Premi **Scarica** oppure **⌘Invio**. I video terminati compaiono nella **Libreria**.
5. Se il link diretto non funziona, apri **Browser**, avvia il video nella pagina e controlla i video rilevati.

Con **⇧⌘M** passi alla modalità mini: Velora ricorda le dimensioni delle due modalità e, quando espandi, ritorna alla sezione precedente. **⇧⌘V** invia i link copiati al pannello Download.

Nella Libreria, **Pulisci** rimuove le voci dei download completati dalla cronologia, lasciando video e sottotitoli nella loro cartella. Se hai impostato una ricerca o un filtro, **Pulisci risultati** agisce solo sulle voci visibili. Puoi ripristinarle con **Annulla**.

## Qualità originale e conversioni

Velora conserva i flussi offerti dal sito. Se audio e video sono separati, li unisce senza ricodificarli; se serve un contenitore diverso, copia le tracce senza ricodificare video e audio.

**MP4, MOV e MKV sono contenitori:** non tutti accettano gli stessi codec. Se il formato scelto è incompatibile, Velora segnala il problema e propone MKV, senza abbassare silenziosamente la qualità del video.

La conversione si avvia esplicitamente dalla Libreria con **Converti una copia…**. Il file originale viene conservato. Per i video riconosciuti come HDR è disponibile la copia delle tracce originali; la conversione H.264/AAC viene bloccata per evitare un risultato con colori errati. “Originale” indica la sorgente disponibile sul sito, che può essere diversa dal file master caricato dall’autore.

## Aggiornamenti automatici

Sono previsti due aggiornamenti distinti, attivi per impostazione predefinita:

- **Motore di download:** Velora controlla le nuove versioni ufficiali di yt-dlp, che includono correzioni e supporto aggiornato per i siti.
- **App Velora:** controlla le nuove release tramite un catalogo firmato. Verifica firma e integrità del pacchetto; l’installazione automatica attende che l’app sia in background, senza operazioni o link in preparazione. Conserva una copia di recupero e ripristina la versione precedente se il nuovo avvio non viene confermato.

I controlli periodici avvengono mentre Velora è aperta. Puoi avviarli anche da **Impostazioni → Aggiornamenti**. Le nuove funzioni dell’app arrivano quando viene pubblicata una nuova release: il motore non genera nuove funzioni da solo.

## Dati e compatibilità

I file e la cronologia restano sul Mac. Non serve un account Velora e l’app non carica la tua libreria su un servizio cloud. L’anteprima può contattare il sito e caricare miniature già dopo l’incolla. Il browser può caricare anche risorse di terze parti presenti nelle pagine; download e controlli degli aggiornamenti contattano le rispettive sorgenti.

Il download diretto usa [yt-dlp](https://github.com/yt-dlp/yt-dlp), affiancato dal browser integrato. **La compatibilità dipende dal sito:** modifiche ai player, autenticazione o restrizioni del servizio possono impedire un download. Velora non aggira DRM o restrizioni di accesso e non promette di scaricare qualsiasi video. Usala per contenuti che hai il diritto o il permesso di scaricare.

## Segnalazioni

Hai trovato un problema? [Apri una segnalazione](https://github.com/fraprili-code/Velora-updates/issues) indicando versione di Velora, versione di macOS, sito coinvolto e passaggi per riprodurlo. Se utile, aggiungi il messaggio d’errore. Evita password, cookie, link privati e dati personali.

Questo repository distribuisce i pacchetti dell’app e il catalogo degli aggiornamenti; non contiene il codice sorgente completo di Velora. I componenti di terze parti e le relative licenze sono inclusi nel pacchetto.
