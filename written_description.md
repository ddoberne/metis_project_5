# Background
Fire Emblem is a Japanese video game series developed by Intelligent Systems, spanning 16 games over 30 years and selling over seven million copies. There are many polarizing opinions on Fire Emblem, but based on most of the discourse surrounding the game, one of the biggest pleasures of being a fan is complaining about the franchise's direction in nonspecific "recent years". The series is discontinuous, so characters often only exist in one or two games in the franchise. The "Fire Emblem" that supposedly might bind these games together, is not often of importance. By analyzing the scripts from each of the games, I hope to answer two questions: 1) What is Fire Emblem really about? 2) How have the topics of the games changed over time?

To answer those two questions, 1) It's about geo-political strife and familial tragedy, and 2) The topics have stayed consistent throughout the series. It's not about the Fire Emblem.
## Data
Scripts for 11 of the game's entries were scraped from [fireemblem.fandom.com](https://fireemblem.fandom.com/) using a custom [scraping tool](/scrape_tool.ipynb), totaling over 57,000 documents. Data was vectorized with CountVectorizer and TF-IDF excluding a custom list of stop words then run through topic modeling tools LSA, NMF, and LDA. It was found that the LDA and NMF models that used CV were most insightful. Games were put through this process individually, then as a group afterward. Stemming was attempted, but ultimately scrapped for the final result.
## Algorithms and Tools
- Selenium and BeautifulSoup for web scraping
- CountVectorizer and TF-IDF from scikit-learn for tokenization
- LSA, NMF, and LDA for topic modeling
- SnowballStemmer, but was not used for the final product
- pyLDAvis for visualization of LDA
- pandas and numpy
- Tableau and seaborn for visualization
- Markov Chain Text Generation
## Communication
* [Slide presentation](/what_is_fire_emblem_about_anyway.pdf)
* Future webpage using the Markov Chain Text Generation tool

