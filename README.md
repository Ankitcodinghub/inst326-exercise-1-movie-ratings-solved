# inst326-exercise-1-movie-ratings-solved
**TO GET THIS SOLUTION VISIT:** [INST326 Exercise 1-Movie-Ratings Solved](https://www.ankitcodinghub.com/product/inst326-exercise-1-movie-ratings-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;93564&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;2&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (2 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;INST326 Exercise 1-Movie-Ratings Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (2 votes)    </div>
    </div>
# Background

The goal of this exercise is to practice merging DataFrames and using split-apply-combine to analyze data. For this exercise, you will read in data about movies and ratings of those movies, and you will find the highest-rated movies in the dataset.

# About the data

The data are derived from the MovieLens 100k dataset, available at https://www.kaggle.com/prajitdatta/movielens-100k-dataset. Two files are provided: **movies.csv** and **ratings.csv** **movies.csv** contains information about a number of movies, and **ratings.csv** contains users’ ratings of these movies. There are several ratings for each movie.

# Template

A template script, **movies.py**, is provided. This script contains import statements, a **parse_args()** function to process command-line arguments, and an **if __name__ == “__main__()”:** statement to run the program.

# Instructions

**best_movies() function**

Write a function called best_movies() with two parameters: the path to a file of movie data (such as movies.csv) and the path to a file of rating data (such as ratings.csv).

Your function should read each CSV file into its own DataFrame. Do not hard-code the filenames into your function; use the parameters you defined instead. Merge the DataFrames using the “item id” column of the ratings DataFrame and the “movie id” column of the movie DataFrame. This should be an inner merge.

Group by the “movie title” column and find the average (mean) value of the “rating” column. This should give you a Series where the index labels are movie titles and the values are average ratings. Store this Series in a variable.

Return a sorted version of your Series of average ratings by appending .sort_values(ascending=False) to the name of your variable. For example, if you used the variable name average_ratings, your return statement could be

&gt; return average_ratings.sort_values(ascending=False)

This will sort the values in your Series from highest-rated movie to lowest-rated.

# Running your script

Your script should require two command-line arguments. Assuming your script is called movies.py and is in the same directory as movies.csv and ratings.csv, and assuming this is the working directory of your terminal, here’s how you could run your script (Windows users, replace “python3” with “python”):

&gt; python3 movies.py movies.csv ratings.csv

The top-most rated movie in this dataset is “Close Shave, A (1995)” with an average rating of 4.491071.
