#1)Le reti WPAN coprono il raggio di azione di una persona (10-15 metri) e sono utilizzate soprattutto nella domotica, ovvero nelle tecnologie casalinghe e/o di ufficio intente alla creazione di case e uffici smart.
La maggior parte delle reti WPAN utilizza le onde radio per la comunicazione, ad esempio la specifica bluethooth definisce una PAN wireless nella banda di frequenza ISM a 2.4 Ghz di frequenza e 2 MBps di velocità di trasferimento.
Bluethooth è adatta a piccoli dispositivi a bassa portata e consumo, e la sua specifica è nello standard IEEE 802.15 per WPAN.
I dispositivi SRD possono operare senza alcun tipo di restrizione a livello mondiale.
La connessione si instaura tra un dispositivo che assume il ruolo di Master e uno che assume il ruolo di Slave creando la cosiddetta rete Piconet.
Per comunicare utilizzando Bluethooth un dispositivo deve essere in possesso di apposito software e chip Bluethooth con unità trasmittente e ricevente.
Vi sono poi anche tipi di WPAN che utilizzano i raggi infrarossi come metodo di comunicazione.
irDA, un associazione non-profit di produttori elettronici, mette a disposizione le specifiche fisiche utilizzate dai dispositivi che utilizzano gli infrarossi per comunicare.
IrDA inoltre definisce una tecnologia di interconnessione tramite infrarossi di tipo bidirezionale point-to-point, tra dispositivi posizionati a visibilità reciproca in LOS con range ridotto.
Il problema delle WPAN  a onde radio è il fatto che le onde radio sono vulnerabili a interferenze, cosa che invece non succede con i segnali a infrarossi, che però possono essere interrotti in presenza di un ostacolo fra i due dispositivi che stanno comunicando.
2)
Il pairing, o accoppiamento, viene stabilito nel momento in cui in una connessione vi è un dispositivo Master e almeno un dispositivo Slave, in modo da creare una piconet.
Entrambi i dispositivi devono essere in possesso di uno specifico software attivato da una casella di controllo o un pulsante raffigurante il simbolo del Bluethooth.
Per effettuare la connessione, il dispositivo Slave ascolta il segnale trasmesso ogni 2,56 secondi dal Master, il pairing generalmente avviene entro 1,28 secondi ,verrà  mostrato il pin di autorizzazzione sul dispositivo Slave , una volta che un dispositivo è stato accoppiato a un dispositivo bluethooth questo viene inserito in una lista e ogni volta che, avendo il bluethooth attivo, il dispositivo entrerà nel campo di azione del bluethooth dell’altro dispositivo, verrà automaticamente rieffettuata la connessione.
Le piconet hanno un limite di 8 dispositivi connessi, un dispositivo può partecipare a più piconet come Slave ma solo ad una come master.
Fino a 10 piconrt formano la cosiddetta scatternet.

3)
In una WLAN, si definisce BSS(Basic Service Set) l’insieme degli access point e delle stazioni di sua copertura, costituendo una cella.
Nella cosiddetta modalità infrastruttura, il BSS-ID corrisponde all’indirizzo MAC dell’access point.
Gli access point funzionano sia da bridge tra la connessione wireless e quella cablata che da gateway per i WT, connettendoli alla connessione wireless.
È possibile anche collegare più Access point tra loro,in questo caso si crea una wireless Distribution system e gli Access point fungono come Bridge tra BSS e wireless Distribution system
Due o più BSS collegati tra loro attraverso un wireless Distribution system creano un ESS (extended service set ) in cui i possono essere inseriti secondo diversi criteri:
•	BSS parzialmente sovrapposti:permettono di fornire una copertura contigua
•	BSS fisicamente disgiunti
•	BSS co-locati: creano ridondanze migliorando la qualità della rete.

