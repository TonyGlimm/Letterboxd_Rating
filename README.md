# Letterboxd_Rating WIP!


## 🎥 Introduction  🎥
Goal is to create a movie rating system which will recommend me the next movie if I dont have an idea on what to watch next (which happens quite often recently). Why dont I use the recommendations of the established streaming services? Because I rarely experienced that they recommend somethin which I actually like. Furthermore I would like to see how these type of systems work behind the curtain and get some practice in. I also have the option to decide on which data (which other user ratings) my system learns and can use the public user profiles of movie reviewers I like or just pull from a bigger database if I want.

I will pull the data myself using Letterboxd.com as a source, look over it and see if I have to gather more, explore it and clean it up and eventually build a recommendation model which will rate all the movies I didnt see but the other reviewers already rated. Afterwards I will sort that list and maybe give out the top 5. I'm not sure about the output yet and will see how I want to do it when I come closer to the end of this project. 

For this project I will try out google colab. 


## Table of Contents 📹

### Data Collectino via webscraping
- Scraped  data from the [letterboxd.com](https://letterboxd.com/) using Python's `BeautifulSoup` package.
- Cleaned up pulled data
- manipulate data into fitting format

### Modeling
- Decided on SVD(surprise) to create user recommendations
- used anti-test-user to create a user-x-title matrix for the movies a user didnt watch yet
- made predictions on the grading
- sorted predictions and gave out top 20 movies as recommendations for that user
