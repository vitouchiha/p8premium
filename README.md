# 📺 OMG Premium TV per Stremio

## 👋 Introduzione

Benvenuto in OMG Premium TV, l'addon per Stremio che ti permette di guardare i tuoi canali TV e IPTV preferiti da playlist M3U/M3U8, arricchiti con informazioni sui programmi (EPG). Questa guida ti aiuterà a sfruttare al meglio tutte le funzionalità disponibili.

# 🔄 Changelog di OMG TV

## 🚀 Versione 6.0.0 (Attuale)

### ✨ Nuove funzionalità
- **🐍 Resolver Python**: Sistema completo per risolvere URL di streaming tramite script Python personalizzabili
- **🔄 Canale di rigenerazione**: Nuovo canale nella categoria MANUTENZIONE per rigenerare la playlist senza accedere al pannello web
- **🛠️ Backup e ripristino**: Sistema per salvare e ripristinare la configurazione completa
- **🔧 Template resolver**: Funzionalità per creare automaticamente template di script resolver personalizzabili
- **👤 User-Agent avanzato**: Gestione migliorata degli header User-Agent, Referer e Origin
- **🧩 Moduli Python**: Supporto integrato per request e altri moduli Python per script avanzati

### 🔧 Miglioramenti
- **🐳 Supporto Docker migliorato**: Configurazioni ottimizzate per Hugging Face e Portainer
- **♻️ Cache intelligente**: Sistema di cache completamente ridisegnato con performance migliorate
- **🔄 Aggiornamento pianificato**: Controllo preciso dell'intervallo di aggiornamento in formato HH:MM
- **📋 Interfaccia web rinnovata**: Pannello di configurazione più intuitivo e ricco di funzionalità
- **⚡ Streaming ottimizzato**: Miglior gestione del fallback tra proxy e stream diretti
- **🛡️ Gestione errori robusta**: Sistema migliorato di gestione errori e tentativi multipli

### 🐛 Correzioni
- **🔄 Risolto il loop infinito**: Corretto il problema del loop infinito con resolver e proxy attivi
- **🔌 Migliorata compatibilità**: Risolti problemi di compatibilità con diverse tipologie di playlist
- **🧰 Fix header HTTP**: Corretta la gestione degli header HTTP personalizzati
- **🔍 Fix ricerca canali**: Migliorata la ricerca dei canali per corrispondenza parziale
- **📊 Ottimizzazione EPG**: Risolti problemi con EPG di grandi dimensioni

## 📝 Note di aggiornamento
- Le configurazioni precedenti NON compatibili rispetto alle installazioni di OMG TV e OMG+ TV.
- Si consiglia di eseguire una nuova installazione da zero su Hugging Face o su VPS (consiglio Portainer)
- Per sfruttare le funzionalità del resolver Python, è necessario configurarlo nella sezione avanzata

Per dettagli completi sul funzionamento delle nuove funzionalità, consulta il manuale utente aggiornato.

## 🚀 Iniziamo: Installazione

### Deploy su DOCKER
- Per poter procedere devi prima fare l'installazione tramite docker su Hugging Face o su VPS.
- Segui la guida qui e poi ritorna a questa pagina una volta disponibile il sito web del tuo addon.

### 📲 Installazione dell'addon
1. Apri la pagina web di configurazione OMG TV
2. Configura l'addon secondo le tue esigenze
3. Clicca sul pulsante **INSTALLA SU STREMIO** 🔘
4. Stremio si aprirà automaticamente e ti chiederà di confermare l'installazione
5. Clicca su **Installa** ✅

## ⚙️ Configurazione di base

### 📋 Configurazione della playlist
- **URL M3U** 📋: Inserisci l'URL della tua playlist M3U/M3U8
  - *Esempio*: `http://example.com/playlist.m3u`

### 📊 Configurazione EPG
- **URL EPG** 📊: Inserisci l'URL del file EPG (guida elettronica dei programmi)
  - *Esempio*: `http://example.com/epg.xml` o `http://example.com/epg.xml.gz`
- **Abilita EPG** ✅: Spunta questa casella per visualizzare le informazioni sui programmi

## 🔍 Utilizzo dell'addon

### 📱 Navigazione nel catalogo
1. Apri Stremio
2. Vai alla sezione **Discover** 🔍
3. Seleziona **OMG TV** dalla lista degli addon
4. Vedrai la lista completa dei canali disponibili

### 🎯 Filtraggio dei canali
- **Per genere** 🏷️: Seleziona un genere dal menu a discesa per filtrare i canali
- **Ricerca** 🔍: Usa la funzione di ricerca per trovare canali specifici per nome

### 🎬 Visualizzazione dei dettagli del canale
Clicca su un canale per vedere:
- 📋 Informazioni sul canale
- 📺 Programma attualmente in onda (se EPG abilitato)
- 🕒 Prossimi programmi (se EPG abilitato)
- 🏷️ Categorie del canale

### ▶️ Riproduzione di un canale
- Clicca sul canale e poi sul pulsante **WATCH** ▶️
- Scegli tra le opzioni di stream disponibili:
  - 📺 **Stream Originale**: Lo stream standard dalla playlist
  - 🌐 **Stream Proxy**: Lo stream attraverso un proxy (maggiore compatibilità)
  - 🧩 **Stream Risolto**: Lo stream elaborato da uno script resolver (per canali speciali)

