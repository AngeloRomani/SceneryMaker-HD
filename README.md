# Scenery Maker HD — progetto iniziale

Questo archivio contiene uno scheletro Android ricostruito da zero. L'APK originale fornito era un pacchetto compilato, non il progetto sorgente: non è stato possibile recuperare automaticamente la logica originale.

## Stato
- Interfaccia Android moderna di partenza.
- Selettore di file TME tramite Android Storage Access Framework.
- Controllo dimensione massima esportabile: 200 MiB.
- Workflow GitHub Actions predisposto per compilare l'APK e creare uno ZIP di distribuzione.
- **Non è ancora implementato** il motore di acquisizione immagini satellitari, la selezione geografica su mappa, né la generazione del formato TME compatibile con Aerofly.

Prima di implementare le immagini satellitari serve scegliere una fonte che autorizzi esplicitamente download, caching e uso offline. Non usare scraping o download massivo da Google Maps/Bing senza licenza appropriata.

## Requisiti
- Android Studio recente / JDK 17.
- Android SDK 35.
- Gradle wrapper generato da Android Studio (oppure aggiungere i file wrapper ufficiali).

## Compilazione locale
Aprire la cartella `project` in Android Studio e lasciare che venga sincronizzata. Il workflow GitHub usa Gradle installato nell'ambiente Actions.
