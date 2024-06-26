<H3>NAME: Sri Varshan P</H3>
<H3>REGISTER NO: 212222240104</H3>
<H3>DATE: 28-04-2024</H3>
<H1 Align="center">Project Based Experiment<H1>
<H3>Objective:<H3>
To perform sentiment analysis on Facebook data and filter for messages, comments, or posts with negative feedback.

<H3>Program:</H3>
  
  ```py
import nltk
from nltk.sentiment import SentimentIntensityAnalyzer
 ```

```py
# Download NLTK resources 
nltk.download('vader_lexicon')

# Load the sentiment analyzer
sia = SentimentIntensityAnalyzer()

# Example Facebook data 
facebook_data = [
  "We won the tournament",
  "I hope you die",
  "The employees are lazy",
  "The service was extraordinary"
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

<H3>Output:</H3>

![image](https://github.com/PSriVarshan/Project-Based-Experiment-AAI/assets/114944059/52a164c6-3c0e-4429-9050-f0d4bbc6b40d)

<H3>Inference:</H3>

 A sentiment analysis project using Facebook data provides valuable learning experiences in data handling, text processing, sentiment analysis, and ethical considerations, while also honing communication, problem-solving, and project management skills.
