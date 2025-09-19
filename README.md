# Naive-Bayes-Model-From-Scratch
"ML models implemented from scratch using NumPy and Pandas only"

📩 Naive Bayes Classifier (From Scratch)

📌 Overview

This project implements a Naive Bayes Classifier from scratch (without libraries like scikit-learn) for text classification (e.g., Spam vs Ham).
Naive Bayes is a probabilistic algorithm based on Bayes’ Theorem with the assumption that features (words) are conditionally independent given the class.


---

⚙️ How it Works

1. Preprocessing

Tokenize text → build vocabulary → Bag of Words representation.



2. Training (fit)

Compute prior probability:




$$P(y=c) = \frac{\#docs\ in\ class\ c}{\#total\ docs}$$

$$P(word \mid class) = \frac{count(word\ in\ class) + 1}{total\ words\ in\ class + |V|}$$

3. Prediction

For a new message, compute:




$$Score(c) = \log P(y=c) + \sum_{i=1}^{n} x_i \cdot \log P(word_i \mid y=c)$$


---

🖥️ Example Dataset

label   | message
--------|-------------------
spam    | win money now
spam    | claim your prize
ham     | hi how are you
ham     | let’s go to dinner


---

📊 Results

Achieved good accuracy on spam/ham dataset(~97%).

Outputs accuracy, precision, recall, and F1-score.



---

📚 References

Stanford NLP IR Book – Chapter 13

Scikit-learn Documentation

StatQuest: Naive Bayes Explained (YouTube)
