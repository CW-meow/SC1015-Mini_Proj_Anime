# SC1015-Mini_Proj_Anime

## About

This is a Mini-Project for SC1015 (Introduction to Data Science and Artificial Intelligence) which focuses on Anime.

<i>Notebook has not been segregated due to columns being unable to be loaded in correct format.</i>
- [Link to .ipynb](https://github.com/CW-meow/SC1015-Mini_Proj_Anime/blob/main/Project.ipynb)


## Contributors

- B128 Team 1
- Chen Wei - Data Cleaning, Explaratory Data Analysis, Data Visualization
- Aaron - Explaratory Data Analysis, Data Visualization
- Yon Nan - Explaratory Data Analysis, Data Visualization

## Problem Definition

- What makes an Anime good?
- Can we predict an Animes' Popularity (Which indicates how good an Anime is)?

## Datasets

- Jerry Kim. (2023). <i>Anime2023February</i> [Data set]. Kaggle. <https://doi.org/10.34740/KAGGLE/DSV/5040882>
- Michael Roberts. (2023). <i>Anime Character Traits Dataset</i> [Data set]. Kaggle. <https://www.kaggle.com/datasets/mjrone/anime-character-traits-dataset>

## Data Cleaning

- Most of the columns were imported as a Str instead of a List, and had to be converted to a List.
- Character and Anime names had to be standardised to read across datasets.

## Exploratory Analysis

- Identified the possible response variables: Score, Popularity.
- Removed all non-predictor / response columns.
- Looked at each columns correlation with the response variables.
- Most of the data was categorical thus it was was plotted in a boxplot to check how the categories varied against the response.
- Columns with lists had to be sorted into singular categories and then plotted.
- Characters column had to be matched against their respective ranks, then their correlation was plotted on a heatmap.
- Studio and Voice Actor columns had to be ranked based on their Animes, and their correlation was plotted on a heatmap.

## Models Used

1. Linear Regression
2. Random Forest Regressor 
3. Extreme Gradient Boosting

## Conclusion

- The predictors of "Themes", "Studio Rank (sorted by Popularity)", "Voice Actor Rank (sorted by Popularity)", "Age Rating", "Main Avg" (Main Character Average Rank), "Char Avg" (The Average Character Rank) has the highest correlation with the response variable Popularity.
- All the models had about a 0.6 explained variance, and about a 2000 mean error which was about a 10% error (2000/24000 = 10%), meaning these models are all of moderate Precision and Accuracy.
- Both Extreme Gradient Boosting and Random Forest Regressor put Character Rank as a very important indicator of Popularity, which suggests that the Anime Characters play a very big role in determining how good an Anime is.
- The Linear Regression Model to predict Character Rank showed that character traits had very little correlation with the Characters Rank, indicating that it is not the character traits that makes the character popular/ good.
- These Models have allowed us to see that alot more goes into making a good Anime than quantifiable points, there was more nuances like the story that cannot be quantified that plays a big role.

## What did we learn from this project?

- Regex to clean strings.
- Extreme Gradient Boosting, Random Forest Regression, RandomSearchCV.
- Collaborating using Kaggle.

## References

- <https://www.animenewsnetwork.com/answerman/2017-05-31/.116809>
- <https://machinelearningmastery.com/extreme-gradient-boosting-ensemble-in-python>
- <https://www.datatechnotes.com/2019/06/regression-example-with-xgbregressor-in.html>
- <https://www.analyticsvidhya.com/blog/2021/06/understanding-random-forest/>
- <https://slidesgo.com/theme/cosplay-workshop#search-anime&position-13&results-40&rs=search>
