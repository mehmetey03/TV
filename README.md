# 📺 Lista IPTV + EPG con Proxy

Benvenuto nella tua **lista IPTV personalizzata** con **EPG** integrata e supporto proxy, perfetta per goderti i tuoi contenuti preferiti ovunque ti trovi!

---

## 🌟 Cosa include la lista?

- **🎥 Pluto TV Italia**  
  Il meglio della TV italiana con tutti i canali Pluto TV sempre disponibili.

- **⚽ Eventi Sportivi Live**  
  Segui in diretta **calcio**, **basket** e altri sport. Non perderti neanche un'azione!

- **📡 Sky e altro ancora**  
  Contenuti esclusivi: film, serie TV, sport e molto di più direttamente da Sky.

---

## 🔗 Link pronti all'uso

Queste liste utilizzano un proxy ospitato su **HuggingFace Spaces**.

- **Lista M3U**  
  [`https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/lista.m3u`](https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/lista.m3u)

- **EPG XML**  
  [`https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/epg.xml`](https://raw.githubusercontent.com/nzo66/TV/refs/heads/main/epg.xml)

---

## 📺 Come aggiungere la lista su Stremio

Per utilizzare questa lista IPTV su Stremio, dovrai usare l'addon **OMG Premium TV**:

### 🚀 Installazione OMG Premium TV

1. **Usa questo fork specifico**: [https://github.com/nzo66/OMG-Premium-TV](https://github.com/nzo66/OMG-Premium-TV)  
2. **Deploy su Docker** tramite Hugging Face o VPS seguendo la guida nel repository  
3. **Configura l'addon** inserendo:
   - **URL M3U**: Il link della lista M3U sopra indicato  
   - **URL EPG**: Il link dell'EPG XML sopra indicato  
4. **Installa su Stremio** cliccando sul pulsante "INSTALLA SU STREMIO"

### ✨ Funzionalità disponibili

Con OMG Premium TV potrai sfruttare:
- Supporto playlist **M3U/M3U8** complete  
- **EPG integrata** con informazioni sui programmi  
- **Filtri per genere** e ricerca canali  
- **Proxy per maggiore compatibilità**  
- **Resolver Python** per stream speciali  
- **Backup e ripristino** della configurazione  

---

## 🧩 Proxy: come funziona

Se il proxy fornito non dovesse funzionare o preferisci crearne uno tuo, puoi farlo facilmente.

### ✅ Crea il tuo proxy personalizzato

- **Proxy base consigliato**:
  [tvproxy (repo GitHub)](https://github.com/nzo66/tvproxy)

  `usando questo proxy hai la possibilita' di installarlo su un qualsiasi dispositivo android grazie all'app Termux`

- **Proxy alternativo**:  
  [mediaflow-proxy](https://github.com/mhdzumair/mediaflow-proxy)

- **Per HuggingFace**  
  Usa questa repo ottimizzata: [hfmfp](https://github.com/nzo66/hfmfp)

---

## ⚙️ Personalizza la lista

### 1. Fai il fork della repo

Avvia creando un fork della repository proxy.

### 2. Modifica il file `.env` ed inserisci i tuoi dati.

---

## 🔒 Proxy sicuro con tvproxy

Se utilizzi **tvproxy**, hai la possibilità di lasciare il campo `PROXYIP` vuoto nel file `.env` e proxare direttamente la lista per una maggiore sicurezza.

📘 **Per maggiori informazioni, consulta il repo:**  
👉 [https://github.com/nzo66/tvproxy](https://github.com/nzo66/tvproxy)

### 🔁 Come proxare la lista completa?

Utilizza il seguente URL: `<server-ip>/proxy?url=<URL_LISTA_M3U>`

questo sara il link della tua lista da mettere nelle app iptv!

Sostituisci:

- `<server-ip>` con l'indirizzo IP del tuo server  
- `<URL_LISTA_M3U>` con l'URL effettivo della tua lista M3U (es. quello GitHub)

Questo ti permetterà di servire la lista M3U attraverso il tuo proxy personale in modo sicuro e performante.

---

## 🔒 Proxy sicuro con mediaflow-proxy

Se utilizzi **mediaflow-proxy**, hai la possibilità di lasciare il campo `PROXYIP` vuoto nel file `.env` e proxare direttamente la lista per una maggiore sicurezza.

### 🔁 Come proxare la lista completa?

Utilizza il seguente URL: `https://nzo66-mfpform3u.hf.space/proxy?<server-ip>:<password>?url=<url-lista>`

questo sara il link della tua lista da mettere nelle app iptv!

Sostituisci:

- `<server-ip>` con l'indirizzo IP del tuo server MFP
- `<password>` con la password del tuo mediaflow-proxy  
- `<url-lista>` con l'URL effettivo della tua lista M3U (es. quello GitHub)

Questo ti permetterà di servire la lista M3U attraverso il tuo proxy personale in modo sicuro e performante.

---

## 🚀 Esecuzione automatica con GitHub Actions

Dopo le modifiche:

1. Vai sulla sezione **Actions** della tua repo  
2. Avvia manualmente lo script  
3. Assicurati che **GitHub Actions sia abilitato** nella repository  

---

## 🤝 Hai bisogno di aiuto?

Apri una **issue** o proponi un miglioramento con una **pull request**.  
Contribuire è sempre benvenuto!
