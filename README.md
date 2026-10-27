# IMDb Top 1000 Movies: Exploratory Data Analysis

End-to-end exploratory data analysis (EDA) of the Top 1000 IMDb movies dataset in Python: data cleaning, feature creation, visualization and answers to 11 concrete questions about ratings, votes, gross earnings and release trends.

## Dataset

- 1000 movies, 9 raw columns: movie name, year of release, watch time (runtime), IMDb rating, Metascore, gross, votes, description.
- Missing values: Metascore (155 missing) and Gross (162 missing).
- The CSV file is **not included** in this repository. Download `Top_1000_IMDb_movies_New_version.csv` from its original source (Kaggle) and place it in the same folder as the notebook.

## Analysis workflow

1. **Data understanding**: shape, `info`, `head`/`tail`, `describe`
2. **Data preparation**: dropping irrelevant columns, duplicates, renaming columns, feature creation
3. **Feature understanding**: distributions of individual variables
4. **Feature relationships**: correlations and relationships between variables
5. **Questions**, for example:
   - Top-rated movies with fewer than 100,000 votes (IMDb and Metascore)
   - Movies longer than 180 minutes with a rating above 8
   - Years with the highest total gross, most releases and best average rating
   - How average gross changed before and after COVID-19

## Key findings

- Most movies are rated between 7.0 and 8.5; very few exceed 9.0.
- Number of votes and gross earnings are strongly positively correlated; Metascore is a significant predictor of IMDb rating.
- Older films have higher average IMDb ratings than newer ones.
- Average gross is higher in the post-COVID-19 period than before it.

## Tech stack

Python, pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook.

## How to run

```bash
git clone https://github.com/<your-username>/imdb-top-1000-eda.git
cd imdb-top-1000-eda
pip install -r requirements.txt
# put Top_1000_IMDb_movies_New_version.csv next to the notebook
jupyter notebook imdb_top1000_eda.ipynb
```

## Author

Aleksa Rajković — [LinkedIn](https://www.linkedin.com/in/aleksa-rajkovi%C4%87-1b46652ba/)
