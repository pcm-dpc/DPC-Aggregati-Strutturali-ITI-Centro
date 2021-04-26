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


##Fonti dei dati

**LAZIO**
Disponibili nel Web: http://dati.lazio.it/catalog/it/dataset
Tipo: CTRN/DBT
Edizione: 2014
Scala: 5000

**MARCHE**
Disponibili nel Web: La Regione Marche non rende fruibili i propri dati come open data in formato shape https://www.regione.marche.it/Regione-Utile/Paesaggio-Territorio-Urbanistica-Genio-Civile/Cartografia-regionale/Repertorio/Carta-tecnica-numerica-110000/opendata . I dati in formato shape sono ceduti dietro richiesta per fini istituzionali con la clausola di non cederli a terzi.
Tipo: CTRN
Edizione: 1999/2000
Scala: 10000

**TOSCANA**
Disponibili nel Web: http://www502.regione.toscana.it/geoscopio/cartoteca.html
Tipo: DBT(DM2011)
Edizione: 1988/2013
Scala: 10000/2000

**UMBRIA**
Disponibili nel Web: La Regione Umbria dispone per il suo territorio di una “base” denominata Ecografico Catastale (vedi http://www.umbriageo.regione.umbria.it/pagine/ecografico-catastale ) che non è disponibile per il riutilizzo aggiornata al 2010. Esiste anche la Carta Tecnica Regionale vettoriale alla scala 1:5.000 scaricabile come Open Data (vedi http://www.umbriageo.regione.umbria.it/pagina/distribuzione-carta-tecnica-regionale-vettoriale-1-000 ) con aggiornamento dal 1985 al 2006. Infine, esiste anche il prodotto denominato “Distribuzione Carta Tecnica Regionale 10k vettoriale - esito grafico del Data Base GeoTopografico Tevere-Trasimeno (2013) (vedi http://www.umbriageo.regione.umbria.it/pagina/distribuzione-carta-tecnica-regionale-10k-esito-gr ). In accordo con la Regione Umbria il Dipartimento per la realizzazione degli aggregati strutturali il Dipartimento ha utilizzato la cartografia catastale ricevuta dall’Agenzia delle Entrate in occasione del terremoto nel Centro Italia del 2016.
Tipo: Catasto
Edizione: 2016
Scala: 2000

## Collegamenti utili

## Normativa di riferimento


## Licenza
[CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.it) - [Visualizza licenza](https://github.com/pcm-dpc/DPC-Aggregati-Strutturali-ITI-Centro/blob/master/LICENSE)
