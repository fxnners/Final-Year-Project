# Analysis of 3-Point Shot Decisions Using Game Theory

## Project Overview

This final year project is used to conduct research and analysis on decision making
within basketball, with emphasis on the decision making rational behind 3PT shot selection. 

The project makes use of game theoretic concepts such as Nash equilibrium to make theoretical 
predictions of the actions player may take and constructs payoff matrices to present offensive 
and defensive interactions and compares these equilibrium results with real world NBA data.

The research model is also extended to analyse the effect of a variety of different factors 
that have an impact on in game decision making such as game clock pressure, player fatigue and
different types of defensive matchups, the research and analysis conduct looks at answering
5 key research questions.

1. Do players’ 3-point shot-selection tendencies reflect mixed-strategy equilibrium 
   predictions when considering defensive contest levels?

2. How do game-clock dynamics influence the equilibrium between taking a 3-pointer 
   and driving and to what extent do real players adapt their choices accordingly?

3. Do players deliberately mix between contested and uncontested 3-point attempts 
   and alternative actions to keep defenders indifferent, as predicted by 
   mixed strategies?

4. How does fatigue affect the payoff structure of 3-point shot-selection, and do 
   players’ decisions shift away from equilibrium under physical strain?

5. Do defensive matchups and defensive adjustments (e.g., hard close-outs, sagging) 
   approximate best-response behaviour predicted by game theory, and how does offence respond?


---

## Prerequisites
- Python 3.7 or later
- Download required libraries **(Found in requirements.txt)** 

## File Structure
```
CS3IP_FinlaySmith.zip
├── FYP_Code/                       # Python notebooks
├── 2022-23 play-by-play.csv        # Dataset 
├── NBA_Stats_Defence.csv           # Dataset
├── requirements.txt                # Python dependencies
└── README.md                       # This file
```

## Setup Instructions

### Installation Steps and Running the Code

1. **Unzip file**

2. **Install required packages**
   ```
   pip install -r requirements.txt

   ```
3. **Open notebooks**
   - Open Notebooks in desired environment  

4. **Upload Dataset**
   - Upload the required dataset(s) for each notebook to google colab (or other desired environment) using file upload

5. **Run the code in each cell sequentially**

---

## How to access datasets 
The '2022-23 play-by-play.csv' can be found in the submission folder


The 'NBA_Stats_Defence.csv' is available on the repository and submission folder


## How and where to use the datasets

For the 'Empirical_Model.ipynb', 'Game_Clock_Ext.ipynb', 'Fatigue_Ext.ipynb' and 'Defensive_Matchup_Ext.ipynb' the '2022-23 play_by_play.csv'
must be uploaded to the notebook or placed in the same directory (depending on environment being used)

The 'Defensive_Matchup_Ext.ipynb' notebook also requires the 'NBA_Stats_Defence.csv' to be uploaded/placed in the same directory as well

---

## Guidance on how to use the Notebooks 

Each notebook is separated based on each stage of the research, all code cells in each notebook must be run sequentially (Top to Bottom).

The notebooks should be run in the following order, as some notebook outputs are dependent on outputs from notebooks in the earlier stages of research.

## Notebook structure 

1. **Baseline_Model.ipynb**
   - Defines initial theoretic offensive and defensive actions sets
   - Builds payoff matrix and solves for pure or mixed strategy equilibria to establish payoffs 

2. **Empirical_Model.ipynb**
   - Extracts 3PT shot and Drive frequencies from play-by-play data
   - Generate expected points for each defensive contest level
   - Compare theory equilibrium predictions with real world NBA data

3. **Game_Clock_Ext.ipynb**
   - Separates the game clock into different stages and recomputes payoff matrices and equilibria based on each stage
   - Compares equilibrium predictions for each stage against real player behaviour    

4. **Fatigue_Ext.ipynb**
   - Uses remaining time left in game to establish fatigue states
   - Recomputes payoff matrices and equilibria based on each fatigue state
   - Compares equilibrium predictions for each fatigue state against real player behaviour 

5. **Defensive_Matchup_Ext.ipynb**
   - Classifies defence into Below Average, Average and Above Average Defenders based on defensive stats
   - Recomputes payoff matrices and equilibria for each type of defence
   - Analyses how offence responds to defence quality

---
