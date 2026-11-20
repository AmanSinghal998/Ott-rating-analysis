OTT Rating Analysis – Core Python Project Documentation
Nov 20, 2026 · @Aman
Submitted by: Aman Singhal
Course / Year: B.Tech, 1st Year
College: ABES EC
1. Introduction
This project analyses the ratings of 100 popular movies and shows from six OTT streaming platforms using only core Python, with no NumPy, pandas or other external library. It loads the data, calculates statistics, ranks titles, searches by keyword and saves the data to a CSV file. All of this is done with lists, dictionaries, loops, functions such as sorted(), and the built-in csv module.
2. Objectives
• Practise core Python: lists, dictionaries, loops, f-strings and lambda.
• Calculate the average rating of all titles and of each platform.
• Count how many titles belong to each genre.
• Find the top-rated titles.
• Let the user search the data by keyword.
• Save the dataset to a CSV file using the built-in csv module.
3. Dataset
The dataset has 100 titles (93 shows and 7 movies), stored in the program as one text block with one title per line and fields separated by the | symbol.
Field
Meaning
Example
title
Name of the movie or show
Breaking Bad
type
S for show, M for movie (converted to Show or Movie)
S
platform
One-letter code, converted to the platform name
N (Netflix)
year
Release year
2008
genre
Main genre
Crime
rating
Approximate IMDb score out of 10
9.5
Platform codes: N = Netflix, P = Prime Video, H = Hotstar, M = HBO / Max, A = Apple TV+, S = SonyLIV.
Limitation: the ratings were compiled by hand from general knowledge of IMDb scores, so they are approximate. [Check a few ratings on IMDb before submission.]
4. Technologies used
Technology
Purpose
Python 3 (core)
The whole program, using only built-in features
csv module
Saving the dataset as ott_dataset.csv
Text editor or IDLE
Writing and running the code

5. Python concepts used
Concept
Where it is used
List of dictionaries
movies stores all 100 records
Dictionary
PLATFORMS code lookup, platform_ratings, genre_count
for loop
Loading data, grouping ratings, counting genres, search
setdefault()
Creates a list for a platform the first time it is seen
sum() and len()
Calculating averages
Dictionary comprehension
Building platform_avg
sorted() with lambda
Ranking platforms and the top 5 titles
f-strings
Formatted output and the text bar chart
input()
Reading the search keyword
csv.DictWriter
Saving records to a CSV file
6. Sample output
The first part of the output when the program runs:
Total titles  : 100
Average rating: 8.29

Average rating by platform
HBO / Max     8.74  ###########################
SonyLIV       8.46  ########################
Netflix       8.27  ######################
Prime Video    8.2  #####################
Apple TV+     8.11  #####################
Hotstar       8.05  ####################

Titles by genre
Crime        24
Drama        22
Sci-Fi       14
Comedy       11
...
7. Results
• The overall average rating is 8.29.
• HBO / Max has the highest platform average (8.74), followed by SonyLIV (8.46) and Netflix (8.27). Hotstar has the lowest (8.05).
• The highest-rated title is Breaking Bad (9.5).
• Crime (24 titles) and Drama (22 titles) are the most common genres.
These results describe this sample of 100 titles only. The platforms have different numbers of titles, so the averages should not be taken as a ranking of the platforms overall.
8. Conclusion
The project shows that useful data analysis is possible with core Python alone. Dictionaries group and count the data, loops process every record, sorted() ranks the titles, and the csv module saves the results. In this sample, HBO / Max has the highest average rating, and crime and drama are the most common genres.
