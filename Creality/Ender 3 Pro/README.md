# Creality Ender 3 Pro
La Ender 3 Pro è una versione rivista della popolare Creality Ender 3 e prevede alcune migliorie rispetto al modello base. La più vistosa è il letto di stampa, che ora appoggia su un Asse Y composto da un estruso di alluminio 4040 al posto che 4020. L'alloggiamento dell'elettronica è stato ribaltato, in modo da far aspirare l'aria da sotto la stampante ed impedire ad eventuali filamenti in caduta dal piano di stampa di essere catturati dalla ventola.

Un'altra importante modifica è l'alimentatore, che passa da un alimentatore non brandizzato ad un modello di Meanwell, con una migliore protezione dalla sovratensione.

## Principali problematiche della stampante
### Mettere in squadra la stampante durante l'assemblaggio
Una dei primi passi per avere una stampante in grado di offrire una buona superficie dei pezzi stampati è di montarla correttamente durante l'assemblaggio. Oltre a verificare che tutte le parti assemblate sono state serrate correttamente e montate in modo che i componenti a scorrimento siano in grado di farlo senza giochi o frizioni eccessive, è anche necessario dare un occhio di riguardo al montaggio del portale dell'asse X sul corpo della stampante. Dopo aver avvitato le brugole che lo fissano al corpo, è bene aiutarsi con una squadra prima di serrarlo per assicurarsi che formi un angolo di 90 gradi rispetto al piano di stampa.

### Regolazione dei dadi eccentrici
Un'altra operazione - che andrà ripetuta nel tempo come parte della ordinaria manutenzione - è controllare la regolazione degli eccentrici. Tutte le parti della macchina che necessitano di scorrere sugli estrusi di alluminio quali il carrello dell'hotend, il carro dell'asse X rispetto ai due estrusi dell'asse Z ed il piano di stampa sull'asse Y sono dotate di tre ruote gommate, di cui una delle tre possiede un dado di regolazione al posto del distanziale. Tale dado presenta un foro eccentrico che permette di regolare la presa del componente verso l'estruso, allontanando o avvicinando le due rotelle opposte. La regolazione avviene regolando con una chiave fissa, solitamente già presente nel kit di assemblaggio della macchina. 

Quanto "stringere" il dado eccentrico di ogni componente? Non va serrato a fondo, ma abbastanza per far smettere alla parte di avere eccessivo gioco. Un buon metodo per regolarlo è tenere ferma la parte con una mano e con l'altra dare piccole regolazioni al dado. Quando le ruote smettono di slittare, ruotando libere, si è giusti ad una aderenza sufficiente. Dopo la regolazione è necessario muovere manualmente il componente lungo tutta la corsa per avvertire se oppone resistenza eccessiva, segnale che indicherebbe una stretta eccessiva dell'eccentrico. Per una guida visiva, date un occhio al video sotto incluso.

