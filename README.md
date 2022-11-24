# Overview

This takes a text from news and run a sentiment analysis using FinBERT.

# Call URL

This is a local website that uses FinBert.
localhost:8102/sentiment
{
"text": "msft is doing good"
}

# sample return

[
{
"sentence":"Affordable Housing \ud83c\udfe1 Covid-19 \ud83c\udfe5 Cybersecurity \ud83d\udd12 The #WashingtonState
Legislature has made progress in these important areas for the 7.7 million people who live
here.",
"logit":[0.175154984,0.1141656563,0.7106794119],
"prediction":"neutral",
"sentiment_score":0.0609893277
},
{
"sentence":"Watch below to find out more \u2b07\ufe0f https:\/\/t.co\/fEWwXnCphd",
"logit":[0.1641570032,0.2038217187,0.6320212483],
"prediction":"neutral",
"sentiment_score":-0.0396647155
}
]

# duration

It takes around 1 second (on my computer). This is a time consuming process.

## RUN IT

conda activate finbert1

# The main.py returns a sentiment score

python3 main.py

# The app.py read the text information from the database and sets the score there

python3 app.py
