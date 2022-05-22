# Microsoft movie studio project
#### Author: Nick Kimani

## Business Problem
Microsoft wants to make a movie studio. But they don't know what kind of movies to make. I am tasked with analysing data to come up with which movies to produce and pressent my findings to the studio director in a way that is easy to understand.

Consider:
- What genre of movies are most popular?
- What genre of movies generate high returns?
- What length should the movies be made?
- How are non-english speakers catered for?
- What genre is popular but risky to produce?

## Data
Our datasets are:
- title_akas
- title_basics
- bom_gross
- title_ratings
- tmdb_movies
- movie_budgets

All of this data was sourced externally.
This data consists of movie titles, their IDs, genre classification, movie popularity, movie ratings, movie versions and last but not least, the financial information on movies.
I mainly use the movie genre classifications, financial information, their popularity and IDs. Most of the data used is of a numeric type. 

## Method
I combined `movie_budgets` with `bom_gross` so as to get a wider range of records for analysis. Then I went on to combine `title_ratings`, `title_akas`, `title_basics`, `tmdb_movies`,  to get movie versions, their ratings, their runtimes, number of votes and popularities. After this I combined the data made in step one with the one in step 2 so as to match financial information with all the other information. 

The analysis majorly involves the relations of popularity, vote count, version count, runtime and rating to movie budgets and grossing.

This was the most fitting method because as a business the goal is to make profits. Getting to know the how financial matters relate to the variables therein the market puts a business at a good position of knowing what moves to make and not to make for the sake of the business.

## Results
### Representation of movie productions grouped by genres
!(/home/nick/Documents/Project_1/Project1/Images/all_genre_magnitudes.jpg)

### Representation of top 1000 movie productions grouped by genres
!(/home/nick/Documents/Project_1/Project1/Images/first_1000_genre_magnitudes.jpg)

### Movie genres vs average production budget
!(/home/nick/Documents/Project_1/Project1/Images/genres_vs_budgets.jpg)

### Movie genres vs average grossing
!(/home/nick/Documents/Project_1/Project1/Images/genres_vs_grossing.jpg)

### Length of the movie vs popularity
!(/home/nick/Documents/Project_1/Project1/Images/runtime_vs_popularity.jpg)

### Version count vs popularity
!(/home/nick/Documents/Project_1/Project1/Images/popularity_vs_versions.jpg)

### Version count vs grossing
!(/home/nick/Documents/Project_1/Project1/Images/versions_vs_grossing.jpg)

### Version count vs production budget
!(/home/nick/Documents/Project_1/Project1/Images/versions_vs_budget.jpg)

### Movie rating vs grossing
!(/home/nick/Documents/Project_1/Project1/Images/rating_vs_grossing.jpg)



## Conclusions
This analysis leads to 4 recommendations as to what movies to produce and how to produce them:
- **Mainly produce adventure movies** Adventure movies are common in the top thousand grossing movies and also they record the highest grossing values in the market. However, they also take a largest budget to make. Its sales would also go well if it is also an action, animation and or drama movie as they are similarly popular and profitable.

- **Produce movies that range between 75 minutes to 120 minutes** Movies generally seem to be of this length. Moreover, making a long movie takes up more resources(budget) but doesn't translate to getting a higher gross thus making it pointless.

- **Make a healthy amount of translations for the movies produced** Making more verions of a movie makes it easy for people of different languages to watch it. By doing this the sales increase thereby increasing the gross obtained. However, it is important to note that in order to make more versions the budget has to increase.

- **Drama movies are risky to produce** The most produced movies are drama movies. Due to this the market is highly populated with drama movies which makes their sales to not be as good as other genres

**Disclaimer**
The data used here is of a relatively small scale compared to the wide market that consists of millions of data. This results in not so accurate findings as when the whole movie market is considered, the results may not be as visualized.

**Solution**
In future providing a larger set of data would improve the accuracy of the results thereby making the model more suitable to make concrete recommendations.
