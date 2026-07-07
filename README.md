# NBA Players & Teams Analysis with R Markdown

[Italiano](#italiano) · [English](#english)

---

## Italiano

## Panoramica

Questo repository contiene un progetto di analisi dati realizzato in **R Markdown** sul campionato NBA.  
Il progetto analizza statistiche relative a giocatori, squadre e partite, con particolare attenzione a punti segnati, minuti giocati, rendimento stagionale, rendimento in carriera e confronti tra giocatori e team.

L'obiettivo principale è esplorare i dati NBA attraverso operazioni di data wrangling e visualizzazioni grafiche, utilizzando il linguaggio **R** e librerie dedicate alla manipolazione e rappresentazione dei dati.

## Contenuto del progetto

Il file principale del progetto è:

```text
ProgettoRmarkdownGiacomoMariuzza.Rmd
```

Il documento R Markdown include:

- introduzione al tema dell'analisi NBA;
- caricamento e preparazione dei dataset;
- ricerca e selezione dei giocatori tramite ID;
- analisi dei punti segnati per stagione e carriera;
- confronto tra giocatori NBA;
- analisi del rapporto tra punti e minuti giocati;
- visualizzazioni per squadra e stagione;
- grafici animati tramite `gganimate`;
- bubble plot sulle statistiche di squadre e giocatori.

## Dataset utilizzati

Il progetto prevede la presenza dei seguenti file CSV nella directory principale della repository:

```text
players.csv
games_details.csv
games.csv
teams.csv
ranking.csv
```

Questi file vengono caricati nello script con `read_csv()` e sono necessari per eseguire correttamente l'analisi.

## Librerie richieste

Per eseguire il progetto sono necessari R e i seguenti pacchetti:

```r
install.packages(c(
  "readr",
  "dplyr",
  "ggplot2",
  "gganimate",
  "tidyr",
  "BasketballAnalyzeR"
))
```

## Come eseguire il progetto

1. Clonare la repository:

```bash
git clone <repository-url>
cd <repository-name>
```

2. Inserire nella cartella principale i dataset CSV richiesti:

```text
players.csv
games_details.csv
games.csv
teams.csv
ranking.csv
```

3. Aprire il file R Markdown in RStudio:

```text
ProgettoRmarkdownGiacomoMariuzza.Rmd
```

4. Eseguire il rendering del documento in HTML tramite il pulsante **Knit** di RStudio oppure da console R:

```r
rmarkdown::render("ProgettoRmarkdownGiacomoMariuzza.Rmd")
```

## Analisi incluse

### Analisi giocatori

Il progetto confronta diversi giocatori NBA utilizzando statistiche come:

- punti segnati;
- minuti giocati;
- stagione;
- squadra di appartenenza;
- andamento dei punti nel tempo.

Tra i giocatori analizzati sono presenti, tra gli altri:

- LeBron James;
- Stephen Curry;
- Jimmy Butler;
- Carmelo Anthony.

### Analisi squadre

Il progetto utilizza anche statistiche aggregate di squadra per analizzare:

- percentuale di tiri da 2 punti realizzati;
- percentuale di tiri da 3 punti realizzati;
- percentuale di tiri liberi realizzati;
- punti totali;
- assist in rapporto ai tentativi.

Le visualizzazioni vengono generate tramite bubble plot, utili per confrontare più variabili nello stesso grafico.

## Output

Il progetto produce un report HTML contenente tabelle, grafici statici e grafici animati.  
L'output permette di osservare e confrontare il rendimento di giocatori e squadre NBA in modo visivo e interattivo.

## Struttura consigliata della repository

```text
.
├── ProgettoRmarkdownGiacomoMariuzza.Rmd
├── players.csv
├── games_details.csv
├── games.csv
├── teams.csv
├── ranking.csv
└── README.md
```

## Note

I file CSV non sono inclusi automaticamente nel file R Markdown. Per riprodurre correttamente l'analisi è necessario inserirli nella stessa cartella del progetto oppure modificare i percorsi di lettura all'interno dello script.

---

## English

## Overview

This repository contains an **R Markdown** data analysis project focused on the NBA basketball league.  
The project analyzes player, team and game statistics, with a specific focus on points scored, minutes played, seasonal performance, career performance and comparisons between players and teams.

The main goal is to explore NBA data through data wrangling and data visualization using **R** and several packages for data manipulation, plotting and basketball analytics.

## Project contents

The main project file is:

```text
ProgettoRmarkdownGiacomoMariuzza.Rmd
```

The R Markdown document includes:

- an introduction to the NBA analysis topic;
- dataset loading and preparation;
- player search and selection through player IDs;
- points analysis by season and career;
- comparisons between NBA players;
- analysis of the relationship between points and minutes played;
- team and season visualizations;
- animated charts with `gganimate`;
- bubble plots for team and player statistics.

## Datasets

The project expects the following CSV files to be available in the root folder of the repository:

```text
players.csv
games_details.csv
games.csv
teams.csv
ranking.csv
```

These files are loaded in the script using `read_csv()` and are required to run the analysis correctly.

## Required packages

To run the project, R and the following packages are required:

```r
install.packages(c(
  "readr",
  "dplyr",
  "ggplot2",
  "gganimate",
  "tidyr",
  "BasketballAnalyzeR"
))
```

## How to run the project

1. Clone the repository:

```bash
git clone <repository-url>
cd <repository-name>
```

2. Place the required CSV datasets in the root folder:

```text
players.csv
games_details.csv
games.csv
teams.csv
ranking.csv
```

3. Open the R Markdown file in RStudio:

```text
ProgettoRmarkdownGiacomoMariuzza.Rmd
```

4. Render the document to HTML using the **Knit** button in RStudio or from the R console:

```r
rmarkdown::render("ProgettoRmarkdownGiacomoMariuzza.Rmd")
```

## Included analysis

### Player analysis

The project compares several NBA players using statistics such as:

- points scored;
- minutes played;
- season;
- team abbreviation;
- point trends over time.

Among the analyzed players are:

- LeBron James;
- Stephen Curry;
- Jimmy Butler;
- Carmelo Anthony.

### Team analysis

The project also uses aggregated team statistics to analyze:

- two-point field goal percentage;
- three-point field goal percentage;
- free throw percentage;
- total points;
- assists per shot attempt.

The visualizations are generated using bubble plots, which are useful for comparing multiple variables in a single chart.

## Output

The project generates an HTML report containing tables, static plots and animated plots.  
The output allows users to visually compare NBA players and teams across different performance metrics.

## Suggested repository structure

```text
.
├── ProgettoRmarkdownGiacomoMariuzza.Rmd
├── players.csv
├── games_details.csv
├── games.csv
├── teams.csv
├── ranking.csv
└── README.md
```

## Notes

The CSV files are not embedded in the R Markdown file. To reproduce the analysis correctly, place them in the same folder as the project file or update the file paths inside the script.