[![Regolazione Eccentrici](https://img.youtube.com/vi/GsEdU8ZtI6U/0.jpg)](https://youtu.be/GsEdU8ZtI6U "Regolazione Eccentrici")

### Layer non consistenti lungo l'asse Z
Un problema che affligge diversi utenti riguarda alcuni artefatti nella stampa lungo l'asse Z. Questi artefatti sono solitamente singoli layer più "schiacciati". Il problema è dovuto ad un orientamento spesso non corretto della madrevite dell'asse Z, che tende a divergere rispetto all'estruso di alluminio che compone l'asse X. Il primo passo, già sviluppato poch'anzi, è di verificare che l'asse Z sia in squadra rispetto al corpo della macchina. Successivamente si andrà a verificare se la madrevite è montata bene, andando a verificare se il giunto è montato correttamente e non introduce eccessivo errore sulla concentricità della rotazione della vite. 

L'ultimo step, a cui purtroppo si arriva a dover fare i conti, è il pezzo di plastica fornito da Creality per fissare il motore dell'asse Z all'estruso di alluminio. Purtroppo molto spesso il componente stock si rivela inadeguato per sorreggere il peso del motore e mantenerlo dritto, ma si tratta di un problema facilmente risolvibile. Su Internet si trovano infatti diversi design alternativi che permettono un montaggio più solido e dritto, di cui propongo alcuni design sicuramente funzionali:
* [Ender 3 / Pro / V2 Z axis motor mount by mknet](https://www.thingiverse.com/thing:4699747)
* [Ender 3 Z-Axis Damper Mount by AndiArbeit90](https://www.thingiverse.com/thing:3434253)


### Ecco perché i vari cuscinetti e stabilizzatori per la madrevite sono inutili
Su Thingverse o su Reddit troverete anche molti utenti che propongono di aggiungere un cuscinetto opposto al motore per "raddrizzare" la madrevite. Questo passaggio - salvo non vogliate aggiornare ad un sistema a doppia madrevite - è totalmente inutile e dannoso. La madrevite è utilzzata unicamente come trazione ed avere un lato libero permette di ridurre l'effettivo errore anche in caso di madreviti economiche ed eccessivamente storte, non si tratta di un risparmio da parte dei vari brand ma di una precisa scelta di design da parte del progetto RepRap. Maggiori informazioni, compresa una rappresentazione grafica del fenomeno, sono disponibili nel seguente video youtube.

[![Spiegazione sulla madrevite "libera"](https://img.youtube.com/vi/2Z7mZVvPlc8/0.jpg)](https://www.youtube.com/watch?v=2Z7mZVvPlc8&t=480s "Spiegazione sulla madrevite 'libera'")

### Comprato una Ender 3 Pro usata?
Prima di stampare felicemente con la propria Ender 3 comprata usata, è bene sapere che alcune stampanti appartenenti ai primi lotti venduti hanno avuto alcuni problemi di cui è meglio accertarsi di non essere affetti. Il primo problema riguarda le primissime Ender 3 e Ender 3 Pro immesse nel mercato, in cui erroneamente il firmware stock non aveva abilitato il "Thermal runeaway", una importante funzionalità software in grado di spegnere autonomamente la stampante in caso di letture errate dalle sonde termiche.

Per accertarsi di non aver acquistato una macchina senza le protezioni termiche attivate le vie sono due: O aggiornare il firmware della stampante all'ultima versione disponibile, o controllare se la stampane è in grado di fermarsi nel caso la sonda non invii correttamente la temperatura rilevata. In quest'ultimo caso è sufficiente scollegare momentaneamente il connettore della sonda dalla scheda madre, il cui ingresso è quello marcato come "ETEMP". 

Riguardo al connettore, date un occhio al seguente video:

[![Connettore XT60](https://img.youtube.com/vi/4yDp9frWkcg/0.jpg)](https://youtu.be/4yDp9frWkcg "Connettore XT60")

## Primi aggiornamenti
### Sostituire l'estrusore
Uno dei punti deboli della stampane è purtroppo l'estrusore (anche noto come Extruder) stock di plastica, destinato a rompersi nel giro di un paio di settimane d'uso intenso. Al momento le migliori alternative e che dovreste tenere a mente come una delle prime modifiche da effettuare alla stampante sono il Bondtech BMG Dual Drive (o relativi cloni cinesi) o un prodotto identico all'originale in plastica ma realizzato in alluminio. 

Il BMG ha un costo decisamente elevato, ma permette - specie se montato in Direct Drive - di stampare senza problemi i materiali flessibili ed ha un ottimo grip sul filamento, i cloni costano una frazione del costo dell'originale ma possono avere seri problemi di controllo della qualità delle unità. L'estrusore in alluminio è invece una alternativa economica anche se brandizzata da Creality ed ha prestazioni simili all'originale ma senza dare problemi di sottoetrusione che compaiono man mano che la leva di plastica dell'originale comincia a fratturarsi.

L'unica accortezza è quella di regolare in entrambi bene l'altezza della ruota dentata, poiché con il BMG darebbe una spinta disomogenea al filamento e rovinerebbe l'altra ruota di plastica, mentre con l'estrusore di alluminio tenderebbe a farla frizionare con il metallo.
 
### Sostituire le molle del piano di stampa
Uno dei problemi più noiosi di una Ender 3 Pro completamente stock è il livellamento del piano che tende a perdere la propria regolazione molto spesso, arrivando a dover essere controllata quasi ad ogni stampa. Il problema è dato dalle molle che Creality ha deciso di utilizzare, che risultano essere troppo poco rigide per tenere la regolazione del piano. Le alternative sono due:
* Sostituire le molle con una variante più rigida, spesso indicata nelle varie community come "le molle arancioni", per via del colore adottato per i pezzi di ricambio dei vari venditori. Il colore non è importante, ma lo è la maggiore rigidezza, solitamente data da un diametro maggiore delle spire e di un passo inferiore tra una spira e l'altra.
* Abbandonare le molle per degli appositi distanziali in silicone. Si tratta di un materiale morbido ma che se soggetto a pressione tende a mantenere una distanza omogenea nel tempo.

Una volta sostituite le molle stock con altra soluzione si notera una maggiore durata della regolazione del piano. Una soluzione a basso costo adottata da alcuni utenti per non dover comprare delle nuove molle consiste nello stampare degli appositi spessori, il cui modello [è disponibile su Thingverse](https://www.thingiverse.com/thing:3682481).

### Stampare una copertura per l'elettronica dello schermo
Può sembrare un vezzo estetico, ma coprire l'elettronica dello schermo - lasciata esposta da Creality per palese risparmio dei costi di produzione - ha anche dei vantaggi pratici. Il principale è ovviamente il non ferirsi alle dita nel caso si utilizzi con troppa foga il display, mentre l'altro motivo è proteggere lo schermo e la scheda ad esso collegato dai danni dell'elettrostatica o dai corti. Se per sbaglio si toccassero più pin con un cacciavite o altri utensili fatti di materiale conduttivo  addoperati vicino alla stampante, vi è il rischio di mettere in corto lo schermo e di conseguenza uccidere lo schermo e\o la scheda della stampante. Anche l'elettrostatica o la polvere potrebbero fare un danno simile, ma si tratta di casi più rari. Leggendo le varie comunità su Reddit, la maggior parte delle schede "morte" sono state causate da corti sullo schermo o da una pinza che ha messo in corto la cartuccia riscaldante durante un cambio di nozzle.

Di seguito alcuni design su Thingverse per racchiudere l'elettronica dello schermo in una custodia più consona:
* [Ender 3 Display LCD PCB Coverby Rocco81-92](https://www.thingiverse.com/thing:2858209)
* [ENDER 3 FACTORY SCREWS display rear cover by MakeChetti](https://www.thingiverse.com/thing:2987100)

### Sostituire il tubo bowden in PTFE con un Capricorn XS
La Ender 3 Pro, come tante altre stampanti in questa fascia di prezzo, usa un hotend la cui gola non è completamente metallica, ma permette al tubo in PTFE di arrivare a contatto con il nozzle. Si tratta di una soluzione piuttosto ottimale per quanto riguarda la trasmissione del calore, poiché il PTFE è un cattivo conduttore di calore, il filamento rimane freddo fino alla zona calda dell'hotend. Inoltre il basso attrito del PTFE - anche quello economico - lo rende una soluzione più scorrevole rispetto alle gole all-metal economiche, la cui finitura delle superfici interne è spesso troppo ruvida per avere uno scorrimento ottimale del filamento. 

Perché sostituire quindi il PTFE originale se è una soluzione che funziona? In effetti è un aggiornamento trascurabile se con la stampante vi limitate a stampare materiali che richiedono una temperatura relativamente bassa, come PLA e TPU, ma a temperature superiori ai 220 gradi - richiesti per materiali come PETG, ABS e ASA - il bowden vicino al nozzle comincerà a diventare soffice, deformandosi nel tempo e portando ad un inevitabile intasamento dell'hotend. Inoltre potrebbero svilupparsi gas tossici per i piccoli animali domestici.

I tubi Capricorn XS (e relativi cloni) possono invece superare con tranquillità i 260 gradi (fino ai 270 gradi) senza vedere la vita operativa utile ridursi drasticamente. Inoltre con ogni kit di tubi Capricorn vengono dati spesso in dotazione nuovi connettori pneumatici M6 e M8 con cui sostituire quelli stock forniti da Creality, notoriamente di pessima qualità e che tendono ad avere rotture nell'anello dentato interno che dovrebbe garantire la tenuta del connettore, facendo poi muovere il bowden dal gruppo estrusore - causando stringing - o facendo retrarre il bowden dall'hotend, causando gap che possono portare all'intasamento dell'hotend.

### Rendere più efficente il letto riscaldato con dell'isolamento termico
Molte stampanti 3d di generazione successiva alla Ender 3 Pro adottano questa miglioria già di fabbrica. Uno dei tempi di attesa più lunghi prima di iniziare una stampa è appunto il riscaldamento del piatto, poiché una lastra di circa 230mm di lato richiede diverso tempo per essere portata in temperatura anche utilizzando i 24v. 

Diversi prodotti economici e reperibili anche su Amazon, sono materiali dotati di cattiva conducibilità termica e che possono essere adoperati per fare una sorta di "cappotto termico" al letto della stampante. Questa modifica permetterà non solo di avviare prima le stampe, ma anche di risparmiare corrente elettrica poiché il letto ci metterrà più tempo a raffreddarsi, richiedendo meno inpulsi di corrente dalla scheda elettrica per mantenerlo a temperatura costante.

 Tra i prodotti disponibili ricordiamo:
 * Pannelli di cotone, schiuma e alluminia disponibili a circa 8-10 euro per i fogli da 230mm di lato
 * Sughero, più economico ma non consigliato perché potenzialmente infiammabile
 * Tappetini da saldatura ritagliati a misura. Si tratta ddi supporti economici usati nella salddatura a stagno per non rovinare i tavoli da lavoro e che sono isolanti termici e resistenti al calore.
 * Una soluzione molto "barbona" ma anche rischiosa è usare diversi strati di carbone, magari dell'imballaggio della stampante. Avendo aria al suo interno, il cartone è un ottimo isolante termico ma anche infiammabile. Considerando che la temperatura di innesco è di 200 gradi, si potrebbe quasi considerare "sicuro" per l'uso, ma sarebbe assai rischioso per una stampante utilizzata senza presidio o sistemi antincendio quali i rivelatori di fumo.