4)I WT nella WLAN sono i wireless terminal ovvero dispositivi mobili dotati di interfaccia PCMCIA o fissi con schede integrate PCI.
Lo standard 802.11 gestisce la mobilità delle stazioni seguendo 3 modalita di transizioni:
•	Transizioni statiche: le stazioni sono immbili e/ si spostano solamente nella stessa BSS.
•	Transizioni tra BSS: le stazioni si possono muovere soltanto tra BSS della stessa ESS
•	Transizioni tra ESS: le stazioni si possono muovere tra BSS di ESS differenti.
In quest'ultimo caso la connessione viene interrotta quando si tenta di passare da una WLAN a un'altra.appena entrato nel raggio di azione della nuova WLAN occorrerà accedere aprire una nuova connessione

5)
La configurazione di un Access point prevede una serie di parametri 
•	Sid ovvero l'identificatore del servizio serve ad associare un nome alla rete in modo che gli utenti possano identificarla. L'access point emette in broadcast un frame periodico detto beacon tramite il quale può essere identificata. Non vi è corrispondenza biunivoca tra l'access point è l'i d poiché l'access point può fornire connessione a reti diverse e dunque possedere più id. Allo stesso tempo più Access point possono fornire connessione alla stessa rete e dunque avere lo stesso id. 
•	Potenza la normativa della ETS impone di irradiare segnale con una EIRP non superiore a 100 milliwatt con banda a 2.4 GHz è un watt per banda a 5 GHz. La eirp e la potenza effettivamente emessa dall'antenna ovvero la somma della potenza dell'access point e del guadagno dell'antenna. 
•	Canali si può impostare l'access point su uno dei 13 canali questa operazione non è necessaria nel momento in cui abbiamo un solo Access point in una Wlan tuttavia se abbiamo più Access point oppure un Access point di un'altra rete è necessario applicare la regola del 5 ovvero ogni Access point dovrà essere 5 canali distanti da quello precedente. 
•	La crittografia lo standard di crittografia 802 11 e la WEP e deve essere impostata come livello minimo di sicurezza questo tipo di crittografia assegna a ogni utente una chiave che può essere di 10 cifre esadecimali o 26 esadecimali corrispondenti rispettivamente alla crittografia a 64 bit o 128 bit. 
•	Incapsulamento deve essere specificato, nel caso in cui un Access point funzioni anche da router, il protocollo per il trasferimento del frame gli standard sono PPoA e PPoE. 
•	NAT  e DHCP sempre nel caso in cui l'access point funzioni anche da router occorre attivare il nat e ildhcp
6)
I principali rischi per le reti wireless sono lo sniffing, lo spoofing, il denial of service e l'accesso non autorizzato.
lo spoofing consiste nella intercettazione passiva di dati che transitano su una rete wireless un hacker può infatti facilmente intercettare pacchetti di dati wireless non protetti usando appositi applicativi di sniffing che, oltre ad intercettare e memorizzare il traffico permette di effettuare analisi del traffico stesso lo sniffing può essere fatto sia a scopi leciti che illeciti in pratica lo sniffer intercetta e decodifica l’header in modo da ricostruire lo scambio dei dati fra le varie applicazioni

7)
La WEP crea un livello di sicurezza pari di quella della connessione cablata.
E la tecnica di crittografia e autenticazione di base per la specifica 802.11 implementata a livello Mac è supportata dalla maggior parte degli Access point quando questo metodo di crittografia è attivato viene crittografato il payload del frame da trasmettere attraverso largo l'algoritmo di cifratura afflusso a chiave asimmetrica RC quattro, RC quattro crea una sequenza pseudo casuale utilizzando una S- box di 256 byte e due indici da 8 bit ciascuno la chiave è lunga da 40 a 256 bit ed è usata per inizializzare l'x box.
Il WT ho l'access point effettuerà la decriptazione all'arrivo del frame, WEP utilizza una crittografia a chiave simmetrica dunque la chiave sarà la stessa sia per la cifratura e la decifratura. Rc quattro si divide in 5 passi
1.	L’IV a 24 bit generato casualmente viene trasmesso in chiaro nei primi byte del frame
2.	L’IV viene combinato con la chiave segreta dell'utente in modo da creare una sequenza di chiavi
3.	in base a questa rc quattro crea una sequenza di bit pseudo casuali della stessa lunghezza del payload
4.	il payloadviene composto dal testo in chiaro combinato con i bit di check calcolati con l’CRC 32
5.	viene effettuato lo XOR tra la keystream e il payload.
8)
TKIP Utilizza una chiave a 128 bit.
combina la chiave temporale con l'indirizzo Mac del WT e aggiunge una IV di altri 128 bit per formare la chiave di crittografia dei dati.
 la chiave viene rigenerata a ogni pacchetto oppure a ogni raffica di pacchetti inviati, si ha così una distribuzione dinamica delle chiavi
