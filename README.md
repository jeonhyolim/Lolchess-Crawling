# Lolchess-Crawling
Lolchess Crawling using python selenium

The "challenger_br_page1_20231025140659.csv" is the sample data, which can be crawlled using this python file.

### Assignment Purpose and Overview
In this project, I implemented a web crawler that retrieves primary crawling targets by accessing the Lolchess site (https://lolchess.gg/leaderboards?region=global&mode=ranked). Since Global contains complete data for several countries, you can exclude this part and import the Challenger and Grandmaster leaderboards for each of the 16 countries. Ranking, summoner (nickname), tier, LP, win rate, Top 4%, number of games, wins, and Top 4 on the leaderboard were crawled and listed from 1st to 100th on one page, so if additional pages exist, the data is also included. Everyone crawled. At this time, when the page changed, it was saved to a new CSV.

### Main functions (all main functions are listed in the crawler)
Website input function: Implemented to receive the user's desired tier and country as input values and save them for each page as CSV.
Classification through unique definitions when saving web pages: Since there were two things to distinguish in the crawler code, tier, and country, I implemented a saved CSV file by dividing it by tier. We decided that saving data by tier would be more convenient for later use of data.
Name of the output CSV file: Configured to contain the current date and time and included tier and country in the CSV name. At this time, the time was rounded to the second digit.
After completion, information on crawling results and time required: The time required and crawling are displayed so that users can know. In the case of the time required, it was measured immediately when crawling began and was measured once the crawling of one page was completed.
