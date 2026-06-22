# Dal sacro all'umano: la Storia dell'Arte letta in chiave digitale

## DOI
(https://doi.org/10.5281/zenodo.20795019)

## Descrizione
In questo progetto effettuiamo un'analisi dei dati (esplorativa e esplicativa) di un dataset storico-artistico, contenente opere d'arte realizzate tra il 1200 e il 2000. 

Il lavoro consiste nell’esplorazione, nella pulizia e nell’analisi del set di dati. Verranno esaminate alcune categorie presenti nel dataset, come i contenuti, le date di creazione, i generi e i movimenti artistici, analizzandole nel dettaglio per rispondere alle domande di ricerca individuate.

### Quali sono i risultati?
Al termine dell’indagine emerge come gran parte della produzione artistica sia caratterizzata da una forte presenza di opere a soggetto religioso: fino al 1600/1700 predominano infatti le raffigurazioni della Vergine Maria e di Gesù. 

Nel corso dell’Ottocento, invece, i soggetti religiosi diminuiscono lasciando spazio a rappresentazioni di figure umane generiche. Ciò dimostra che, pur non scomparendo del tutto, l’arte religiosa subisce un calo significativo rispetto ai secoli precedenti.

## Fonte dei dati

I dati in input sono costituiti da un file CSV di 523+ KB scaricato da una repository GitHub del corso di studi (https://raw.githubusercontent.com/dhdmch/2025-2026/refs/heads/main/data/vapod/data.csv).

| Variabile | Tipo |  Definizione | Esempio |
| :------- | :--- | :--------- | :------ |
| id       |  str | ID dell'opera |   http://www.wikidata.org/entity/Q428274 |
| titolo | str | Titolo dell'opera | Ritratto di Fedra Inghirami, detto Fedra |
| artisti | str | Artista dell'opera |  Raffaello Sanzio (maschio) |
| data_creazione |  int |  Anno di realizzazione | 1510 |
| generi | str | Genere pittorico | ritratto |
| luoghi |  str | Dove è stata l'opera | Galleria Palatina |
| collezioni | str |  Collezione di appartenenza | Galleria Palatina |
| contenuti | str | Elementi presenti | libro; carta; scrittura; strabismo; posizione seduta; scrivania; calamaio |
| movimenti | str | Periodo/corrente artistica |  Alto Rinascimento |
| soggetti | str | Soggetti dell'opera | Tommaso Inghirami |
| altezza | float | Altezza dell'opera | 91.0 |
| larghezza | float | Larghezza dell'opera | 61.0 |

I dati in output consistono in questo Jupyter Notebook lavorato su Google Colab, contenente testo e codice per l'analisi computazionale dei dati.


## Metodi e strumenti
Il progetto è stato sviluppato in un ambiente Google Colab utilizzando il linguaggio di programmazione Python. Lo strumento principale utilizzato per la manipolazione, l'analisi e la visualizzazione dei dati è la libreria Pandas.

Le operazioni includono:
*	Caricamento e ispezione dei dati (pd.read_csv, df.shape, df.info(), df.head(), df.tail(), df.describe());
*	Bonifica e normalizzazione dei dati (valori di misurazione sbagliati, id_number considerati come stringhe e non come Int64);
*	Analisi esplorativa e visualizzazioni tramite grafici a barre (plot.barh()), a linee (plot.line()), a torta (plot.pie()) e heatmap;
*	Analisi esplicativa focalizzata sulle diverse categorie proposte per rispondere alle domande di ricerca individuate.
*	Sono state utilizzate anche le librerie Matplotlib e Seaborn per la visualizzazione dei risultati.


## Responsabili
- Trazzi, Martina - https://orcid.org/0009-0008-8508-8588 - Researcher
- Lanotte, Federica - https://orcid.org/0009-0009-7253-2851 - Researcher

## Licenza
I dati di input e il codice di output (incluso in questo Notebook) sono rilasciati sotto licenza [CC0 1.0 Universal](https://creativecommons.org/publicdomain/zero/1.0/).
