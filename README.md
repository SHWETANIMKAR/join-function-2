# Pandas Join Function

Practice of join() function in Pandas.

## What is Join?
Do alag DataFrame ko index ke basis pe jodna.

## Code

First Table - Movies
import pandas as pd
movies = pd.DataFrame({
    "Genre": ["Drama", "Action", "Comedy"]
}, index=["Dangal", "Jawan", "3 Idiots"])

Second Table - Ratings
ratings = pd.DataFrame({
    "Rating": [8.4, 7.0, 8.4]
}, index=["Dangal", "Jawan", "3 Idiots"])

## Join Types
LEFT JOIN - movies.join(ratings, how='left')
RIGHT JOIN - movies.join(ratings, how='right')
INNER JOIN - movies.join(ratings, how='inner')
OUTER JOIN - movies.join(ratings, how='outer')

## Final Output
           Genre  Rating
Dangal     Drama     8.4
Jawan     Action     7.0
3 Idiots  Comedy     8.4

## Learnings
right = right table ka index
inner = matching index dega
outer = dono table ke sare index dega

## Author
Shweta Nimkar
