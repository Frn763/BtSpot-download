# BtSpot

## Scarica

**[Ultima versione: BtSpot-<versione>.apk](https://github.com/Frn763/BtSpot-download/releases/latest)** (in fondo alla pagina, sotto "Assets"). Serve Android 13 o più recente.

Qui ci sono solo l'APK e le istruzioni: il codice dell'app non è pubblico.

BtSpot salva da sola la posizione del telefono quando si scollega da un dispositivo Bluetooth, per esempio l'auto quando spegni il motore. Così, in un parcheggio grande, ritrovi l'auto.

## Prima di iniziare

- Serve un telefono **Android 13 o più recente** (Impostazioni → Info telefono → Versione Android).
- L'app non è sul Play Store: si installa da un file APK (`BtSpot-<versione>.apk`), che ti mando io oppure scarichi dall'ultima Release: <https://github.com/Frn763/BtSpot-download/releases/latest> (in fondo, sotto "Assets").

## Installare l'app

1. Scarica il file `BtSpot-<versione>.apk` sul telefono (dal link qui sopra, in **Assets**, oppure da quello che ti ho mandato).
2. Aprilo dalla notifica del download o dall'app **File**.
3. Android ti chiede di consentire l'installazione da quella app (browser, File, WhatsApp, Telegram…): tocca **Impostazioni**, attiva **Consenti da questa fonte** ("Installa app sconosciute") e torna indietro.
4. Tocca **Installa**.
5. **Play Protect** potrebbe avvisarti che l'app è sconosciuta o non verificata: è normale per un'app che non viene dal Play Store. Tocca **Altri dettagli** → **Installa comunque**. Se ti propone di inviare l'app per l'analisi, puoi scegliere tu.

Dopo l'installazione puoi togliere di nuovo il permesso "Installa app sconosciute" a quella app.

## Primo avvio: permessi

Perché la posizione si salvi anche con l'app chiusa, BtSpot ha bisogno di alcuni permessi. Li trovi tutti in **Impostazioni (ingranaggio in alto) → Affidabilità**: ogni riga dice "A posto" o "Da sistemare" e ha un pulsante che porta al punto giusto. Concedili in quest'ordine:

1. **Posizione precisa**: quando Android chiede, scegli **Mentre usi l'app** e lascia attivo **Posizione esatta**.
2. **Posizione "Consenti sempre"**: Android non lo chiede in una finestra, si fa dalle impostazioni. Il pulsante apre la pagina giusta: **Autorizzazioni → Posizione → Consenti sempre**, con "Usa posizione esatta" attivo. Senza questo l'app non può salvare quando è chiusa.
3. **Dispositivi nelle vicinanze**: **Consenti**. Serve per sapere quando il telefono si scollega dall'auto.
4. **Notifiche**: **Consenti**. Servono solo per la conferma "Posizione salvata"; la posizione si salva comunque.
5. **Batteria**: scegli **Senza restrizioni** (consigliato) oppure lascia **Ottimizzata**. **Non** usare "Limitata": con quella l'app non funziona in background.
6. **"Sospendi attività app se inutilizzata"**: va **disattivato** (Info app, voce in fondo). BtSpot si apre di rado: senza questa modifica, dopo qualche mese Android le toglierebbe i permessi e il salvataggio si fermerebbe senza avvisare.

Quando manca qualcosa di essenziale, nella Home compare l'avviso "Salvataggio automatico non attivo" con il pulsante **Risolvi**.

## Aggiungere l'auto (o un altro dispositivo)

1. Prima collega il telefono all'auto via Bluetooth come fai di solito (deve essere già associato).
2. In BtSpot apri **Dispositivi** (in basso) → **Aggiungi dispositivo** e scegli l'auto dall'elenco.
3. Tocca la **stella** accanto all'auto per impostarla come **preferito**: la Home mostrerà dove l'hai lasciata.
4. Se vuoi, dal menu ⋮ della riga scegli **Modifica** per darle un nome più chiaro e un'icona.

L'app salva solo i dispositivi che hai aggiunto qui; gli altri (cuffie, smartwatch…) vengono ignorati finché non li aggiungi.

Da quel momento, ogni volta che il telefono si scollega dall'auto, BtSpot salva la posizione e mostra per un minuto una notifica di conferma. Nella Home vedi la mappa rotonda con te e l'auto, la distanza e il pulsante **Indicazioni a piedi**.

## Aggiornare l'app

1. Scarica il nuovo `BtSpot-<versione>.apk` dall'[ultima Release](https://github.com/Frn763/BtSpot-download/releases/latest).
2. Aprilo e tocca **Aggiorna** (installa sopra la versione che hai già).

**Non disinstallare** prima di aggiornare: la disinstallazione cancella dispositivi e posizioni salvate. Installando sopra, i dati restano.

## Privacy

- Le posizioni salvate restano **solo sul tuo telefono**: nessun account, nessun server mio.
- Per mostrare il nome del luogo ("Forse in Via …") l'app invia a **Nominatim** (OpenStreetMap) le coordinate delle posizioni salvate, non la tua posizione attuale.
- Se accendi il **percorso a piedi** (pulsante con l'icona del percorso) con la Home aperta, l'app invia al servizio di percorsi di **FOSSGIS** (routing.openstreetmap.de) la tua posizione attuale e quella dell'auto. Con il percorso spento non invia nulla.
- La mappa si scarica da OpenFreeMap (o dal fornitore dello stile scelto nelle Impostazioni), come succede con qualsiasi mappa online.

## Da sapere

BtSpot è un progetto personale che condivido con pochi amici: **nessuna garanzia**. Il Bluetooth e il salvataggio in background dipendono dal telefono, dalla versione di Android e da come il produttore gestisce la batteria: su alcuni telefoni potrebbe non funzionare sempre. In un parcheggio sotterraneo il GPS può essere impreciso: la notifica lo segnala. Se qualcosa non va, scrivimi.
