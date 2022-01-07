<!--## Peter Wu's Data Science and Software Engineer Portfolio-->

<!--### You're in the Main Branch-->

<!--Welcome! This is my data science and software engineering portfolio to showcase my demonstrated skills. I have hidden these projects from Google searches by putting them in a separate branch in this repository. If you are seeing this message, please switch to the [`hiddenfromrobots` branch](https://github.com/pwu97/ds-swe-portfolio/tree/hiddenfromrobots) to see my work.-->

## Peter Wu's Data Science and Software Engineer Portfolio

1. [Betpath - Machine Learning for Sports Betting](https://betpath.io)

Betpath is a sports betting startup building the next generation of predictive analytics in sports prediction from the ground up through machine learning and Bayesian statistics. For 13 sporting leagues (NBA, MLB, NFL, NHL, NCAAB, NCAAF, La Liga, English Premier League, Serie A, Ligue 1, MLS, Bundesliga, Primiera Liga), I have built sports-specific machine learning algorithms to predict the outcome of matches, accounting for factors such as team strength, home field advantage, and injuries.

Betpath has sold monthly sports betting picks for $49/month. I have implemented various A/B tests on different Instagram stories that advertise the picks to select the type of promotions that will engage and reach more Instagram accounts. Using different GIF's and including the Betpath logo were effective in garnering more Instagram engagements and leads.

Betpath models for moneylines and spreads have achieved a 1.67% ROI through 1500+ unit wagers and counting. Our totals models are weaker, but this was a great learning experience for me as I had discovered a bug within our totals models that I am working to patch. I also gained a deeper understanding of what it takes to constantly refine a sports prediction model and assess how good a model is doing during the season (current NBA season, for example) through log-loss. If the model is not outperforming Vegas without their built-in 2.7% margin, then I know that I have to look deeper into the games to understand why it is not winning (not factoring in lineups properly, data scraping error, etc.).

Betpath was built using Google Cloud Platform (GCP) and using Google's Datastore NoSQL database. I have experience querying the data using GQL (Google's SQL equivalent). The front-end was built using HTML/CSS, Chart.js to display plots, and Jinja2 for templating. The back-end uses Python and Flask. Stripe API was used as a payment processor. Firebase was used to authenticate users. The machine learning models were built in Python using scikit-learn, numpy, and matplotlib.

2. [DIRECT: A Two-Level System for Defensive Pass Interference Rooted in Repeatability, Enforceability, Clarity, and Transparency](https://operations.nfl.com/media/3667/big-data-bowl-cmu.pdf) 

For this project, we conducted an analysis of predicted catch probabilities to determine suitable rule proposal changes that would help improve the game. We analyzed about 6,000 catch plays from the sample of 91 games provided as a part of the Big Data Bowl. We built a multiple logistic regression model to help us predict catch probability statistics if we had altered the predictors we used, like the different pass lengths of each play. By filtering catch probability plays by the type of penalty called, we discovered various insights pertaining to how each penalty was being officiated, most notably the bimodal shape of the defensive pass interference (DPI) distributions. We hypothesized that this was because of differing standards for what a DPI entails. Through a detailed analysis of the data, we propose a novel “two-level” system for DPI which protects the officials on borderline calls:

* “Common Foul” penalty will be defined as a general PI call (holding receiver’s arms down, pushing, etc.) where the defender was playing the ball and results in a 10-yard penalty.
* “Flagrant Foul” penalty will be defined as a general PI call where the defender clearly was not playing the ball and results in a spot foul.
Click here to read the full paper.

Code: [https://github.com/pwu97/pass-interference](https://github.com/pwu97/pass-interference)

This project was coded using R.

3. [CMU Sustainability Initiative](https://cmusustainability.shinyapps.io/sdg-mapping/)

While working as a Sustainability Data Analytics Intern at CMU, I researched and applied data analytical tools to map CMU’s curriculum, research, and club activities to the United Nations 17 Sustainable Development Goals (SDGs). We used techniques such as tf-idf, tf-idf weighted Word2Vec, average Word2Vec, Word2Vec, PCA, and t-SNE to generate keywords for each of the 17 Sustainable Development Goals (SDGs). I then built the R package [SDGMapR](https://github.com/CMUSustainability/SDGmapR) to map text to the SDGs based on simple keyword appearance within text. The link above is the app I built that maps CMU's classes and department to the SDGs. Given SDG1 (No Poverty), the app can generate the most relevant CMU classes that target this SDG based on the keywords we had defined. 