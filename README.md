### Table of Contents

1. [Installation](#installation)
2. [File Descriptions](#files)
3. [Project Motivation](#motivation)
4. [CRISP-DM Process](#crispdm)
5. [Results](#results)
6. [Licensing, Authors, and Acknowledgements](#licensing)

## Installation <a name="installation"></a>

Should include python packages: 'numpy', 'pandas', 'matplotlib', 'sklearn', and 'seaborn'.  The code should run with no issues using Python versions 3.*.
The notebook comes with a function to install the functions for you, but you can install the libraries manually if you wish.

## File Descriptions <a name="files"></a>

There is one notebook available, `videogames.ipynb`, to showcase the work related to the above questions.  Question 1 is ineferential, questions 2 and 5 are predictive, and questions 3 and 4 are exploratory.  Markdown cells were used when trying to explain the findings and thought process of the analysis. Comments were also used throughout the code to make it easier to follow.

There is also `vgsales-12-4-2019.csv` which is the dataset used in the notebook.

## Project Motivation<a name="motivation"></a>

For this project, I was interested in using video games sales up to 2019 to better understand:

1. Do games with higher critic scores tend to have higher user scores as well?
2. Can we predict a game's user score based on its critic score?
3. What's the average global sales for each game genre, ESRB rating, and platform?
4. How has the trend in global sales changed over the years?
5. Can we guess a game's global sales based on its critic score, genre, and platform?

## CRISP-DM Process<a name="crispdm"></a>

1. Business Understanding
For this project, the objective is to understand different factors that influence video game sales and user scores, and use this understanding to predict future game sales and scores. From a business perspective, this could help game developers/publishers identify which features of a game (genre, platform, ESRB rating, critic score) are the most relevant to focus on for increasing sales and positive user reviews.

2. Data Understanding
The data used for this project was obtained from Kaggle, and contains information on video game sales up to 2019. The data contains information on the game's name, platform, genre, publisher, year of release, critic score, user score, ESRB rating, and global sales.  The data contains 55792 rows and 16 columns.

3. Data Preparation
The data was cleaned by dropping columns that were irrelevant, dropping rows with missing values or were filtered out by a criteria (ie. games with 0 sales), and creating dummy variables for categorical variables.  Some data was also split into training and testing sets for the predictive models.

4. Modeling
The only predictive models that were used were linear regression models used to answers questions 2 and 5.  The other questions were answered using descriptive statistics and visualizations.

5. Results
See `videogames.ipynb` for a techincal analysis or the link below for a more general overview of the results.

## Results<a name="results"></a>

The main findings of the code can be found at the post available [here](https://medium.com/@elijah_89308/3b3a3fa91f57).

## Licensing, Authors, Acknowledgements<a name="licensing"></a>

Credit goes to ABDULSHAHEED ALQUNBER who got the data by scraping vgchartz.com. You can view the dataset [here](https://www.kaggle.com/datasets/ashaheedq/video-games-sales-2019).

