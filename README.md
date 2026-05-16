# BC Transporter Web

## 🚆 Professional Train Tracking Website

BC Transporter Web è una moderna applicazione web professionale per il tracciamento treni in tempo reale su tutta Europa. Convertita dall'app Flutter originale, mantiene tutte le funzionalità con[...]  

## ⚠️ Nota importante / Disclaimer

Questa applicazione non intende in alcun modo sostituire le piattaforme ufficiali delle compagnie ferroviarie o i loro canali di vendita. BC Transporter Web fornisce informazioni e dati di tracciamento a scopo puramente informativo. Per l'acquisto dei biglietti e per verificare disponibilità, tariffe, condizioni di viaggio e conferme ufficiali, è necessario rivolgersi esclusivamente ai canali ufficiali delle compagnie ferroviarie (siti web, app ufficiali, agenzie autorizzate o rivenditori certificati). I biglietti devono essere acquistati tramite le piattaforme ufficiali; BC Transporter Web non vende biglietti e non sostituisce i canali ufficiali di vendita.

Non ci assumiamo responsabilità per acquisti effettuati su canali non ufficiali o per informazioni di prezzo/condizioni non aggiornate. Eventuali link a siti di terze parti sono forniti a scopo di comodità e non implicano approvazione o partnership.

## ✨ Caratteristiche Principali

### 🗺️ Mappa Interattiva in Tempo Reale  
- **Tracciamento Live**: Visualizza la posizione di centinaia di treni in tempo reale  
- **Mappa Interattiva**: Basata su **Mapbox GL JS v3** con stili moderni  
- **Aggiornamento Automatico**: Dati aggiornati ogni 10 secondi  
- **Marker Colorati**: Ogni treno ha un colore unico per facile identificazione  
- **Hover Popup**: Passa sopra i marker per vedere informazioni rapide  
- **Focus Mode**: Concentrati su un singolo treno nascondendo gli altri  

### 🛤️ Dettagli Percorso  
- **Visualizzazione Tracciato**: Linea colorata che mostra il percorso completo  
- **Lista Fermate**: Timeline dettagliata con orari e ritardi  
- **Informazioni Real-Time**: Integrazione con API dynamic-trip  
- **Binari e Platform**: Dettagli precisi per ogni fermata  
- **Ritardi in Evidenza**: Indicatori visivi per ritardi e cancellazioni  

### 🔍 Ricerca Avanzata  
- **Ricerca per Stazione**: Trova partenze e arrivi da qualsiasi stazione  
- **Ricerca per Numero Treno**: Traccia un treno specifico  
- **Autocomplete Intelligente**: Suggerimenti in tempo reale mentre digiti  
- **Ricerche Recenti**: Accesso rapido alle ricerche precedenti  

### 📊 Visualizzazione Dati  
- **Vista Tabella**: Visualizzazione compatta con tutte le informazioni  
- **Vista Carte**: Card eleganti con design moderno  
- **Statistiche Live**: Numero treni attivi, paesi coperti, stato sistema  
- **Informazioni Dettagliate**: Orari, binari, ritardi, destinazioni  

### 📱 Design Responsive  
- **Mobile First**: Ottimizzato per smartphone e tablet  
- **Desktop Ready**: Esperienza completa su schermi grandi  
- **Touch Friendly**: Interfaccia ottimizzata per touch screen  
- **Navigazione Intuitiva**: Bottom navigation per facile accesso  

## 🛠️ Tecnologie Utilizzate  

### Frontend  
- **HTML5**: Markup semantico moderno  
- **CSS3**: Custom properties, Grid, Flexbox, animazioni  
- **JavaScript ES6+**: Moduli, async/await, classi  

### Librerie  
- **Mapbox GL JS v3**: Mappa interattiva professionale con WebGL  
- **Font Awesome 6**: Icone moderne  
- **Google Fonts (Inter)**: Typography professionale  

### API (Si ringrazia [Martin](https://github.com/CuzImMartin) per avermi fornito la possibilità di usare le sue API)  
- **Train Position API**: `https://data.cuzimmartin.dev/train-map` - Posizioni in tempo reale  
- **Route Polyline API**: `https://data.cuzimmartin.dev/trip/{tripId}/polyline` - Tracciati percorsi  
- **Dynamic Trip API**: `https://data.cuzimmartin.dev/dynamic-trip` - Dettagli fermate con orari e ritardi  
- **Backend**: `betacloud-transporter.vercel.app` per ricerche e dettagli  

## 📖 Utilizzo  

### Home Page - Mappa Interattiva  
1. **Visualizza Treni Live**: Marker colorati mostrano tutti i treni in movimento  
2. **Hover su Marker**: Passa sopra un marker per vedere info rapide (numero treno, destinazione)  
3. **Click su Marker**: Clicca per aprire il pannello dettagli con:  
   - Percorso completo tracciato sulla mappa  
   - Timeline fermate con orari previsti/effettivi  
   - Ritardi e informazioni binari  
