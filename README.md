# DPC-Aggregati-Strutturali-ITI-Centro
## Repository degli aggregati strutturali italiani area ITI Centro



[![GitHub license](https://img.shields.io/badge/License-Creative%20Commons%20Attribution%204.0%20International-blue)](https://github.com/pcm-dpc/DPC-Aggregati-Strutturali-ITI-Centro/blob/master/LICENSE)
[![GitHub commit](https://img.shields.io/github/last-commit/pcm-dpc/DPC-Aggregati-Strutturali-ITC-NordOvest)](https://github.com/pcm-dpc/DPC-Aggregati-Strutturali-ITI-Centro/commits/master)

## Avvisi
Repository in fase di caricamento

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

## Sistema di riferimento della Carta Nazionale degli Aggregati strutturali

Il sistema di riferimento ufficiale per l’Italia è il sistema ETRF2000 (all’epoca in cui venne definito 2008.0) ed è un obbligo per le Pubbliche Amministrazioni adottarlo in base a quanto stabilito dal DM 10 novembre 2011 “Adozione del Sistema di riferimento geodetico nazionale” (https://www.gazzettaufficiale.it/eli/id/2012/02/27/12A01799/sg).

Per facilitare il corretto utilizzo dei sistemi di riferimento all’interno dei software GIS, l’Istituto Geografico Militare (IGM) ha pubblicato una apposita Nota (https://www.igmi.org/++theme++igm/pdf/nuova_nota_EPSG.pdf), nella quale – in particolare – viene consigliato l’uso dei sistemi proiettati dell’RDN2008. 
Nel caso della Carta Nazionale degli Aggregati Strutturali pertanto è stato adottato il sistema proiettato RDN2008 / Italy zone (E-N) (EPSG7794).

Per facilitare e standardizzare le procedure di conversione tra i sistemi di riferimenti, infine, l’IGM ha reso disponibili (https://www.igmi.org/++theme++igm/pdf/nuovi_PRJ.zip) i file .prj da associare ai file cartografici e il Comitato Permanente Sistemi Geografici (CPSG) del Centro Interregionale per i Sistemi Informatici Geografici e Statistici (CISIS) ha messo a disposizione di tutti gli utenti il Programma ConveRgo (Il software (realizzato dall’Ing. V. Cima e disponibile in https://www.cisis.it/?page_id=3214 ) consente di eseguire le trasformazioni di coordinate fra i vari sistemi di riferimento in cui sono espressi i dati geografici (ROMA40, ED50, ETRS89 nelle due realizzazioni ETRF89 e ETRF2000), considerando anche i rispettivi sistemi cartografici (Gauss-Boaga, UTM-ED50, UTM-ETRF89 e UTM-ETRF2000).).

Pertanto, utilizzando il software ConveRgo e adottando il ,prj corrispondente al sistema prima nominato RDN2008 / Italy zone (E-N), ovvero l’EPSG 7794, sono stati trasformati tutti i dati dei singoli file regionali dai loro sistemi di riferimento originali in quello di destinazione sopraindicato.

## Collegamenti utili

## Normativa di riferimento


## Licenza
[CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.it) - [Visualizza licenza](https://github.com/pcm-dpc/DPC-Aggregati-Strutturali-ITI-Centro/blob/master/LICENSE)
