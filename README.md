
# Fake News Detection with RNN 

This is a project built while participating in the AIcrowd KIIT(AI) Mini Blitz Challenge and is the first one out of the three puzzles given. We are given a train, test and val set and the objective is to submit a submission.csv with our predicted labels on the test set after modelling. For this, I went through several different approaches working with a total of 270,000 datapoints. 


  
## 🚀 The Result

I was able to score a **F1 score of 0.949** on the test set and secured the first place for this specific puzzle as of now. 
 

## ✏ Tech Stack for Project Development

- Python
- Tensorflow
- Scikit-learn
- Pandas
- Numpy
- Seaborn
- Plotly
- Regex


  
## 🧠 Different Approaches Used & Findings

 1. I first tried to fine-tune the bert-base-uncased model on our dataset. Soon, I found out that it was taking a long time to train and the time it'd take to fully complete would excede the 12-hour limit on Colab. Hence, I moved on to the next approach.
 2. Next, I tried Pycaret to get a consensus of which model would be best for the task. However, the memory required for our large dataset was simply too large and everytime it was executed, the runtime crashed due to the same reason.
 3. Now, I wanted to go back to the basics and attempt with the traditional models and all of them worked including Logistic Regression, Decision Tree, Gradient Boosting, Random Forests, and XGBoost. Out of these, Logistic Regression performed the best and it gave a F1 Score of **0.925** after submission which was quite good.
 4. Finally, I gave RNNs a shot to try and improve upon the current score through DL and after 5 epochs (with early stopping), I was able to get a better accuracy than Logistic Regression with a F1 Score of **0.949** upon submission. 


  

## 🔗 Connect with me:
[![portfolio](https://img.shields.io/badge/my_portfolio-000?style=for-the-badge&logo=ko-fi&logoColor=white)](https://www.polywork.com/kunal_bhadra)
[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/kunal-bhadra-cs/)
[![twitter](https://img.shields.io/badge/twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/kunal_kaun)

  