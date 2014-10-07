## Q1: There are generally 2 situations you'll start from when approaching a question of data: a) You designed and collected the data yourself OR b) You have to work with a data set you've been given access to.  What do you think makes these 2 starting points different?  How might it change what analysis you'll do?

If you're given data, the analysis methods are limited by the availability and schema of the data. Often you decide what is important based on what's available. When you're collecting data, you have to decide what data is necessary and what the most accurate way of collecting it is.
 
 (For the following set of questions we'll assume we're in situation A - you are going to design your own data collection)
 
 ## Q2: What factors go into deciding what data format to use?  Under what circumstances may you use different data types? (i.e., JSON, CSV, Key-Value Store, txt documents)
 [provide response here]
 
CSV and will be better if the data schema will not change over time. If it does, the unstructured nature of JSON and text files would be better if the data schema is going to change. Key-value storing is very fast and helpful for when data is expensive.

 ## Q3: Once you've chosen a format, you'll need to determine fields to capture and store.  A common approach for this involves determining what QUESTIONS you want to ask of your dataset.  For the following examples, please respond with which field(s) your may need to answer the questions needed:
 1. You're working for a company that tracks data on public transportation, you know you'll want to be able to ask "What percentage of a time is a bus/train late?"
 2. You're working for a school district, and you need to be able to help the principal answer the question "Which teachers are most successful at getting students interested in extra-curricular educational activities (e.g., Math Team, Quiz Bowl, Science Olypiad, Robot Building, etc)? 
 3. You're starting a social networking website that helps friends choose what to do on a Friday night, and you need to be able to answer the question, "Who made the suggestion that led to the final decision?"

 ### Answers:
-1. [Field(s) here]
-2. [Field(s) here]
-3. [Field(s) here]
1. Bus Identifier, routes, predicted arrival time, actual arrival time, 
2. Teacher name, Students, Activities per student
3. Authors, Friends, Suggestions, Final Decisions, Time
 
 ## Q4: Now you need to decide how you'll query your data.  What are the costs and benefits of the following options: 
 1. Store the data raw and load it into a Python or JavaScript Shell for analysis.  
 3. Build a webserver and write an API that dumps and queries that data in your database.
 
1. The data will not be stored for a long period of time and can only be analyzed in the moment. The data can be easily analyzed with complex frameworks and is optimal for displaying visualizations in real-time.
2. It is more costly than dumping it into a shell, but the data can be stored permanently across many servers without compromosing time. Complex analysis is difficult due to sharding.
3. It is costly to scale and takes time, but it is optimized for specific use case. Queries can be very complex and data is easy to keep track of. It is more expensive to maintain than NoSQL.
 
 ## Q5: You've now set up your database and have a website with 10,000 users, but have realized that you forgot a much needed field (say, an ID number for each user).  What do you do and how might different database designs have helped this situation?

NoSQL database designs would have made this process easier because new fields could just be added to each object. Otherwise, migrate the data to a new database that has the needed fields.
 
 ---------------
 
 (For this section, you may need to do some online research to answer the questions.)
 
 ## Q6: What is a Baysian Classifier?  What is it used for?
It is a feature/variable that is measured independently of other features. A probable identity/result of an instance composed of many factors can be determined by analyzing the combining the probabilities that each classifier is that identity independently.
 
 ## Q7: What is a simple graph you could generate to check for outliers in a dataset?
A box plot.
 
 ## Q8: What is a Null Hypothesis?
A statement that assumes initially that there is no relationship between two measures of data.
 
 ----------
 
 Answer the following questions using this scenario: You just got a HUGE dataset from Spotify where each entry contains these fields -> [username, song, # of times played, user rating, genre]
 
 ## Q9: How would you figure out the most popular song?
Query to find the songs associated with the most user names.
 
 ## Q10: How do you determine what genre a certain user likes the most?
Query to find the most frequent genre of the top-rated songs of the users.
 
 ## Q11: How do we match 2 users that we think may want to share playlists?
Find users who have rated the most songs with high ratings.
 
 ## Q12: What assumptions would you have before digging into Spotify data?  How would you test them?

 
 ----------
 
 Answer these last questions generally.
 
 ## Q12: What is a correlation and how do you find them in a data set?
It is the a measure of how much a change of one variable relates to a change in another variable.
 
 ## Q13: How can correlations help us tell a story with our data? 
Variables that are highly correlated can be used to find the relations between the variables.
 
 ## Q14: Let's think about data science as a way to tell a story about some data.  Why would I want to bring a second data set into my story?
A second data set can help confirm that the results of the initial set are accurate and provide additional insights.
 
 ## Q15: This one's just for fun.  How percent of the time do you expect to actually get the result you wanted?
5%

# Part 2: Analyzing Your Data

While there are many tools to do this analysis, we will use the JS library Gauss to accomplish this task since everyone should have used it by now.

## Screenshot of Data in Gauss
![screenshot of data in gauss](image.png?raw=true) 

## Most Frequent Value
[cut and paste command used and the output it produced]

## Range of data
[cut and paste command used and the output it produced]

## Biggest Change
[cut and paste command used and the related snippet from the output]

## Shape of data
[Describe]

## Threshold
[Value]

## Percentage above/below
[Command and output]

## Yes/No + Justification
[Answer and any images/snippets to justify]

# Part 3: Project Design Exercise

## Link to the device or devices you're interested in using
* [device1](URL to this device)
* [device2](URL to this device)

## What it would measure and how?
[Response]

## Where you'd put it in the lobby?
[Location]

## What problems could threaten the validity of your data?
[Response]

## How often to sample and when to make a data dump?
[Response]

## Resulting viz.
[Describe or link to example]

## Timing trigger
[Necessary? Why? and How?]

