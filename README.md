# WordCloud
## 🛈 Background Information
The NBA All-Star game (ASG) is a stage set for the biggest stars to team up or go head-to-head in a exhibition style game with high flying dunks, 30-ft 3 point shots, and some of the flashiest passes in the league. The overall temperature at these games is light, fresh, fun, but the gameplay is dynamic and exciting. The NBA regular season takes a weeklong hiatus and offers players a chance to step away from the 82-game grog of a regular season during this event. The combination of the best stars and a break from the regular season sets up for interesting and unique interviews from players. In particular, we will analyze Lebron James' interviews.

Lebron James will go down as one of the greatest basketball players to ever live. He has dominated his time in the NBA, so much that he has been named to the All-Star team for 19 consecutive seasons. Only failing to make the team his rookie season, when he entered the league directly from high school. His nineteen appearances have him tied with Kareem Abdul-Jabbar for the most in NBA history. 

## 🎯 Aim
We want to evaluate Lebron James ASG interviews by identifying common themes and topics. We also hope to gain some insights into trends or popular NBA news of each year around the time of the All-Star game.

We aim to continue the pattern set forth by the All-Star game and will execute our analysis in a fun and dynamic way. Let's explore these Lebron interviews with a word cloud!

## :mag_right: Interview Source
http://www.asapsports.com/show_player.php?id=13888

## :triangular_ruler: Skills and Methods
**Web Scraping** - We conducted web scraping using the bs4 library to extract data. Encoding detectors were employed to identify all the links on the page, and the BeautifulSoup package was utilized to extract the text from the selected links. By leveraging my understanding of website tags, I targeted specific text elements, such as 'b' and 'td' tags, considering the variations in formatting caused by the age of certain interviews, some of which date back over 15 years      

**Natural Language Processing (NLP)** - After aggregating the text from each interview into a single array, we proceeded to process our data. To accomplish this, we employed the natural language toolkit (NLTK) library. Specifically, we utilized the word_tokenize and stopwords packages to effectively eliminate punctuation and transition words. Moreover, we implemented a for loop and if statements to remove common words that held no significant value.   

**Data Visualization** - The first task of creating our visualization was choosing an impactful and clear image for our mask. Next, we ensured the image format was in-line with the requirements for a word cloud object (e.g. 255 for background). Finally, we implemented the wordcloud library to identify the colors in our mask (ImageColorGenerator) and create the image (WordCloud).

## :basketball: Word Cloud

<img src="Bball_wordcloud.png" width="30%"> 

## :closed_book: Conclusion
All- Star Game interviews were chosen in anticipation of different themes than those from the regular and post season. Surprisingly, we discovered the common theme aligns with typical Lebron James interviews. The words 'guy' and 'team' emerged as the most frequent terms. LeBron frequently refers to himself as a 'guy' or 'just a guy' to emphasize his humanity, while his 'team' first approach, a hallmark of his entire career, further solidifies his reputation as one of the greatest players in basketball history.

Some notable appearances are Kyrie and Kobe. Mention of both of them does not come as a surprise. Kyrie and Lebron both played for the Cleveland Cavaliers from 2015-2017 and won a championship together. As for Kobe, him and Lebron had some what of a rivalry - as Kobe is also considered one of the all-time greats. Additionally, Kobe's tragic passing in 2020 influences his mention as well. 

Lastly, we see 'great', 'time', and 'always' piecing together a common expression of enjoyment during ASG weekend and being able to take a break from regular season activities. Overall, this project contributed further evidence of the poise and mindset we typically see Lebron bring to an interview.

## :construction: Improvements
As a whole this project was successful and (at the time) a great introduction to text analysis. First, we must acknowledge the weakness of insights based on a word cloud object. I believe this project would be best to analyze NBA ASG interviews on a year to year basis- as opposed to an individual player. This should highlight those interesting and unique topics which we mentioned in our 'Aim'.
