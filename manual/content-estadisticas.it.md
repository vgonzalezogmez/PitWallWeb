# Manuale di interpretazione delle viste Live / Statistiche

Guida per i piloti. Senza tecnicismi. L'idea è semplice: **cosa ti dice ogni numero e come usarlo per andare più veloce e più regolare.**

In PitWall corri per **corsie** (C1, C2, C3…) e **ruoti di corsia manche dopo manche**. Per questo ci sono due modi di guardare la tua gara: **cosa succede ADESSO in questa manche** e **come chiuderai ALLA FINE** quando sommi tutte le tue manche. Questo manuale ti insegna a leggere entrambi.

---

## 1. La schermata in diretta

![img: 20-live-timing.png]

È la schermata della manche in corso. Ciò che vedi in tempo reale, giro per giro.

**Orologi per circuito (C1, C2, C3…).** Se la gara usa più circuiti insieme, in alto hai un orologio per ciascuno. Ogni orologio segna il tempo di quella manche su quel circuito. Quando l'orologio arriva a zero, quella manche termina e tutti ruotate di corsia.

**Schede di corsia.** Una scheda per ogni auto in pista. In ogni scheda leggi, a colpo d'occhio:

- **TOTALE** — giri accumulati finora nella manche.
- **ULTIMO** — il tuo ultimo giro completo. È il tuo riferimento immediato: migliori o cali?
- **MEDIA** — il tuo ritmo medio nella manche (media semplice dei tuoi giri, senza contare quello di riscaldamento). È ciò che davvero conta per vincere in resistenza: non il miglior giro isolato, ma il ritmo sostenuto.
- **MIGLIORE** — il tuo miglior giro valido della manche.

**Banner del giro veloce.** Quando qualcuno segna il giro più veloce del momento, appare un avviso in evidenza. Se è tuo, bene. Se è di un rivale, è il metro di misura da battere.

### Le tre viste della diretta (pulsante "Vista")

Con il pulsante **Vista** scegli come mostrare le schede, in base a quante corsie ci sono. Ci sono tre modalità:

**1 · Righe orizzontali** — una riga per corsia. Consigliata per **poche corsie**: ogni corsia occupa una riga larga e si legge molto comodamente.

![img: 31-vista-1.png]

**2 · Griglia compatta** — tutte le piste insieme in griglia. Ideale per **molte corsie**: vedi tutto senza scorrere.

![img: 31-vista-2.png]

**3 · Schede con dettagli** — come la compatta, ma con **VLT** (giri), **SAL** (uscite), **PIT** e **Δ** visibili in ogni scheda. Più informazioni per corsia a colpo d'occhio.

![img: 31-vista-3.png]

---

## 2. Live-stats: le 3 schede

Live-stats è la vista delle statistiche. Ha tre schede e ognuna risponde a una domanda diversa.

**Manche attuale.**

![img: 21-livestats-manga.png]

La classifica di **questa** manche, con il dettaglio di ogni pilota: **G** (giri), **MIGLIORE**, **MEDIA**, **Δ** (delta, il tuo margine), **USCITE** e **PERSO** (tempo perso nelle uscite). Guardalo per sapere come vai ADESSO, con chi condividi la corsia e chi comanda nella tua manche.

**Classifica proiettata.**

![img: 22-livestats-proyectada.png]

La posizione stimata **alla fine della gara**, quando tutti avrete completato tutte le vostre manche. È quella che conta davvero per sapere se stai vincendo. Guardala per sapere la tua posizione REALE nella generale, non solo nella manche che stai correndo.

**Comparativa per corsia.**

![img: 23-livestats-carril.png]

Quanto rende ogni corsia. Alcune corsie sono più veloci di altre. Qui vedi le differenze tra C1, C2, C3… Guardala per sapere se la tua corsia attuale ti aiuta o ti penalizza, e quali corsie ti restano da girare.

**Regola rapida:** *Manche attuale* = la foto di adesso. *Proiettata* = come finisci. *Corsia* = perché il tuo ritmo cambia da manche a manche.

---

## 3. Il tuo pannello (Il mio pannello)

![img: 21b-livestats-mipanel.png]

