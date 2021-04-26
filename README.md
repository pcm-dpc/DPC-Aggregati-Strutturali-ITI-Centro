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
| **Label**                       | ID Sequenziale nell’ambito del Comune. | Numero progressivo di identificazione dell’aggregato strutturale all’interno del Comune (utile per la rappresentazione in mappa). |692|
| **Comune**              | Nome ISTAT del Comune.| Denominazione unità amministrative territoriali comunali ISTAT. | Castiglione Cavarese |


## Collegamenti utili


## Normativa di riferimento


## Licenza
[CC-BY-4.0](https://creativecommons.org/licenses/by/4.0/deed.it) - [Visualizza licenza](https://github.com/pcm-dpc/DPC-Aggregati-Strutturali-ITI-Centro/blob/master/LICENSE)
