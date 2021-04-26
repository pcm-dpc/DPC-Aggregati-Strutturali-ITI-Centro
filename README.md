# DPC-Aggregati-Strutturali-ITI-Centro
Repository degli aggregati strutturali italiani area ITI Centro

[![GitHub license](https://img.shields.io/badge/License-Creative%20Commons%20Attribution%204.0%20International-blue)](https://github.com/pcm-dpc/DPC-Aggregati-Strutturali-ITI-Centro/blob/master/LICENSE)
[![GitHub commit](https://img.shields.io/github/last-commit/pcm-dpc/DPC-Aggregati-Strutturali-ITC-NordOvest)](https://github.com/pcm-dpc/DPC-Aggregati-Strutturali-ITI-Centro/commits/master)

## Avvisi
Repository in fase di caricamento

## Sommario
[Struttura del Repository](#Struttura-del-repository)

[Aggiornamento dei dati](#Aggiornamento-dei-dati)

[Formato dei dati](#Formato-dei-dati)

[Fonti dei dati originali](#Fonti-dei-dati-originali)

[Licenza dei dati originali](#Licenza-dei-dati-originali)

[Sistemi di riferimento degli dati originali](#Sistemi-di-riferimento-dei-dati-originali)

[Sistema di riferimento degli Aggregati Strutturali](#Sistema-di-riferimento-degli-Aggregati-Strutturali)

[Procedura per la generazione degli Aggregati Strutturali](#Procedura-per-la-generazione-degli-Aggregati-Strutturali)

[Verifiche di qualità degli Aggregati Strutturali](#Verifiche-di-qualità-degli-Aggregati-Strutturali)

[Occupazione di memoria Regionale](#Occupazione-di-memoria-Regionale)

[Attori coinvolti](#Attori-coinvolti)

[Ulteriori approfondimenti](#Ulteriori-approfondimenti)

[Licenza](#Licenza)


## Struttura del repository
La serie di Dataset è organizzata in 5 repository corrispondenti alla classe 1 della Nomenclatura delle Unità territoriali statistiche (NUTS), che identifica la ripartizione del territorio dell'Unione europea a fini statistici. 
La classe 1 (NUTS-1) nel caso dell’Italia, ai fini statistici, rappresenta la divisione ufficiale delle macroregioni e consta di cinque gruppi: Nord-ovest, Nord-est, Centro, Sud e Isole. 
A ciascun gruppo è associato un proprio identificativo composto da una sequenza di tre lettere di cui le prime due corrispondono alla sigla dello Stato Italiano (IT).

<img src="https://github.com/pcm-dpc/DPC-Aggregati-Strutturali-ITI-Centro/blob/master/RipartizioniISTAT.PNG" />

```
DPC-Aggregati-Strutturali-ITI-Centro/
│
├── Centro/
│   ├── Lazio/
│   │   ├── Frosinone/
│   │   │   ├── shapefile comuni
│   │   ├── Latina/
│   │   │   ├── shapefile comuni
│   │   ├── Rieti/
│   │   │   ├── shapefile comuni
│   │   ├── Roma/
│   │   │   ├── shapefile comuni
│   │   ├── Viterbo/
│   │   │   ├── shapefile comuni
│   ├── Marche/
│   │   ├── Ancona/
│   │   │   ├── shapefile comuni
│   │   ├── AscoliPiceno/
│   │   │   ├── shapefile comuni
│   │   ├── Fermo/
│   │   │   ├── shapefile comuni
│   │   ├── Macerata/
│   │   │   ├── shapefile comuni
│   │   ├── PesaroUrbino/
│   │   │   ├── shapefile comuni
│   ├── Toscana/
│   │   ├── Arezzo/
│   │   │   ├── shapefile comuni
│   │   ├── Firenze/
│   │   │   ├── shapefile comuni
│   │   ├── Grosseto/
│   │   │   ├── shapefile comuni
│   │   ├── Livorno/
│   │   │   ├── shapefile comuni
│   │   ├── Lucca/
│   │   │   ├── shapefile comuni
│   │   ├── MassaCarrara/
│   │   │   ├── shapefile comuni
│   │   ├── Pisa/
│   │   │   ├── shapefile comuni
│   │   ├── Pistoia/
│   │   │   ├── shapefile comuni
│   │   ├── Prato/
│   │   │   ├── shapefile comuni
│   │   ├── Siena/
│   │   │   ├── shapefile comuni
│   ├── Umbria/
│   │   ├── Perugia/
│   │   │   ├── shapefile comuni
│   │   ├── Terni/
│   │   │   ├── shapefile comuni
```

## Aggiornamento dei dati
Non pianificato

## Formato dei dati
Il formato dei dati è shape. Ogni shape è formato da 4 file con le seguenti estensioni: .dbf, .prj, .shp, .shx.

La struttura dei file è la seguente:

| Nome campo                  | Descrizione                       | Formato                            | Esempio                            |
|-----------------------------|-----------------------------------|----------------------------------------|----------------------------------------|
| **IDAG**                        | Codice univoco dell’Aggregato Strutturale | 2 cifre: codice ISTAT Regione; 3 cifre: codice ISTAT Provincia; 3 cifre: codice ISTAT Comune; 10 cifre numero progressivo nel Comune; 2 cifre ulteriore identificativo. |07010013000000069200| 
| **Label**                       | ID Sequenziale nell’ambito del Comune. | Numero progressivo di identificazione dell’aggregato strutturale all’interno del Comune (utile per la rappresentazione in mappa). Questo ulteriore identificativo (in genere pari a 00, viene utilizzato in casi particolari, come quando è necessario ripartire un aggregato – inizialmente definito come un singolo poligono – in base alla realtà osservata dalla squadra durante il sopralluogo in due o più aggregati (Ad esempio, l’aggregato 08 036 022 0000000347 00 suddiviso in due genera i codici:08 036 022 0000000347 01 e 08 036 022 0000000347 02). |692|
| **Comune**              | Nome ISTAT del Comune.| Denominazione unità amministrative territoriali comunali ISTAT. | Castiglione Cavarese |


## Fonti dei dati originali

**LAZIO**

**Disponibili nel Web:** http://dati.lazio.it/catalog/it/dataset

**Tipo:** CTRN/DBT

**Edizione:** 2014

**Scala:** 5000

**MARCHE**

**Disponibili nel Web:** La Regione Marche non rende fruibili i propri dati come open data in formato shape https://www.regione.marche.it/Regione-Utile/Paesaggio-Territorio-Urbanistica-Genio-Civile/Cartografia-regionale/Repertorio/Carta-tecnica-numerica-110000/opendata . I dati in formato shape sono ceduti dietro richiesta per fini istituzionali con la clausola di non cederli a terzi.

**Tipo:** CTRN

**Edizione:** 1999/2000

**Scala:** 10000

**TOSCANA**

**Disponibili nel Web:** http://www502.regione.toscana.it/geoscopio/cartoteca.html

**Tipo:** DBT(DM2011)

**Edizione:** 1988/2013

**Scala:** 10000/2000

**UMBRIA**

**Disponibili nel Web:** La Regione Umbria dispone per il suo territorio di una “base” denominata Ecografico Catastale (vedi http://www.umbriageo.regione.umbria.it/pagine/ecografico-catastale ) che non è disponibile per il riutilizzo aggiornata al 2010. Esiste anche la Carta Tecnica Regionale vettoriale alla scala 1:5.000 scaricabile come Open Data (vedi http://www.umbriageo.regione.umbria.it/pagina/distribuzione-carta-tecnica-regionale-vettoriale-1-000 ) con aggiornamento dal 1985 al 2006. Infine, esiste anche il prodotto denominato “Distribuzione Carta Tecnica Regionale 10k vettoriale - esito grafico del Data Base GeoTopografico Tevere-Trasimeno (2013) (vedi http://www.umbriageo.regione.umbria.it/pagina/distribuzione-carta-tecnica-regionale-10k-esito-gr ). In accordo con la Regione Umbria il Dipartimento per la realizzazione degli aggregati strutturali il Dipartimento ha utilizzato la cartografia catastale ricevuta dall’Agenzia delle Entrate in occasione del terremoto nel Centro Italia del 2016.

**Tipo:** Catasto

**Edizione:** 2016

**Scala:** 2000

## Licenza dei dati originali

**LAZIO**

**Licenza dataset originale:** CC BY 3.0

**Autorizzazione specifica:** NO

**Attribuzione richiesta:** Regione Lazio

**MARCHE**

**Licenza dataset originale:** DGR n.783/2017

**Autorizzazione specifica:** Nota del 18 gennaio 2021 Regione Marche Giunta Regionale – Servizio Tutela, Gestione e Assetto del Territorio

**Attribuzione richiesta:** Regione Marche

**TOSCANA**

**Licenza dataset originale:** CC BY 4.0

**Autorizzazione specifica:** NO

**Attribuzione richiesta:** Regione Toscana

**UMBRIA**

**Licenza dataset originale:** Non presente

**Autorizzazione specifica:** Nota dell’1 marzo 2021 dell’Agenzia delle Entrate – Direzione Centrale Servizi Catastali, Cartografici e di Pubblicità Immobiliare

**Attribuzione richiesta:** Agenzia delle Entrate

## Sistemi di riferimento dei dati originali

**LAZIO**

**Sistema Riferimento:** ETRS_1989_UTM_Zone_33N

**EPSG:** 25833

**MARCHE**

**Sistema Riferimento:** RDN2008_Italy_zone

**EPSG:** 6875

**TOSCANA**

**Sistema Riferimento** Monte_Mario_Italy_1

**EPSG** 3003

**UMBRIA**

**Sistema Riferimento:** ETRS_1989_ETRS-UTM33

**EPSG:** 3045

## Sistema di riferimento degli Aggregati Strutturali

Il sistema di riferimento ufficiale per l’Italia è il sistema ETRF2000 (all’epoca in cui venne definito 2008.0) ed è un obbligo per le Pubbliche Amministrazioni adottarlo in base a quanto stabilito dal DM 10 novembre 2011 “Adozione del Sistema di riferimento geodetico nazionale” (https://www.gazzettaufficiale.it/eli/id/2012/02/27/12A01799/sg).

Per facilitare il corretto utilizzo dei sistemi di riferimento all’interno dei software GIS, l’Istituto Geografico Militare (IGM) ha pubblicato una apposita Nota (https://www.igmi.org/++theme++igm/pdf/nuova_nota_EPSG.pdf), nella quale – in particolare – viene consigliato l’uso dei sistemi proiettati dell’RDN2008. 
Nel caso della Carta Nazionale degli Aggregati Strutturali pertanto è stato adottato il sistema proiettato RDN2008 / Italy zone (E-N) (EPSG7794).

Per facilitare e standardizzare le procedure di conversione tra i sistemi di riferimenti, infine, l’IGM ha reso disponibili (https://www.igmi.org/++theme++igm/pdf/nuovi_PRJ.zip) i file .prj da associare ai file cartografici e il Comitato Permanente Sistemi Geografici (CPSG) del Centro Interregionale per i Sistemi Informatici Geografici e Statistici (CISIS) ha messo a disposizione di tutti gli utenti il Programma ConveRgo (Il software (realizzato dall’Ing. V. Cima e disponibile in https://www.cisis.it/?page_id=3214 ) consente di eseguire le trasformazioni di coordinate fra i vari sistemi di riferimento in cui sono espressi i dati geografici (ROMA40, ED50, ETRS89 nelle due realizzazioni ETRF89 e ETRF2000), considerando anche i rispettivi sistemi cartografici (Gauss-Boaga, UTM-ED50, UTM-ETRF89 e UTM-ETRF2000).).

Pertanto, utilizzando il software ConveRgo e adottando il ,prj corrispondente al sistema prima nominato RDN2008 / Italy zone (E-N), ovvero l’EPSG 7794, sono stati trasformati tutti i dati dei singoli file regionali dai loro sistemi di riferimento originali in quello di destinazione sopraindicato.

## Procedura per la generazione degli Aggregati Strutturali

**Fase 1:** _Estrazione e selezione dei dati_

Ove disponibili, vengono scaricate le feature delle classi del DBT “Edifici”, “Edifici minori” e “Manufatti industriali”. Nell’ambito delle tipologie previste dalle specifiche dei DBT (https://www.cisis.it/wp-content/uploads/2020/10/Specifiche_DBGT_v2.0-1.pdf) vengono selezione in particolare la maggior parte delle feature previste, con l’esclusione di una piccola parte di oggetti ritenuti non di interesse ai fini dei sopralluoghi di rilievo del danno ai fini della valutazione di agibilità. Questa riselezione riguarda in prevalenza la classe degli edifici minori e dei manufatti industriali (ad es. sono esclusi, tombe, edicole funerarie, garage, attrezzature turistiche, tendoni pressurizzati tra le tipologie di edifici minori e serbatoi interrati, pale eoliche, pannelli fotovoltaici e torri di raffreddamento tra le tipologie di manufatti industriali).

**Fase 2:** _Riferimento alle Unità amministrative territoriali ISTAT_

Secondo il Manuale per la compilazione della Scheda AeDES (http://www.protezionecivile.gov.it/documents/20182/0/2_LRManualeAedes_31_ottobre_GU_.pdf/8b4e4207-a767-4579-9971-d4c714a5fd4c - pagina 22) gli aggregati strutturali devono essere identificati principalmente con riferimento ai codici ISTAT delle Regioni, Province e Comuni. Pertanto nell’attribuzione del codice IDAG e nella selezione delle relative feature sono stati utilizzati i dati delle Unità Amministrative Territoriali ISTAT con aggiornamento 2021 (https://www.istat.it/it/archivio/222527). Nell’operazione di selezione sono state incluse in ciascun comune le feature che avessero il proprio centroide all’interno del relativo poligono ISTAT.

**Fase 3:** _Elaborazione dei dati a livello comunale_

L’elaborazione principale avviene per tutti i comuni all’interno di ciascuna provincia e utilizza alcuni tool di geoprocessing resi disponibili dal software ArcGIS di ESRI, che è stato appunto utilizzato per le elaborazioni.
Ciascun poligono viene inizialmente convertito in line derivate dai segmenti che costituiscono i contorni dei medesimi poligoni tenendo conto se ciascun segmento è condiviso o meno con un poligono confinante (vedi figura: Fonte ESRI Inc.).

<img src="https://github.com/pcm-dpc/DPC-Aggregati-Strutturali-ITI-Centro/blob/master/PolygonNeighbors.png" />

I segmenti che riguardano poligoni adiacenti vengono successivamente selezionati e i poligoni a cui essi appartengono sono uniti secondo il criterio di prevalenza del poligono con area maggiore e bordo comune più lungo.

**Fase 4:** _Memorizzazione dei risultati_

Ai nuovi poligoni generati vengono assegnati dei nuovi attributi secondo lo schema adottato (in particolare il codice IDAG) e vengono memorizzati in formato shapefile con un nome corrispondente al nome del comune ISTAT a cui si riferiscono. I nomi dei comuni per diventare nome di file vengono normalizzati rispetto ad alcune caratteristiche testuali che possono generare conflitti (ad es. spazi, accenti, apostrofi).
Tutti i dati generati durante le varie fasi dell’elaborazione sono conservati in appositi file in formato File Geodatabase ESRI. Anche i file originali sono conservati nei formati con i quali sono stati trasmessi al DPC.

**Fase 5:** _Elaborazione dei dati a livello regionale_

Per risolvere eventuali incongruenze generatesi ai bordi di comuni adiacenti, tutti i file comunali vengono successivamente uniti a livello provinciale e, infine, regionale e sottoposti alla medesima procedura illustrata in precedenza. In tal modo potranno essere ulteriormente accorpati – ove necessario – ulteriori poligoni adiacenti posti ai confini dei comuni e rimasti separati. L’aggregazione a livello regionale risulta infine propedeutica all’effettuazione dei controlli di qualità.

## Verifiche di qualità degli Aggregati Strutturali

**Fase 1:** _Verifica a livello comunale_
-	Controllo completezza dei dati
	
-	Controllo conformità allo schema dati
	
-	Verifica IDAG duplicati. Si evidenzia il caso della Regione Piemonte, che è l’unica regione per la quale non sono stati calcolati i nuovi valori di IDAG in quanto la regione li aveva precedentemente calcolati attribuendoli alla classe degli Edifici del BDTRE. Questo ha comportato, nella suddivisione nelle unità amministrative istata, anche delle discrepanze tra l comune ISTAT e il comune dal quale è stato ricavato il codice IDAG. In questa regione sono stati verificati anche gli UUID degli edifici, che in taluni casi sono risultati duplicati.

-	Verifica correttezza IDAG

**Fase 2:** _Verifica a livello regionale_

-	Effettuazione analisi di prossimità sui file regionali (viene mantenuto il campo IDAG)

-	Ricalcolo dei codici ProCom dei comuni adiacenti per controllo dei poligoni adiacenti ma appartenenti a comuni diversi

-	Join con della tabella generata dall’analisi di prossimità con il file regionale e analisi dei poligoni interessati

-	Verifica dei casi in cui è stata individuata sovrapposizione e successiva eliminazione di feature duplicate

-	Verifica dei casi con segmenti adiacenti ed eventuale unione con editing manuale

-	Verifica dei casi di vertici adiacenti. Si considerano solo i casi di 2 o più vertici coincidenti perché possono evidenziare adiacenze complesse. Questi casi, ove riscontrati, sono corretti da editing manuale

## Occupazione di memoria Regionale

**LAZIO**

**Size (Mb):** 916

**Codice Ripartizione NUTS-1:** 3

**Numero delle features:** 1662265

**MARCHE**

**Size (Mb):** 132

**Codice Ripartizione NUTS-1:** 3

**Numero delle features:** 426976

**TOSCANA**

**Size (Mb):** 427

**Codice Ripartizione NUTS-1:** 3

**Numero delle features:** 1211596

**UMBRIA**

**Size (Mb):** 142

**Codice Ripartizione NUTS-1:** 3

**Numero delle features:** 389943

## Attori coinvolti

Attività istituzionale realizzata in collaborazione tra il Servizio Sistemi Informativi e di comunicazione dell’Ufficio Risorse umane e strumentali e servizi generali di funzionamento (RUS) e i Servizi Attività di rilievo del danno e misure provvisionali e Supporto agli interventi strutturali e gestioni rientrate in ordinario, dell’Ufficio Attività per il superamento dell’emergenza e il supporto agli interventi strutturali (POST), entrambi appartenenti al Dipartimento della protezione civile della Presidenza del Consiglio dei Ministri.

**A cura di:**

Pierluigi Cara

**Revisione della documentazione a cura di:**

Maria Giovanna Martini, Cosmo Mercuri, Simona Papa, Filomena Papa, Angelo Giuseppe Pizza e Carmelo Vairo.

**Referenti regionali (per il tramite della “Commissione speciale Protezione civile” della Conferenza delle Regioni e delle Province autonome):**

_Abruzzo:_ Raffaella Molinari; _Basilicata:_ Alfredo Marino; _Calabria:_ Antonio Morabito; _Campania:_ Massimiliano Rauci; _Emilia-Romagna:_ Fiorella Galluccio; _Friuli Venezia Giulia:_ Fulvio Nodari; _Lazio:_ Adelaide Sericola; _Liguria:_ Mariano Strippoli; _Lombardia:_ Antonella Belloni; _Marche:_ Piepaolo Tiberi; _Molise:_ Diego Antonecchia; _Piemonte:_ Erika Ceriana Mayneri; _Puglia:_ Pasquale Cafaro; _Sardegna:_ Antonio Usai; _Sicilia:_ Antonio Torrisi; _Toscana:_ Massimo Baglione; _Umbria:_ Michele Bellezza; _Valle d’Aosta:_ Gianfranco Maccaferri; _Veneto:_ Umberto Trivelloni; _Provincia Autonoma di Bolzano:_ Diego Mantovani; _Provincia Autonoma di Trento:_ Mauro Zambotto.

**Referenti CISIS:**

Umberto Trivelloni, Gian Bartolomeo Siletto e Claudio Mazzi.

**Ringraziamenti:**

Flavio Celestino Ferrante e Maurizio Ambrosanio (Agenzia delle Entrate - Direzione Centrale Servizi Catastali, Cartografici e di Pubblicità Immobiliare); Mirco Sturari (Regione Marche); Laura Garbati (Consulente CISIS); Stefano Olivucci (Regione Emilia-Romagna); Stefano Campus (Regione Piemonte); Antonella Cuccurullo (Regione Lombardia); David Colmano (P.A. di Bolzano); Maria Basi (Regione Abruzzo).

## Ulteriori approfondimenti

[Relazione tecnica finale](https://github.com/pcm-dpc/DPC-Aggregati-Strutturali-ITI-Centro/blob/master/CartografiaNazionaleAggregatiStrutturali_Finale.pdf)

## Licenza
[CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.it) - [Visualizza licenza](https://github.com/pcm-dpc/DPC-Aggregati-Strutturali-ITI-Centro/blob/master/LICENSE)