Scegli il tuo pilota e avrai il tuo pannello personale con delle schede. Una per una:

**POSIZIONE.** Attenzione a questa: è la tua posizione **PROIETTATA di gara**, non quella della manche. Ti dice dove finirai se il ritmo si mantiene. Se nella tua manche sei 4° ma il tuo pannello dice P1, significa che sommando tutte le manche sei primo. Fidati di questa.

**GIRI MANCHE.** Quanti giri hai fatto nella manche attuale.

**MIGLIORE.** Il tuo miglior giro valido. "Valido" significa che **non conta**:
- il **giro di riscaldamento** (il primo, con la confusione del semaforo e del passaggio iniziale),
- né un **passaggio parziale** (un giro che in realtà è mezzo giro contato male),
- né tempi **al di sotto del minimo** della gara (passaggi fantasma impossibili).

Quindi il tuo MIGLIORE è un giro davvero reale, mai un numero regalato.

**MEDIA.** Il tuo ritmo medio. Media semplice dei tuoi giri di gara (include uscite e pit-stop; esclude solo il riscaldamento). È il numero che la proiezione usa per stimare dove finisci. **Abbassa la tua media e sali nella generale.**

**Δ (delta).** È la tua **media pulita meno il tuo miglior giro**. Cioè: quanto margine ti resta. Un Δ piccolo = giri quasi sempre al massimo, poco da raschiare. Un Δ grande = hai ritmo ma lo perdi in molti giri: lì c'è il tuo oro, nell'essere più costante. La "media pulita" qui non conta uscite né pit, solo il tuo girare normale.

**USCITE / PIT-STOP.** Quante volte sei uscito e quante soste hai fatto. Ogni uscita ti costa tempo e posizioni.

**Tempo perso nelle uscite.** Quanto ti sono costate quelle uscite, in secondi. Mettilo in contesto: a volte una sola uscita vale più posizioni che decimi di ritmo per tutta la manche. Qui lo vedi chiaro.

---

## 4. PitWall Lap: la tua gara sul cellulare

![img: 45-lap-access.png]

**PitWall Lap** è il sito web che apri sul **cellulare dal tuo box** per seguire la tua gara in diretta, senza installare nulla. È solo per le **gare di resistenza (a squadre)**. È in sola lettura: consulti il tuo timing, non controlli la gara.

**Come entri.** L'organizzazione ti dà l'indirizzo (qualcosa come `http://<IP-del-server>:3000/lap/<gara>`) e un **PIN di 4 cifre** della tua squadra. Apri l'indirizzo, scegli la tua **squadra** nell'elenco, inserisci il **PIN** e premi **Entra (“Entrar”)**. Con **Cambia squadra (“Cambiar equipo”)** puoi uscire ed entrare con un'altra.

![img: 48-lap-team-panel.png]

**Il tuo pannello.** In alto, la tua **posizione** in grande: è la **proiettata** (dove finirai sommando tutte le manche), la stessa che vedi nella diretta e nella generale — non quella della singola manche. Sotto, la tua distanza dal leader (*"a N giri"*, *"alla pari"* o *"🏁 Leader della gara"*). La riga di stato ti dice in diretta **in quale manche e corsia sei e quanto manca** (o *"In riposo"* / *"In attesa della prossima manche"* / *"Gara finalizzata"*). E le schede:

