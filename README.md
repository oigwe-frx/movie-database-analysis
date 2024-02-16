# Project: Movie Database Analysis

# PROJECT #1

### Columbia School of Engineering AI Boot Camp


### FANTASTIC 4
(Team 4): 
Jennifer Leone, 
James O’Brien, 
Osita Igwe, 
Giancarlo Ocasio, 
DoraMaria Abreu

### 02.14.24

Premise and vision is that Team 4 aka Fantastic 4 would be providing a 
Consultation for Movie Execs in the Industry



### An executive summary or overview of the project and project goals (5 points).

This data analysis and visualization project aims to investigate and identify critical attributes influencing the commercial success of movies. Leveraging data sourced from IMDb, the project aims to uncover patterns and correlations between various factors and a movie's box office performance. Through meticulous analysis and visualization techniques, the project seeks to provide actionable insights to stakeholders in the film industry, enabling them to make informed decisions to enhance the financial viability of their cinematic endeavors.

Our exhaustive analysis of a dataset encompassing over 10,000 films from 1903 to 2023 offers critical insights into the dynamics shaping box office performance. This rich dataset spans 60 countries, 54 languages, and 19 genres, providing an in-depth analysis of factors that drive movie popularity, revenue generation, and audience preferences. Equipped with these insights, executives can gain a deeper understanding of audience preferences and make well-informed decisions regarding future projects that are profitable and determining returns on investments (ROI)




### An overview of the data collection, cleanup, and exploration processes (5 points).

Dataset Source
The team sourced our data from Kaggle by exploring various datasets available on the website and reviewing how extensive the dataset was to enable us to answer some key questions. The team landed on a data set in the form of a CSV file that contained over 10k rows of data and 12 columns.
The dataset source is kaggle.com; the dataset creator cited their source as www.imdb.com. The creator also used a machine learning algorithm to fill in the missing values, so there may be some possible errors. This data represents a subset of the complete IMDb. The creator did not note the criteria for web scraping. The team assumes the data set is complete and accurate for this project.

### Data Dictionary
<ul>
<li>names: movie name</li>
<li>date_x: release date</li>
<li>score: user rating</li>
<li>genre: genre of the movie</li>
<li>overview: a summary of the movie's plot</li>
<li>crew: crew members</li>
<li>orig_title: the original title of the movie</li>
<li>status: release status</li>
<li>orig_lang: originally released in this language</li>
<li>budget_x: movie budget</li>
<li>revenue: revenue generated worldwide</li>
<li>country: release country</li>
</ul>

### Data Clean-up
The data was explored by importing a CSV file into a Juypter notebook. The team performed the following tasks:
<ul>
 <li>Datatype conversions:</li>
	<ul>
     <li>Within column "date_x," converted datatype from object to DateTime</li>
     <li>Within columns "budget_x" and "revenue," converted floats to integers.</li>
  </ul>
 <li>Removed null values within the columns "genre" and "crew". This action led to the removal of 126 rows of data, leaving us with 10052 rows, down from 10178.</li>
 <li>Reset the index.</li>
 <li>Renamed columns for readability.</li>
</ul>


As a team, the team talked about columns containing data arrays such as "Genre" and "Actors" and how to handle analysis for those. The team looked at data sources to understand if the array is rank-ordered. We found no documentation, so the team will assume the case. For analysis, the team will pull the 1st genre and the top 25 actors/crew members.


### Data Exploration
Our objective was to uncover trends and patterns within the film sector by structuring our analysis as follows:

### Categorical Single-variable Analysis
<ul>
 <li>Movie Ratings: Understanding the distribution </li>
 <li>Budget: Understanding the distribution </li>
 <li>Genre: Classifying movies by genre.</li>
 <li>Actor: Identifying crew member roles.</li>
 <li>Original Language: Language in which the movie was first released.</li>
 <li>Country: Country of the movie release.</li>
</ul>

### Numerical Single-variable Analysis
<ul>
 <li>Release Year: Year the movie was released.</li>
 <li>Budget: Financial investment in the movie.</li>
 <li>Revenue: Earnings from the movie.</li>
 <li>Cost: Production and other associated costs.</li>
</ul>

### Multi-variable Comparisons
<ul>
 <li>Revenue Analysis: Evaluating top earners by genre, country, actors, language, and budget.</li>
 <li>Ratings Analysis: Examining correlations between ratings and actors, revenue, budget, genre, country, and top actors.</li>
 <li>Financial Analysis: Investigating budget and revenue associations with top actors.</li>
</ul>


This approach facilitated a thorough exploration of the intricacies and influences within the movie industry.



