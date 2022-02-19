# TMDB Movies Dataset - Data Exploration & Visualization

## Dataset

Dataset URL : https://www.kaggle.com/tmdb/tmdb-movie-metadata 
The Dataset contains 5000+ movie data containing data of major films 
costing over 100 million dollars to produce, which can still flop, this 
question is more important than ever to the industry. It is expected 
that after reading and analysing this particular dataset we would be 
able to answer some of the more important questions revolving around 
film industry. The dataset has 10866 rows and 21 columns.


## Summary of Findings

23.14 % of the movies made a loss, 39.12 % of the movies made no gain no loss, 
37.74 % of the movies made profit. Over the years there is a increase in profit 
in terms of numerical dollar value, but when thinking in terms of actual dollar 
value since Direct comparison of dollar value over the course of years is not very 
natural, since in 1960 one could buy a lot more than what he can buy in 2015. 
Considering this fact in the analysis we observed a negative slope in the line of 
trends.Maximum number of movies were made with genre 'Drama' where as Most popular 
genre among the viewers as Adventure. Now we also have observed that genres such as 
Western, Tv movie, Foreign has generates the most loss. Popularity plays a very 
important role for a movie to be successful and generate profit. The more the 
popularity is of a movie, it tends to generate more revenue as a linear relation 
it can generate more profit. Now since Adventure genre is already a popular genre,
movies in this genre tends to perform well in terms of revenue & profit.


## Key Insights for Presentation

For the presentation, I focused on all of the featured of interest and
the relevant findings. Features which draws interests, like vote_average, 
release_year, genres, popularity, budget, revenue, budget_adj, revenue_adj, 
runtime.
To support the analysis further, we engineered couple of more features
profit - a numerical feature which is revenue minus budget
if profit is positive it indicates a profit, if negative it indicates
loss and if 0 it indicates no gain no loss.
Using the above we also engineered feature profit_or_loss, which is a 
categorical feature. We also introduced profit_adj which is again 
revenue_adj - budget_adj.
We also worked upon genres, since the genre feature was clubbed together in
a string seperated by '|', we applied split and explode, for each feature to 
be seperated and create a new row.

We applied the necessary cleaning and transformation and most importantly 
plotted the data for further understanding.
I started by plotting number of movies in each genre, then moved with movies
made every year, then plotted how runtime is distributed.
Then moved on with understanding how average movie ratings are performing
over the years, Average profit per year, and popularity per genre.

We plotted many such barplots, lineplots, scatterplots and pieplots in
order to support the analysis and performed feature engineering as and when 
required.