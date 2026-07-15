# Billboard Hot 100 & Spotify Audio Analysis

## Live Demo

[View the interactive report](https://dataprog-music-trends.netlify.app/)

## Overview

This project explores how popular music has evolved over time by combining **Billboard Hot 100 chart data** with **Spotify audio features**. Using R and the tidyverse ecosystem, the analysis investigates trends in music characteristics, artist success, chart performance, and song moods from the 1950s through 2021.

The project was completed as an exploratory data analysis and visualization exercise using real-world datasets.

---

## Objectives

The project aims to answer several questions about popular music:

- How has the average sound of popular music changed across decades?
- Which artists have spent the most weeks on the Billboard Hot 100?
- Do #1 hits have different audio characteristics than other charting songs?
- Which artists have remained successful across multiple decades?
- Can songs be classified into mood categories using Spotify audio features?
- Do collaborations perform better than solo artists?

---

## Datasets

Two publicly available datasets were used:

### Billboard Hot 100

Contains weekly Billboard Hot 100 chart information, including:

- Song title
- Artist
- Chart date
- Peak rank
- Weeks on chart

Source:
https://www.kaggle.com/datasets/dhruvildave/billboard-the-hot-100-songs

### Spotify Tracks Dataset

Contains Spotify audio features such as:

- Danceability
- Energy
- Valence
- Tempo
- Loudness
- Acousticness

Source:
https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset

---

## Technologies Used

- **R**
- **Quarto**
- **tidyverse**
- **ggplot2**
- **readr**
- **lubridate**
- **stringr**
- **dplyr**
- **tidyr**
- **forcats**
- **knitr**

---

## Data Processing

The analysis involved:

- Importing both datasets
- Cleaning song and artist names
- Standardizing text for matching
- Joining Billboard and Spotify data
- Removing duplicate matches
- Creating additional variables such as:
  - decade
  - mood classification
  - collaboration indicator

---

## Analysis Performed

The project includes:

- Average audio features by decade
- Top 20 artists by total weeks on the Billboard Hot 100
- Comparison of #1 hits vs. non-#1 songs
- Most consistent artists across multiple decades
- Song mood classification using energy and valence
- Comparison of solo artists and collaborations

---

## Visualizations

The report includes several visualizations:

- Line chart of audio feature trends by decade
- Horizontal bar chart of top artists
- Pie chart showing mood distribution
- Boxplots comparing #1 hits and other songs
- Dot plot of artists with the longest chart longevity

---

## Key Findings

Some notable findings include:

- Popular music has become louder and more energetic over time.
- Acousticness has declined substantially since the 1950s.
- Songs have generally become less positive (lower valence).
- #1 hits are slightly more danceable but not necessarily more energetic.
- Rock and alternative artists dominate the list of longest-charting artists.
- Most Billboard songs fall into energetic mood categories.

---

## Repository Structure

```
MUSIC-TRENDS
│
├── data
│   ├── billboard
│   │   └── charts.csv
│   └── spotify
│       └── dataset.csv
│
├── Project.qmd
├── Project.html
├── README.md
```

---

## How to Run

1. Clone or download this repository.
2. Open `Project.qmd` in RStudio, Positron or VS Code.
3. Install the required R packages.
4. Render the Quarto document.

```r
install.packages(c(
  "tidyverse",
  "readr",
  "lubridate",
  "stringr",
  "ggplot2",
  "knitr"
))
```

5. Render the Quarto document:

```r
quarto render Project.qmd
```

---

## References

### Datasets

- Billboard Hot 100 Songs Dataset:
  https://www.kaggle.com/datasets/dhruvildave/billboard-the-hot-100-songs

- Spotify Tracks Dataset:
  https://www.kaggle.com/datasets/maharshipandya/-spotify-tracks-dataset

### Additional Reference

- Hyperbits – The Loudness War:
  https://hyperbits.com/ultimate-guide-to-the-loudness-war/

---

## Author

**Simona Cholakova**

June 2026
