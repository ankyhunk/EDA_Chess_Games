# EDA Chess Games

Exploratory data analysis of **6.2 million chess games** played on [lichess.org](https://lichess.org), looking at player ratings, openings, game formats and how games end.

## Dataset

[Chess Games](https://www.kaggle.com/datasets/arevel/chess-games) on Kaggle, built from the [Lichess database](https://database.lichess.org/) (6,256,184 games, 15 columns). The notebook downloads it with `opendatasets`, which asks for your Kaggle username and API key.

## Questions answered

1. How does the Elo rating of White vary among players?
2. How does the Elo rating of Black vary among players?
3. Which are the most played openings?
4. Which colour is likely to win more games?
5. What is the victory status across different game formats?
6. How many openings lead to a win for White / a win for Black?
7. What are the top 10 most efficient openings for White and Black (highest win %)?
8. What are the top 10 winning openings?
9. How do White and Black Elo ratings vary across game formats?

## Key findings

- Modern Defense, Old Benoni Defense and Caro-Kann Defense are among the most played openings, and also produce the most wins for both colours.
- White wins more games than Black when games end normally; both are equally likely to win on time forfeit.
- White wins more than Black in every format, and draws are comparatively rare.
- In faster formats (less time on the clock), players' Elo ratings are higher.

## How to run

```bash
pip install numpy pandas matplotlib seaborn plotly wordcloud opendatasets
jupyter notebook EDA_of_Chess_Games.ipynb
```

## Future work

- Winning percentage of each opening for White and Black
- Why some openings are preferred over others
- Which openings are most common in each format
- How winning percentage translates into Elo gain
- Whether aiming for a time-forfeit win is a better strategy in fast formats

## Technologies

Python, Jupyter Notebook, pandas, NumPy, Matplotlib, seaborn, Plotly, WordCloud, opendatasets
