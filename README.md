<!--## Peter Wu's Data Science and Software Engineer Portfolio-->

<!--### You're in the Main Branch-->

<!--Welcome! This is my data science and software engineering portfolio to showcase my demonstrated skills. I have hidden these projects from Google searches by putting them in a separate branch in this repository. If you are seeing this message, please switch to the [`hiddenfromrobots` branch](https://github.com/pwu97/ds-swe-portfolio/tree/hiddenfromrobots) to see my work.-->

## Peter Wu's Data Science and Software Engineer Portfolio

1. [Betpath - Machine Learning for Sports Betting](https://betpath.io)

Betpath is a sports betting startup building the next generation of predictive analytics in sports prediction from the ground up through machine learning and Bayesian statistics. For 13 sporting leagues (NBA, MLB, NFL, NHL, NCAAB, NCAAF, La Liga, English Premier League, Serie A, Ligue 1, MLS, Bundesliga, Primiera Liga), I have built sports-specific machine learning algorithms to predict the outcome of matches, accounting for factors such as team strength, home field advantage, and injuries.

Betpath has sold monthly sports betting picks for $49/month. I have implemented various A/B tests on different Instagram stories that advertise the picks to select the type of promotions that will engage and reach more Instagram accounts. Using different GIF's and including the Betpath logo were effective in garnering more Instagram engagements and leads.

Betpath was built using Google Cloud Platform (GCP) and using Google's Datastore NoSQL database. I have experience querying the data using GQL (Google's SQL equivalent). The front-end was built using HTML/CSS and Jinja2 for templating. The back-end uses Flask. Stripe API was used as a payment processor.

Betpath models for moneylines and spreads have achieved a 1.67% ROI through 1500+ unit wagers and counting. Our totals models are weaker, but this was a great learning experience for me as I had discovered a bug within our totals models that I am working to patch. I also gained a deeper understanding of what it takes to constantly refine a sports prediction model and assess how good a model is doing during the season (current NBA season) for example through log-loss. If the model is not outperforming Vegas without their built-in 2.7% margin, then I know that I have to look deeper into the games to understand why it is not winning (not factoring in lineups properly, data scraping error, etc.).