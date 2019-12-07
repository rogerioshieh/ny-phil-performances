### DESCRIPTION

These Jupyter Notebooks allows anyone to visualize the data about performances in the history of NY Phil performances (1848-2018). The two main questions that I answer are:

1) Given the name of a composer, what is the percentage of his/her performances thoughout the history of NY Phil performances?

2) What is the percentage of living composers being performed per season?

### PURPOSE

Music scholars often examine such datasets manually, either by researching written sources or creating their own tables, which is inneficient. The scripts I provide allow for automatization of the process and enables scholars to more effectively formulate their hypothesis or find evidence for an existing argument.

For example: Wagner is one of the most performed composers of all times. However, the graph of his performances (below) shows that there was a sharp decline of his performances in between 1900-1920s. A music scholar can use this information to create/support an argument that proposes how WW1 affected how the composer was viewed in the US.  

![Wagner graph]( data/graphs/Wagner.png "Logo Title Text 1")

Graphs from other composers can be found on the <code>data/graphs/</code> folder.

### THE DATASET

The New York Philharmonic dataset is publicly available; I downloaded the .csv files from kaggle.com ([link](https://www.kaggle.com/nyphil/perf-history)).

Although the dataset was generally clean, I deleted rown containing intermission and condensed rows that referred to the same piece (i.e., a symphony is a single row instead of four rows with a movement each).

### DETERMINING IF COMPOSER IS ALIVE AT A GIVEN YEAR

Using Wikipedia API, I wrote a script that creates a .csv file of composers with their birth/death years. Using this file, I was able to calculate the percentage of living composers being features by season.

<em> Note: while the script found dates for most composers, some are not yet accounted for. However, performances by these composers only account for under 5% of the whole dataset, which makes the findings of the project statiscally relevant.</em>  

### FUTURE IDEAS FOR THE PROJECT

I am currently working on making the program more user friendly, where the program can automatically give statistics based on the user's input (such as composer's name or a year/time frame, for instance).  

### FINDINGS VIA ANIMATION/SONIFICATION

Thanks to the code provided by [Ben Holtzman](https://github.com/benholtzman/datamovies), I was able to create a sound animation that shows:

1) How classical music is dead (whereas in the 1850s 50% of all composers featured in NY Phil concerts were alive, living composers today account for only 10-15% of composers performed by the NY Phil).

2) How ubiquitous performances of just the top 3 composers (Beethoven, Wagner, Mozart) are.

Watch the animation [on YouTube](https://youtu.be/9nW32ANbVeo). The windy sound is based on the performances of living composers (vanishes with time) while the annoying beeps represent years when either Beethoven, Mozart, or Wagner were the most performed composers of the season. 

Date: May 2019 (updated Dec 2019)




