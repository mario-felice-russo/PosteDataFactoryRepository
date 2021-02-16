# Migrazione EDWH - Acquisizione iniziale

Obiettivo della migrazione sarà quello di trasferire tutti i dati presenti in Teradata on premise nel cloud impiegando il nuovo strumento di DataWareHouse SYNAPSE analytics, disponibile come strumento SaaS sulla piattaforma Azure.

Il processo di migrazione, data la quantità di dati presenti, prevede diverse fasi legate all'obiettivo di cambio piattaforma. Una prima fase di generazione memorizzazione delle strutture dati Teradata che, con l'ausilio di strumenti di migrazione specifici, creerà le stesse tabelle in Synapse, con le opportune variazioni di tipo e caratteristiche.

![image-20210205181616256](Image_Step_Infasamento_Iniziale/image-20210205181616256.png)


## 1. Processo di acquisizione

### 1.1 Configurazione del database di monitoraggio

<div style="width:200px;float:left;">Fase:</div><div style="width:auto;margin-left:200px;">Frammentazione</div>
<div style="width:200px;float:left;">Descrizione:</div><div style="width:auto;margin-left:200px;">Censimento delle tabelle da migrare.<br />Preparazione di un [json](AnaTabelle.json) da inserire in Configurazioni/AnaTabelle</div>
<div style="width:200px;float:left;">Parametri:</div><div style="width:auto;margin-left:200px;">... parametri</div>

<br />

<div style="width:200px;float:left;">Fase:</div><div style="width:auto;margin-left:200px;">Frammentazione</div>
<div style="width:200px;float:left;">Descrizione:</div><div style="width:auto;margin-left:200px;">Spostamento nello storage del fine AnaTabelle.json in  Configurazioni/AnaTabelle</div>
<div style="width:200px;float:left;">Parametri:</div><div style="width:auto;margin-left:200px;">... parametri</div>

<br />

<div style="width:200px;float:left;">Fase:</div><div style="width:auto;margin-left:200px;">Frammentazione</div>
<div style="width:200px;float:left;">Descrizione:</div><div style="width:auto;margin-left:200px;">Esecuzione della pipeline di creazione dei frammenti <b><i>01 Configurazione/pl_TD_MigrazioneEDWH_v01_001_InserimentoAnaTabelle</i></b></div>
<div style="width:200px;float:left;">Parametri:</div><div style="width:auto;margin-left:200px;">... parametri</div>