### The approach that your group took in achieving the project goals (5 points).
<ul>
<li>Include any relevant code or demonstrations of the application or analysis.
<li>Discuss any unanticipated insights or problems that arose and how you resolved them.
      <ul>
        <li>Revenue and Ratings having a poor relationship.</li> 
        <li>Australia having almost twice as many movies released </li> 
        <li>Prolific actors and revenue does not necessarily correlate. </li>
      </ul>
</ul>


### The results/conclusions of the application or analysis:
<ul>
  <li>Include relevant images or examples to support your work.</li>
  <li>If the project goal was not achieved, discuss the issues and how you attempted to resolve them.</li>
</ul>


### Key Findings
<ul>
  <li>Budget and Revenue Correlation: A strong positive correlation exists between movie budgets and revenues, highlighting the importance of strategic budget allocation.</li>

  <li>Genre Popularity: Certain genres consistently engage audiences more, suggesting potential areas for investment.</li>

  <li>Impact of Language: English-language films dominate the dataset and generated the highest revenue, indicating a significant market preference.</li>

  <li>User Ratings: There's a slight negative correlation between budget and ratings, and a very weak positive relationship between revenue and ratings, suggesting that financial success is not solely determined by high budgets or high ratings.</li>
</ul>


### Conclusion:
The film industry's landscape is increasingly competitive and influenced by multiple factors, including genre preferences, budget allocations, and audience engagement. By adopting a data-driven approach, executives can make informed decisions that not only cater to current market demands but also set the stage for future success. Implementing the recommended strategies will enable stakeholders to maximize the potential of their cinematic projects, ensuring they resonate with audiences and achieve commercial success in the evolving film industry landscape.

Recommendation to business
Diversify Genre Selection: Studios should broaden their portfolio by investing in genres that consistently capture audience interest while also venturing into niche markets. This diversification strategy can attract a wider range of audience segments, potentially unlocking new revenue streams. By tapping into the unique appeal of both popular and less conventional genres, studios can cater to varied tastes and preferences, enhancing their market presence and profitability.

Strategic Budget Allocation: Our findings highlight the importance of judicious budget management. While larger budgets are often correlated with higher revenues, significant returns can also be achieved through moderate investments if allocated wisely. Studios are encouraged to prioritize spending on elements that significantly enhance production value and audience appeal, such as compelling storytelling, high-quality production elements, and effective marketing campaigns, to maximize the return on investment.

Leverage User Ratings and Feedback: Actively engaging with audience feedback and user ratings can provide valuable insights for aligning future projects with viewer preferences. This approach emphasizes the importance of quality over mere budget size in boosting film ratings and success. Studios should incorporate this feedback into their project development processes, using it as a guide to refine content, address audience expectations, and improve overall viewer satisfaction.

Embrace Data-Driven Decision Making: Utilizing analytics and data insights is crucial for staying ahead of industry trends and making informed decisions. By analyzing market data, audience behavior, and performance metrics, studios can identify emerging trends, audience preferences, and successful content strategies. This data-driven approach enables more accurate forecasting and experimentation with innovative content and distribution strategies, positioning studios to lead rather than follow market shifts.

Enhance Audience Engagement: Developing targeted marketing strategies based on in-depth analysis of genre preferences, themes, and user ratings can significantly increase audience engagement. Studios should also focus on building a robust online presence to foster a sense of community and anticipation among viewers. By creating engaging content that resonates with target demographics and leveraging digital platforms for marketing, studios can enhance their connection with audiences, driving interest and attendance for new releases.

Implementing these recommendations will empower studio executives to navigate the complex landscape of the film industry effectively. By focusing on strategic genre diversification, smart budget allocation, audience feedback integration, data-driven decision-making, and enhanced audience engagement, studios can optimize their operations for increased revenue and sustained success in a competitive market.




### Additional questions that surfaced, what your group might research next 
if more time was available, or share a plan for future development (5 points).

### Link for project on GitHub
[Movie-database-analysis  – Github](https://github.com/oigwe-frx/movie-database-analysis)


### Further Analysis
<ul>
  <li>The COVID pandemic’s effect on production, revenue, genre selection.</li> 

  <li>Longitudinal Analysis of Genre Trends: Investigating the evolution of genre popularity and profitability over time can provide studios with actionable insights into shifting cultural trends and technological advancements, enabling them to stay ahead of market dynamics.</li>

  <li>Assessing the Digital Landscape's Impact: Analyzing the influence of streaming platforms and social media on movie success, especially in comparison between traditional theatrical releases and digital premieres, can offer studios strategic insights into optimizing content distribution in the digital age.</li>

  <li>Demographic-Driven Content Strategy: A deeper understanding of audience demographics can enable studios to tailor content and marketing strategies more effectively, enhancing viewer engagement and financial outcomes.</li>

  <li>Predictive Analytics for Box Office Success: Employing machine learning to analyze pre-release data can help predict box office performance, allowing studios to make informed decisions on marketing and distribution strategies to maximize revenue potential.</li>
</ul>
