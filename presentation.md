# Movie studio project insights
## Introduction
Welcome to the Movie Studio Insights Project! This project aims to provide a comprehensive analysis of current box office trends to guide the strategic decisions for our new movie studio. By leveraging data from multiple sources, we aim to identify the types of films that are currently performing best at the box office and translate these findings into actionable insights.

# Objectives
1.Identify the Highest Grossing Films: Determine which movies are leading in box office earnings.                                       2.Determine the Most Common Genres Among Top-Grossing Movies: Analyze the prevalent genres among the highest-grossing films.
3.Analyze the Correlation Between Box Office Performance and Movie Ratings: Investigate how movie ratings correlate with their box office success.
4.Identify the Most Successful Film Studios: Recognize the studios that produce the most successful films.
 
 # Data sources 
 The datasets used in this project are from various sources, including:

1.Box Office Mojo
2.IMDB
3.Rotten Tomatoes
4.TheMovieDB
5.The Numbers

# Datasets used
1.im.db.zip: Zipped SQLite database containing movie_basics and movie_ratings tables.
2.bom.movie_gross.csv.gz: Compressed CSV file with box office gross information.

# Project steps
## 1.data extraction and cleaning
1.SQLite Database:
-Extracted and cleaned data from movie_basics and movie_ratings tables.
-Dropped rows with null values in crucial columns like original_title and genres.
-Merged the tables on the movie_id column.
2.CSV File:
-Loaded and cleaned bom.movie_gross.csv.gz.
-Removed commas and converted the foreign_gross column to numeric.
-Filled missing values in foreign_gross with the median of the column.

## 2. data merging
Merged the cleaned data from the SQLite database with the cleaned CSV data using the title and year columns.

## 3.feature enineering
1.Created new columns like total_gross by summing domestic_gross and foreign_gross.
2.Condensed filters using parameters for a more user-friendly dashboard experience.

## 4.visualization and analysis
Generated key visualizations to meet project objectives:
  1.bar graphs to show:
    1.distribution of foreign gross revenue.
    2.total number of votes by genre.
  2.line graph to show:
    1.foreigh gross overtime.
  3.pie chart to show:
    1.genre distribution.
  4.scatter plots to show:
    1.the correlation between box office perfrmance and movie ratings  

 # Recommendations and Insights
  1. Focus on Proven Genres
Insight: The analysis reveals that certain genres consistently perform well at the box office.Recommendation: Prioritize production in high-performing genres such as Action, Adventure, and Animation. These genres have shown strong box office returns and audience appeal.
  2.Collaborate with Successful Studios
Insight: Certain film studios have a track record of producing high-grossing movies.recommendations: Establish partnerships or collaborations with successful studios identified in the analysis. This can help leverage their expertise and increase the likelihood of box office success.
Recommendation: Prioritize production in high-performing genres such as Action, Adventure, and Animation. These genres have shown strong box office returns and audience appeal.
  3.Leverage Strong Ratings
Insight: There is a positive correlation between movie ratings and box office performance.Recommendation: Focus on creating high-quality content that receives positive ratings from critics and audiences. Investing in strong scripts, talented directors, and high production values can help achieve this.
  4.Target International Markets
Insight: Foreign gross revenue is a significant contributor to total box office earnings.
Recommendation: Develop strategies to appeal to international audiences. This includes considering global market trends, incorporating diverse cultural elements, and investing in marketing campaigns tailored to different regions.

 # Conclusion
    This project provides a solid foundation for understanding the current trends in the movie industry. By leveraging the insights gained from this analysis, our new movie studio can make informed decisions to produce content that resonates with audiences and achieves box office success.