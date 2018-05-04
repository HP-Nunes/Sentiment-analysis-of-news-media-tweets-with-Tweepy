# TwitterPy
Sentiment Analysis using Twitter APIs

## Reflection about the assignment
I have been stubborn using Plotly instead of seaborn or matplotlib because I am foremost interested in creating something interactive and customizable. Hence this is an assigment I keep revisiting because I am struggling with implementing certain features, like a drop down menu to see my scatterpoints for a single news media organizations.

Also, as a disclaimer, I have included certain media organization in this exercise which I do not condone (hence media as opposed to "news" organizations), namely InfoWars and Breitbart News which I have no qualms denouncing as pernicious and perverse. I thought it would be interesting to compare media known to generate outrage and distrust with mainstream media, and the results were surprising although limited due to timespan being less than 24 hours (also VADER's methodology can be questionable in assigning sentiment scores). The mainstream tended to be as negative overall as far-right media, and rather surprisingly CNN had on average a near neutral sentiment analysis score.

The overall takeaway was that media will try to "clickbait" or generate as much buzz as possible within the confine of Twitter's limited character space, and entice users to click on their articles. Often that means focusing on news that is polarizing, and perhaps even sensationalized. There's also the aspect of news being inherently "bad", so it may depends on the news stories that were making the buzz at that time.

## Instructions:

In this assignment, you'll create a Python script to perform a sentiment analysis of the Twitter activity of various news oulets, and to present your findings visually.

Your final output should provide a visualized summary of the sentiments expressed in Tweets sent
out by the following news organizations: __BBC, CBS, CNN, Fox, and New York times__.

The first plot will be and/or feature the following:

* Be a scatter plot of sentiments of the last __100__ tweets sent out by each news organization, ranging from -1.0 to 1.0, where a score of 0 expresses a neutral sentiment, -1 the most negative sentiment possible, and +1 the most positive sentiment possible.
* Each plot point will reflect the _compound_ sentiment of a tweet.
* Sort each plot point by its relative timestamp.

The second plot will be a bar plot visualizing the _overall_ sentiments of the last 100 tweets from each organization. For this plot, you will again aggregate the compound sentiments analyzed by VADER.

The tools of the trade you will need for your task as a data analyst include the following: 
                tweepy, pandas, matplotlib, seaborn, textblob, and VADER.

Your final Jupyter notebook must:

* Pull last 100 tweets from each outlet.
* Perform a sentiment analysis with the compound, positive, neutral, and negative scoring for each tweet.
* Pull into a DataFrame the tweet's source acount, its text, its date, and its compound, positive, neutral, and negative sentiment scores.
* Export the data in the DataFrame into a CSV file.
* Save PNG images for each plot.

As final considerations:

* Use the Matplotlib and Seaborn libraries.
* Include a written description of three observable trends based on the data.
* Include proper labeling of your plots, including plot titles (with date of analysis) and axes labels.
* Include an exported markdown version of your Notebook called  `README.md` in your GitHub repository.