AES: molti ritengono questo metodo indecifrabile poiché utilizza l'algoritmo Rijandel il suo svantaggio è il costo infatti cambiare una rete in questa modalità risulta molto costoso poiché richiede di un store ovvero un hardware aggiuntivo
WPA è un aggiornamento di WEP e utilizza il TKIP fornire distribuzione dinamica delle chiavi
WPA2 personal utilizza una PSK
WPA 2 Enterprise utilizza un server di autenticazione

9)
WPA 2 Enterprise utilizza un server di autenticazione definito dallo standard IEE 802.1X che definisce un sistema nel quale possono essere utilizzate varie metodologie.
La metodologia più diffusa è quella che implementa EAP su entrambi i supporti della rete.
Con EAP al WT viene concesso solo lo scambio dei pacchetti EAP.
tale processo si avvale di un server di autenticazione RADIUS,che effettua il controllo delle credenziali, dopodiché fornisce l’autenticazione e una volta fornita viene concesso il traffico sulla rete.
il server usa un algoritmo di autenticazione specifico per verificare l'identità di un client tale algoritmo però non è specificato e bisogna scegliere tra
•	EAP-TLS (transport layer security)
•	EAP-TTLS (tunneled tran sport layer security)
•	LEAP (lightweight EAP)
il software che supporta la specifica e app si trova sul server in questione


10) il routing indiretto avviene in 5 passi principali
1.	Il il corrispondente host invia i pacchetti verso l'home agent del mobile host
2.	l'home agent riceve i pacchetti e li invia al Foreign agent
3.	il Foreign agent riceve i pacchettie li invia al mobile host
4.	il mobile host risponde al Foreign agent 
5.	il Foreign agent inoltra la risposta al corrispondenthost
nel caso in cui il mobile host si muovi in un'altra rete verranno effettuati i seguenti passaggi
1.	si registra a una nuova Foreign agent
2.	il nuovo Foreign agent conferma la registrazione all'home agent
3.	lomé agent aggiorna il care of address
4.	i pacchetti vengono inviati nuovamente all'home agent
11)
il routing diretto avviene in sei passaggi
1.	il corrispondente host prima di inoltrare i pacchetti chiede il caro rudess del mobile host all'home agent
2.	lomé agent risponde con l'ip del Foreign agent in cui si trova il mobile host
3.	il correspondenthost invia un pacchetto al Foreign agent
4.	il Foreign agent invia il pacchetto al mobile Lost
5.	il mobile host risponde al Foreign agent
6.	il Foreign agent inoltra la risposta al correspondent host

nel caso in cui il mobile host si sposti in un'altra foreign network, il foreign agent diventa anchor foreign agent , e il foreign agent della nuova rete deve comunicare a lui il care-of-address del mobile host.
I pacchetti verranno comunque inoltrati prima all’anchor foreign agent .

12)
L’obbiettivo della mobile host è quella dfi mantenere la connessione TCP tra due enti che comunicano.
Agent discovery: quando un mobile host si sposta in una foreign network, questo deve registrarsi presso il nuovo foreign agent in modo da capire che si trovi inj una rete differente , ciò avviene mediante l’invio di agent discovery message inviati dall’Home Agent o dal Foreign Agent.
La registrazione: una volta che il mobile host riceve il care-of address, questo deve essere associato al suo home address registrandolo presso il suo home agent.