## 🛠️ Impostazioni avanzate

### 🌐 Configurazione proxy
- **Proxy URL** 🔗: URL del proxy per gli stream (è compatibile solo con MediaFlow Proxy)
- **Password Proxy** 🔑: Password per l'autenticazione del proxy
- **Forza Proxy** ✅: Obbliga tutti gli stream ad utilizzare il proxy

### 🆔 Gestione ID e aggiornamenti
- **ID Suffix** 🏷️: Aggiunge un suffisso agli ID dei canali (es. `.it`)
- **Percorso file remapper** 📝: Specifica un file per la rimappatura degli ID EPG
- **Intervallo Aggiornamento** ⏱️: Specifica quanto spesso aggiornare la playlist (formato `HH:MM`)

## 🐍 Funzionalità Python avanzate

### 🔄 Generazione playlist con script Python
1. **URL dello Script Python** 🔗: Inserisci l'URL dello script Python
2. **SCARICA SCRIPT** 💾: Scarica lo script sul server
3. **ESEGUI SCRIPT** ▶️: Esegui lo script per generare la playlist
4. **USA QUESTA PLAYLIST** ✅: Utilizza la playlist generata come sorgente

### ⏱️ Aggiornamento automatico
- Inserisci l'intervallo desiderato (es. `12:00` per 12 ore)
- Clicca su **PIANIFICA** 📅 per attivare gli aggiornamenti automatici
- Clicca su **FERMA** ⏹️ per disattivare gli aggiornamenti

### 🧩 Configurazione Resolver Python
- **URL Script Resolver** 🔗: Inserisci l'URL dello script resolver
- **Abilita Resolver Python** ✅: Attiva l'utilizzo del resolver
- **SCARICA SCRIPT** 💾: Scarica lo script resolver
- **CREA TEMPLATE** 📋: Crea un template di script resolver da personalizzare
- **VERIFICA SCRIPT** ✅: Controlla che lo script resolver funzioni correttamente
- **PULISCI CACHE** 🧹: Svuota la cache del resolver

## 💾 Backup e ripristino

### 📤 Backup configurazione
1. Clicca su **BACKUP CONFIGURAZIONE** 💾
2. Un file JSON verrà scaricato con tutte le tue impostazioni

### 📥 Ripristino configurazione
1. Clicca su **RIPRISTINA CONFIGURAZIONE** 📤
2. Seleziona il file JSON precedentemente salvato
3. Attendi il completamento del ripristino

## ❓ Risoluzione problemi

### ⚠️ Stream non funzionanti
- Prova ad attivare l'opzione **Forza Proxy** ✅
- Verifica che l'URL della playlist sia corretto
- Prova a utilizzare uno script resolver Python per canali problematici

### 📊 Problemi con EPG
- Verifica che l'URL dell'EPG sia corretto
- Controlla che l'opzione **Abilita EPG** ✅ sia attivata
- Assicurati che gli ID dei canali corrispondano tra playlist ed EPG

### 🐍 Problemi con script Python
- Controlla che Python sia installato sul server dell'addon
- Verifica lo stato dello script nella sezione **Stato Script Python**
- Prova a scaricare nuovamente lo script

## 🔄 Aggiornamenti e manutenzione

### 🔄 Modifica delle impostazioni
- In Stremio, vai su **Impostazioni** ⚙️ > **Addon**
- Clicca su **Configura** 🔄 accanto a OMG TV
- Accedi alla pagina di configurazione, fai le modifiche che ti interessano
- Premi su **Genera Configurazione**
- Onde evitare un doppione rimuovi l'addon su Stremio
- Torna alla pagina di configurazione e clicca **Installa su Stremio**

### 🔧 Rigenerazione playlist
- Se hai configurato uno script Python, usa il canale speciale **Rigenera Playlist Python** per ricreare la playlist

## 📋 Riepilogo delle funzionalità principali

- ✅ Supporto playlist M3U/M3U8
- ✅ Supporto guide programmi EPG (XMLTV)
- ✅ Filtri per genere e ricerca
- ✅ Proxy per maggiore compatibilità
- ✅ Resolver Python per stream speciali
- ✅ Generazione playlist personalizzate
- ✅ Aggiornamenti automatici
- ✅ Backup e ripristino configurazione

## 📱 Compatibilità

OMG TV funziona su tutte le piattaforme supportate da Stremio:
- 💻 Windows
- 🍎 macOS
- 🐧 Linux
- 📱 Android
- 📱 iOS (tramite browser web)
- 📺 Android TV
- 📺 Apple TV

## ❤️ Supporto e donazioni

Se apprezzi questo addon, considera una donazione all'autore:
- ☕ **Buy Me a Coffee**: Supporta lo sviluppo di OMG TV
- 💰 **PayPal**: Fai una donazione direttamente all'autore

---

📚 **Nota importante**: OMG Premium TV è progettato per accedere a contenuti legali. Nell'addon non sono inclusi canali o flussi. Assicurati di rispettare la normativa del tuo paese riguardo lo streaming di contenuti.

🌟 Grazie per aver scelto OMG Premium TV! Goditi la visione! 🌟
