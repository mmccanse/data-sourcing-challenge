# data-sourcing-challenge

Please find the code for this assignment here: [data-sourcing-challenge/blob/main/retrieve_movie_data.ipynb](https://github.com/mmccanse/data-sourcing-challenge/blob/main/retrieve_movie_data.ipynb). 

The csv output for this assignment can be found here: [data-sourcing-challenge/blob/main/Outputs/movie_data.csv](https://github.com/mmccanse/data-sourcing-challenge/blob/main/Outputs/movie_data.csv)

In completing this assignment, I referenced class activities, class slide decks, and utilized a Chat GPT assistance prompt provided by the instructor to serve as a teaching assistant.  

In Part 1, item 6 of the instructions, students are provided with code to use to create a lamda function to parse out the movie title. This is the code provided

lambda st: st[st.find("\u2018")+1:st.find("\u2019 Review")]

Please note that this function doesn't cleanly isolate all movie titles. There are about 50 titles with single quotes within the review title, that are not well isolated with this code.  I did not make adjustments as the instructions indicated we should use this method. However, in a real world scenario, I believe one could identify all the movie titles that don't match with the TMDB database, and use that list to go back to the NY Times dataframe and merge with those incorrect titles. That would isolate the incorrect titles in their own dataframe. Then the titles could be cleaned up further and merged back with the NY Times data, then crosss referenced with the TMDB data again.  I think the coding knowledge to do that likely involves concepts we have not yet learned, but I look forward to being able to problem solve in that way. 