4. **Focus Mode**: Il treno selezionato rimane visibile, gli altri vengono nascosti  
5. **Auto-Update**: Posizioni e dettagli si aggiornano ogni 10 secondi  
6. **Statistiche Live**: Numero di treni attivi aggiornato in tempo reale  

### Pagina Treni - Ricerca Avanzata  
1. **Seleziona Modalità**: Ricerca per stazione o numero treno  
2. **Inserisci Dati**: Usa l'autocomplete per trovare stazioni  
3. **Visualizza Risultati**: Scegli tra vista tabella o carte  
4. **Filtra Risultati**: Partenze o arrivi  

### Navigazione  
- Usa la **bottom navigation** per spostarti tra le pagine  
- **Home**: Mappa e overview  
- **Treni**: Ricerca dettagliata  
- **Bus**: (In sviluppo)  
- **News**: Ultime notizie ferroviarie  
- **Preferiti**: Salva ricerche e stazioni  
- **Notifiche**: Avvisi e aggiornamenti  

## � Features Avanzate  

### Sistema di Aggiornamento Incrementale  
- Pattern **addAll** per aggiornamenti fluidi senza ricreare marker  
- Rimozione automatica treni dopo 5 minuti di inattività  
- Gestione intelligente dello stato con Map-based storage  

### Gestione Colori Treni  
- Ogni treno ha un colore unico consistente  
- Sistema RGBA per compatibilità con Mapbox expressions  
- Neutralizzazione effetti illuminazione per colori puri  

### Hover Interaction System  
- Timeout di 300ms per transizioni fluide  
- Cancel/Schedule pattern per gestione eventi mouse  
- Popup con glassmorphism e tema dual  

### Focus Mode & View Preservation  
- Focus su singolo treno nasconde gli altri  
- Auto-update non sposta la view durante focus  
- Parametro `fitToView` opzionale per controllo preciso  

## 🎯 Roadmap  

### Completate ✅  
- [x] Mappa interattiva con Mapbox GL JS  
- [x] Tracciamento treni in tempo reale  
- [x] Hover popup sui marker  
- [x] Focus mode (singolo treno)  
- [x] Auto-update ogni 10 secondi  
- [x] Dettagli percorso con timeline fermate  
- [x] Integrazione dynamic-trip API  
- [x] Custom scrollbar  
- [x] Dual theme (chiaro/scuro)  
- [x] Deploy configuration per Vercel  
- [x] Multi-lingua (EN, IT, DE, FR)  

### In Sviluppo  
- [ ] Sistema di autenticazione utenti  
- [ ] Salvataggio preferiti persistente sull'account  
- [ ] Notifiche push  
- [ ] Supporto offline (Service Worker)  
- [ ] Ricerca bus e trasporti pubblici  

### Future Features  
- [ ] Prenotazione biglietti  
- [ ] Condivisione posizione treno  
- [ ] Export PDF itinerari  
- [ ] Integrazione calendario  

## 🤝 Contribuire  

Contributi, issues e feature requests sono benvenuti!  

1. Fork il progetto  
2. Crea un branch per la tua feature (`git checkout -b feature/AmazingFeature`)  
3. Commit le modifiche (`git commit -m 'Add some AmazingFeature'`)  
4. Push al branch (`git push origin feature/AmazingFeature`)  
5. Apri una Pull Request  

## 📝 License  

ISC License - Copyright © 2025 BC Transporter  

## 👨‍💻 Autore  

**Rixolino**  
- GitHub: [@Rixolino](https://github.com/Rixolino)  

**Martin**  
- Martin: [@Martin](https://github.com/CuzImMartin)  

## 🙏 Ringraziamenti  

- Train data API by [cuzimmartin.dev](https://cuzimmartin.dev)  
- [Mapbox](https://www.mapbox.com/) for amazing mapping platform  
- [Font Awesome](https://fontawesome.com/) for icons  
- Backend API: [betacloud-transporter.vercel.app](https://betacloud-transporter.vercel.app)  

---  

**Built with ❤️ for train enthusiasts across Europe** 🚂 🇪🇺  


**Made with ❤️ for train enthusiasts**  

## Caratteristiche  

- **Ricerca Treni**: Cerca treni tra stazioni con date e orari specifici  
- **Treni in Evidenza**: Visualizza i treni più popolari e recenti  
- **Notizie sui Trasporti**: Ultime news dal mondo dei trasporti  
- **Preferiti**: Salva le tue ricerche e tratte preferite  
- **Notifiche**: Ricevi aggiornamenti sui treni che segui  
- **Design Moderno**: Interfaccia responsive e user-friendly  

## Conversione da Flutter  

Questa applicazione web è stata convertita dall'app Flutter originale, mantenendo tutte le logiche e funzionalità principali:  

- Gestione stato con Provider pattern  
- Routing e navigazione  
- API services  
- Modelli di dati  
- Componenti UI  
- Autenticazione utente  
- Notifiche  
- Storage locale  

## Licenza  

Questa applicazione è parte del progetto BC Transporter.
