Balteus @2024
Creato da: https://github.com/iu8lmc

Copyright: 2024 Martino Merola  

Contatto: iu8lmc@gmail.com
Licenza: https://creativecommons.org/licenses/by-nc-nd/4.0/



FACILE DA SCARICARE PER WINDOWS: 📥 Balteus  (WIN)

SCARICA: 📥 Balteus (Ramo Principale)

"Ricorda che questo software richiede conoscenze sia sui sistemi operativi che su PHP.

Ho testato questo programma su Slackware 15.0 e altri colleghi l'hanno testato su Fedora e Debian, oltre che su Windows.

Non garantisco la sua funzionalità se l'utente non ha conoscenze."


Descrizione
BALTEUS è uno strumento software sofisticato progettato per controllare programmi come JTDX, MSHV e WSJT-X in remoto o localmente. Offre un'operazione fluida su piattaforme Windows e Linux, supportando sia versioni a 32 bit che a 64 bit. Il software si basa sull'ultima versione di PHP per un rendimento ottimale.

Vantaggi dell'Uso di BALTEUS
BALTEUS offre molteplici vantaggi come BOT per il controllo di programmi come JTDX, MSHV e WSJT-X:

Controllo Remoto Senza Sforzo: BALTEUS consente agli utenti di controllare i programmi radio in remoto, eliminando la necessità di presenza fisica. Questo è particolarmente utile in scenari in cui sono necessari aggiustamenti e monitoraggio in tempo reale senza essere legati a una posizione specifica.

Maggiore Efficienza: Automatizzando compiti ripetitivi come le chiamate CQ e il riconoscimento dei messaggi, BALTEUS aumenta l'efficienza operativa. Può gestire le comunicazioni senza sosta, liberando gli operatori per concentrarsi su aspetti più strategici delle loro attività radio.

Integrazione Senza Problemi: BALTEUS si integra perfettamente con le piattaforme Windows e Linux, offrendo un'esperienza coerente e user-friendly su diversi sistemi operativi. Il supporto per varie versioni garantisce la compatibilità con una vasta gamma di configurazioni.

Adattabilità in Tempo Reale: La funzionalità in tempo reale di ULTRON consente modifiche dinamiche nelle preferenze del software senza la necessità di frequenti riavvii. Gli utenti possono passare facilmente tra programmi come JTDX, MSHV e WSJT-X, adattandosi alle esigenze comunicative in continua evoluzione.

Gestione Automatica del Registro di Log: La gestione dedicata del registro di log di BALTEUS assicura un tracciamento accurato dei QSO. La possibilità di utilizzare un registro personalizzato mantenendolo separato da altri software semplifica la tenuta dei registri e la verifica dei QSO.

Decisione Intelligente: La capacità di BALTEUS di identificare i messaggi, rispondere ai corrispondenti e gestire le liste d'attesa dimostra la sua intelligenza nel prendere decisioni informate durante la comunicazione. Snellisce il processo QSO, aumentando le possibilità di interazioni di successo.

Valutazione della Forza del Segnale: La considerazione della forza del segnale da parte di ULTRON aumenta le probabilità di successo dei QSO. Prendendo in considerazione segnali più deboli di -20dB, aiuta a dare priorità alle comunicazioni con migliori possibilità di successo.

Feedback Visivo: Per gli utenti di Raspberry Pi, le funzionalità di controllo dei LED e del tono udibile forniscono feedback visivo e audio, migliorando la consapevolezza dell'utente sulle operazioni in corso e sullo stato del processo di comunicazione.

In sintesi, impiegare BALTEUS come BOT per il controllo dei programmi radio offre una serie di vantaggi, che vanno dall'efficienza operativa e l'adattabilità alla decisione intelligente e al successo migliorato nelle comunicazioni. La sua integrazione senza problemi, le capacità in tempo reale e l'automazione intelligente fanno di BALTEUS un prezioso asset nel mondo delle comunicazioni radio amatoriali.

Prova BALTEUS oggi e migliora la tua esperienza radio amatoriale!

Requisiti
Prima di utilizzare BALTEUS, assicurati che i seguenti requisiti siano soddisfatti:

Ultima versione di PHP installata
Elenco dei moduli PHP richiesti (specificato alla fine dello script)
Software radio configurato correttamente per un rendimento ottimale
Raccomandazioni per un utilizzo ottimale:
Disabilitare il Tx watchdog
Configurare il server UDP per puntare alla posizione IP del programma
Abilitare la trasmissione dei dati del QSO registrati in formato ADIF
Non filtrare i dati UDP
Regolare le impostazioni del firewall per facilitare il flusso dei dati
📋 Dettagli
BALTEUS opera in tempo reale, consentendo cambi di software senza la necessità di riavvii. Rileva automaticamente il tuo call sign, l'indirizzo IP e le porte di comunicazione.
BALTEUS utilizza il proprio registro di log, ma puoi fornirne uno tuo posizionandolo nella cartella "wsjtx_log.adi" all'interno di ULTRON. Questo registro rimane separato dagli altri software.
Oltre a chiamare CQ, ULTRON riconosce messaggi come 73 / RRR o RR73 e determina se i corrispondenti sono occupati o non rispondono.
Se un corrispondente non risponde, sarà in lista d'attesa per 30 minuti prima di tentare nuovamente un QSO.
I segnali più deboli di -20dB sono considerati meno probabili di risultare in QSO di successo.
Il messaggio ADIF registrato viene inviato a ULTRON quando l'utente WSJT-X accetta la finestra di dialogo "Log QSO" cliccando sul pulsante "OK".
Terminale e Supporto ai Colori
BALTEUS richiede un terminale con supporto ai colori ASCII. Puoi usare il terminale Linux o il nuovo terminale di Windows 10/11, entrambi supportano i colori ASCII. Per il supporto ai colori su Windows, considera l'uso di ConEmu per un'esperienza migliorata.

Raspberry Pi
Per controllare i LED del Raspberry Pi, usa il comando sudo configurato senza richiesta di password. Il LED verde si accende per ogni decodifica e si spegne quando inattivo. Il LED rosso mostra un effetto simile a un battito cardiaco durante i QSO. La conduzione di un QSO emette un tono udibile se un altoparlante è collegato al jack del Pi.

Istruzioni per Eseguire BALTEUS
Per eseguire BALTEUS su Windows e Linux, hai diverse opzioni:

Esecuzione da Terminale:
Puoi eseguire BALTEUS direttamente tramite il terminale eseguendo il seguente comando: php robot.php

Script Batch (Windows) o Shell (Linux):
In alternativa, puoi creare uno script batch (.BAT) per Windows o uno script shell (.sh) per Linux con i comandi necessari per eseguire BALTEUS.

Task Scheduler:
Puoi anche utilizzare un task scheduler per eseguire ULTRON in background all'avvio del sistema.

Tieni presenti le seguenti considerazioni importanti:

BALTEUS richiede moduli specifici. Assicurati di avere installato i moduli richiesti. Consulta il file "robot.php" per l'elenco dei requisiti.
Effettua le modifiche necessarie alla configurazione "php.ini" per soddisfare i requisiti di BALTEUS.
Per riferimento, è fornita una configurazione "php.ini" di esempio nella cartella "extras".

Per qualsiasi ulteriore assistenza, consulta la documentazione o contatta il nostro team di supporto.

Grazie per aver scelto balteus!

