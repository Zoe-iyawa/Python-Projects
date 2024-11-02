# Netflix Dataset Overview

This dataset offers an extensive look into Netflix's library of movies and TV shows, detailing essential information for each title, such as content type (movie or TV show), genres, release dates, IMDb ratings, duration, and production country. With over 5,000 entries, this dataset provides a rich resource to analyze trends.

The primary goal of this analysis is to identify the distribution of shows and movies across countries, release year as well as popularity of tv shows and movies.

## Data cleaning and Exploration
The initial steps involve checking for duplicate records and handling missing values. Any duplicates are removed with the drop_duplicates) method. The presence of null values is explored using isnull. Change datatype using astype.

## Key Analysis Tasks:
Year with the Most Releases
Movie and TV Show Distribution
Number of Movies and TV Shows Released in 2020.
Number of tv shows and movies from specific countries
Top 10 tv shows and movies

## Key Takeaway 
- 2019 to 2020 had the highest shows released: This period also coincides with a global shift towards streaming as a primary source of entertainment, especially during the COVID-19 pandemic, when traditional film and TV production faced interruptions. The surge in content aimed to meet the heightened demand from viewers staying home, with platforms aiming to provide a wide variety of new content.
- Movies Have a Higher Popularity Score Than TV Shows: Movies generally scored higher on IMDb. Movies are often a one-time commitment, making them easier for viewers to complete and rate. TV shows, on the other hand, can vary widely in quality across episodes and seasons, which might result in lower or more inconsistent IMDb scores. 
- Higher number of production for Movies: The data suggests a higher number of movies produced compared to TV shows. Movies often require less time to complete than multi-episode series, allowing production companies to produce and release more of them within a given time frame. 
- United States has higher number of Movies compared to TV Shows. However, the opposite can be seen to countries like the UK and South Korea: United States shows a preference for movies over TV shows, which may be due to the long-standing Hollywood tradition that has made American films globally popular. The U.S. produces a large volume of blockbuster films that are widely watched, and Netflix likely capitalizes on this by offering a vast library of American movies. On the other hand, UK and South Korea have higher TV show counts, reflecting a strong domestic market for episodic content. The UK, for example, has a rich tradition of serialized TV (e.g., BBC dramas), and South Korea’s globally popular K-drama format has proven highly successful on Netflix, drawing international viewers as well. This pattern may also reflect Netflix’s investment in localized content tailored to each region's cultural preferences, with South Korea and the UK showing consistent viewer interest in TV shows.