- **Ultimo giro** — il tuo ultimo giro (lampeggia all'aggiornarsi).
- **Miglior giro** — il tuo miglior giro valido.
- **Giri** — totale accumulato di tutta la gara.
- **Media gara** — il tuo ritmo medio accumulato (quello che usa la proiezione).
- **Pit stop** — soste effettuate.
- **Gap dal leader** — a quanti giri dal primo.

Se c'è la proiezione attiva, compare **Stima alla fine** con la tua **posizione stimata** e i tuoi **giri proiettati**.

**La voce (annuncia-giri).** Con il pulsante **🔊 Voce (“🔊 Voz”)** attivi lo speaker (parte **spento**: bisogna toccare lo schermo una volta perché il cellulare lasci suonare l'audio). Ti annuncia il **tempo di ogni giro**, e avvisa del **cambio di posizione**, **metà manche**, **ultimo minuto**, **ultimi 30 s** e **fine manche**. In **⚙️ Impostazioni voce (“⚙️ Ajustes de voz”)** attivi/disattivi ogni avviso e, nel blocco avanzato, che annunci ogni X minuti la tua **media di corsia**, i **gap con i rivali** o la **media per salire** una posizione.

**Schermo sempre attivo.** Finché il pannello è aperto, lo schermo **non si spegne**; dopo **30 secondi senza toccarlo si oscura** (per non consumare batteria né disturbare), ma **la voce continua ad annunciare**. Tocca lo schermo per illuminarlo di nuovo.

> Consiglio: entra col PIN, attiva la **Voce**, lascia il cellulare nel box e ascolta. È il modo per essere informato senza staccare lo sguardo dalla pista.

## 5. Consistenza

![img: 26-livestats-cons-con.png]

La scheda più importante per migliorare. **La consistenza misura la tua regolarità giro dopo giro**: se fai sempre lo stesso tempo o se fai salti.

**Cos'è la %.** È 100 meno la tua variazione relativa (il CV, coefficiente di variazione). 100% sarebbe un robot perfetto, sempre identico. Più è alta, più sei regolare. Nei dati reali è normale essere **tra 90% e 99%**. È la stessa formula che usa TicTac, calcolata sui tuoi giri di ritmo (scartando gli incidenti puntuali).

**Il ±DS in secondi (più utile della %).** Accanto alla % vedrai qualcosa come *±0,13 s*. È la tua deviazione standard: **di quanti secondi, in su o in giù, oscilli da un giro all'altro.** Bada più a questo che alla %: un ±0,13 s ti dice in modo diretto quanto giri stretto, e discrimina meglio tra due piloti che a prima vista hanno una % simile. **Obiettivo: ridurre il tuo ±DS.**

**Livelli di colore.** Il sistema ti classifica in base alla tua variazione:

- **Eccellente** — variazione sotto l'1,5%. Girare come un orologio.
- **Buona** — tra 1,5% e 2,5%. Solido.
- **Irregolare** — tra 2,5% e 4%. Fai salti, c'è tempo da guadagnare essendo più fine.
- **Erratica** — sopra il 4%. Molta instabilità; concentrati sul completare giri puliti prima che sull'attaccare.

**Toggle: Senza uscite / Con uscite.**

- **Senza uscite** — il tuo **ritmo puro**. Toglie uscite, pit e incidenti. Risponde: *quando giro bene, sono regolare?* Usalo per rifinire la tua guida.
- **Con uscite** — la **regolarità reale del tuo stint**. Include TUTTO: uscite, pit, traffico. Risponde: *davvero, così com'è, che ritmo ho consegnato?* Usalo per vedere l'impatto reale dei tuoi errori. Di solito esce peggio di "Senza uscite", e quella differenza è esattamente ciò che ti costano gli incidenti.

**Minimo di giri.** Servono almeno **3 giri validi** (che, togliendo il riscaldamento e il primo passaggio, sono circa 5 giri percorsi) perché il numero sia affidabile. Con meno vedrai un trattino (—) finché non accumuli percorso.

---

## 6. I grafici

Ogni grafico ha tre modalità. Cambiano a seconda di ciò che vuoi vedere.

**Tempo per giro.** Il classico: ogni punto è un giro e il suo tempo. Leggi la forma della tua gara. Scendi mentre scaldi? Cali alla fine per l'auto o per te? Un picco isolato (un'uscita) o una tendenza? Serve a vedere dove guadagni e dove perdi lungo lo stint.

**Sulla media.**

![img: 24-livestats-chart-media.png]

Qui ogni giro è disegnato come differenza rispetto alla tua media: sopra = giro più lento, sotto = più veloce. È la migliore vista della **consistenza**: quanto più piatta e attaccata allo zero è la tua linea, più sei regolare. I picchi verso l'alto sono i tuoi giri cattivi. Obiettivo visivo: appiattire la linea.

**Gap di giri.**

![img: 25-livestats-chart-gaplaps.png]

La tua distanza dal leader lungo il tempo (asse X = minuti della manche; asse Y = gap dal leader che scegli). Sale = perdi terreno; scende = recuperi. Serve a vedere IN QUALE MOMENTO della manche hai vinto o perso la gara, e se il distacco è stabile o ti sfugge.

---

## 7. Proiezione e gap

![img: 22-livestats-proyectada.png]

**Posizione proiettata vs posizione di manche.** Sono cose diverse ed entrambe contano:

- **Di manche** — dove sei nella manche che corri ora. Utile per il tuo duello diretto in pista.
- **Proiettata** — dove finirai la gara sommando tutte le manche. È la tua posizione REALE nella generale. La proiezione stima i tuoi giri totali dividendo il tempo totale di gara per la tua media. **Abbassare la tua media = migliore proiezione.**

Importante: la posizione proiettata è **la stessa ovunque** (scheda della diretta, Classifica Generale e pannello Lap). Se in un posto vedi P2, in tutti vedi P2. Non ci sono due verità.

**Tipi di gap.**

- **Gap dal leader** — a quanto stai dal primo.
- **Gap per giri** — la distanza espressa in giri (più intuitivo in resistenza: "sono a un giro").
- **Gap per minuto** — come evolve la distanza col tempo, per vedere se recuperi o ti stacchi.

Quando due piloti hanno gli stessi giri, il pareggio si decide con la **virgola**: la frazione di giro che avevi percorso proprio al calare della bandiera. Girare al limite fino alla fine può darti quella frazione in più che ti fa salire di una posizione.

## 8. La vista Risultati (dopo la gara)

Quando la gara termina, **Risultati (“Resultados”)** è dove si analizza tutto con calma. Ha varie **schede**; ognuna risponde a una domanda diversa. In alto vedi sempre il **giro veloce della gara** (chi e su quale corsia).

### Comparativa (la griglia per corsia)

![img: st-comparativa.png]

È la tabella principale. Una riga per partecipante e, per **ogni corsia** su cui è passato, cinque dati impilati:
- **Veloce** — il tuo miglior giro su quella corsia. Il punto blu + **MIGLIORE** segna il giro veloce *di quella corsia* tra tutti.
- **Media** — il tuo ritmo medio su quella corsia.
- **Cost. senza** — la tua **consistenza** (senza uscite) su quella corsia, in %.
- **Uscite** — quante volte sei uscito lì (e, sotto, il tempo perso).
- **Pit-stop** — soste su quella corsia (con il n° di giro, p.es. *G355*).

Serve a vedere **su quali corsie rendi meglio o peggio**, non solo il tuo numero globale. Il rettangolo blu segna la tua **corsia di partenza**.

**Gare di passate / ripeti-corsia.** Se la stessa corsia si corre più volte, ogni corsia si **sdoppia per occorrenza** (`1/2`, `2/2`…), per confrontare la tua 1ª passata con la 2ª sullo stesso punto.

![img: st-ocurrencia.png]

### Progressione (giro per giro)

![img: st-progresion.png]

Ogni giro della gara, in ordine. Puoi **scegliere con chi confrontarti**, filtrare per **manche** o per **corsia**, e mostrare/nascondere **uscite** (punti rossi) e **pit-stop** (arancioni). Con il pulsante **Δ Delta vs media** ogni giro è disegnato come differenza rispetto alla tua media (miglior vista per giudicare la tua regolarità: quanto più piatta, meglio). Risponde: *sono sceso mentre scaldavo? sono calato alla fine? è stato un picco isolato o una tendenza?*

### Posizioni

![img: st-posiciones.png]

Una linea per partecipante; l'asse verticale è la **posizione** (P1 in alto). Se la tua linea sale, perdi posizioni; se scende, guadagni. Serve a vedere **in quale momento** della gara si è deciso il tuo risultato.

### Gap dal leader

![img: st-gap.png]

La tua distanza dal leader **lungo il tempo** (puoi restringere l'intervallo di manche). La linea che scende = ti avvicini; che sale = ti allontani. Risponde: *in quale manche mi sono staccato o ho recuperato?*

### Gap (griglia)

![img: st-gapgrid.png]

La stessa idea ma in **tabella**: righe = squadre, colonne = manche, e ogni cella i **giri di svantaggio** alla chiusura di quella manche (0 = leader). Il **bordo dorato** avvisa che c'è stato un **pit-stop** in quella manche. Puoi scegliere 2–4 squadre per vedere il gap **tra di loro** (non solo contro il leader).

### Statistiche avanzate

![img: st-avanzadas.png]

L'analisi approfondita di un partecipante: **totale giri** (e puliti), **migliore**, **media** (con toggle *con/senza uscite*), **Δ consistenza**, **uscite · pit-stop** e **tempo perso**. Sotto, l'**evoluzione per corsia** (la tua media pista per pista, per vedere dove sei stato più veloce) e una scheda per corsia. Con **Confronta con (“Comparar con”)** scegli un rivale e si genera una tabella **faccia a faccia** con le differenze colorate (verde = meglio, rosso = peggio).

### Classifica Le Mans (squadre)

![img: st-lemans.png]

Nelle gare a squadre esiste inoltre la **classifica Le Mans**: la generale in grande, con **giri proiettati**, totale, **gap** dal leader, media, migliore e **P/Salire** (il ritmo che ti servirebbe per cacciare quello davanti). Ideale per le gare lunghe.

> **Icone e colori che vedrai:** punto blu + **MIGLIORE** = giro veloce di quella corsia · rettangolo blu = corsia di partenza · **bordo dorato** = c'è stato un pit-stop in quella manche · tendenza **▲/▼** = sei salito/sceso rispetto alla manche precedente.

## 9. Glossario

- **Consistenza** — la tua regolarità giro dopo giro. 100 meno la tua variazione relativa. Più alto = più costante.
- **±DS (deviazione standard) / CV** — il ±DS sono i secondi che oscilli da giro a giro (guarda questo numero). Il CV è quell'oscillazione in percentuale relativa al tuo ritmo; la % di consistenza è 100 − CV.
- **Media** — media semplice dei tuoi tempi di giro, senza quello di riscaldamento. Include uscite e pit. È quella che usa la proiezione.
- **Media pulita** — la tua media contando solo i giri normali (senza uscite). Si usa per il Δ e per rilevare gli incidenti, non per proiettare.
- **Warmup (giro di riscaldamento / passaggio parziale)** — il primo giro reale della manche, con artefatti del semaforo e del passaggio iniziale. Non conta per media, migliore né consistenza.
- **Sotto-minimo** — un tempo al di sotto del minimo di giro della gara. Passaggio fantasma impossibile; si scarta sempre.
- **Uscita (exit)** — sei uscito di pista. Conta per la media (è tempo reale perso) ma non per il tuo miglior giro.
- **Pit-stop** — sosta ai box. Conta come tempo, non come miglior giro.
- **Virgola** — la frazione di giro che avevi percorso al calare della bandiera. Decide il pareggio quando in due avete gli stessi giri.
- **Proiezione** — stima del tuo risultato finale sommando tutte le manche: tempo totale di gara diviso per la tua media.
- **Gap** — la tua distanza da un'altra auto (o dal leader), in tempo, in giri o per minuto.
- **PitWall Lap** — il sito web mobile della tua squadra (accesso tramite PIN): la tua posizione proiettata, le tue schede di ritmo e la voce che annuncia i giri. Solo nelle gare a squadre.
- **Occorrenza** — ogni volta che corri la stessa corsia nelle gare di passate/ripeti-corsia (`1/2`, `2/2`…); permette di confrontare una passata con l'altra.
- **P/Salire** — nella classifica Le Mans, il ritmo (media per giro) che ti servirebbe per raggiungere la squadra davanti.
- **Corsia di partenza** — la corsia da cui sei partito; nella griglia dei risultati è segnata con un riquadro blu.

---

**In una frase:** guarda la tua **posizione proiettata** per sapere dove finisci, abbassa la tua **media** per salire, e appiattisci la tua **consistenza** (riduci il ±DS) per smettere di regalare tempo giro dopo giro.
