<H3>NAME: G.Jayanth</H3>
<H3>REGISTER NO: 212221230030</H3>
<H3>DATE: 15-05-2024</H3>
<H1 Align="center">Project Based Experiment<H1>

## Objective:
To perform sentiment analysis on Facebook data and filter for messages, comments, or posts with negative feedback.

## Program:
  
  ```py
import nltk
from nltk.sentiment import SentimentIntensityAnalyzer

# Download NLTK resources 
nltk.download('vader_lexicon')

# Load the sentiment analyzer
sia = SentimentIntensityAnalyzer()

# Example Facebook data 
facebook_data = [
    "I love the new feature! It's amazing.",
    "The service was terrible. I'm very disappointed.",
    "Great job on the update!",
    "The product quality is poor. I won't be buying again.",
    
]

# Perform sentiment analysis and filter for negative feedback
negative_feedback = []

for message in facebook_data:
    sentiment_score = sia.polarity_scores(message)['compound']
    if sentiment_score < 0:  # Negative sentiment
        negative_feedback.append(message)

# Print the negative feedback
print("Negative Feedback:")
for feedback in negative_feedback:
    print(feedback)

 ```

## OUTPUT:
![326264530-6ce64425-220c-4fd3-a539-b5e07056e655](https://github.com/Afsarjumail/Project-Based-Experiment-AAI/assets/118343395/f88f4bf9-ed93-49ae-85e0-e7fa3bd67dee)


<H3>RESULT:</H3>
 A sentiment analysis project using Facebook data provides valuable learning experiences in data handling, text processing, sentiment analysis, and ethical considerations, while also honing communication, problem-solving, and project management skills.
