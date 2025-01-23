

# **Fake News Detection using Machine Learning**

This Python project uses machine learning to classify news articles or headlines as **REAL** or **FAKE** based on the content. The model is trained using a dataset of labeled news articles.

## **Features**:
- **Machine Learning**: Implements logistic regression to predict fake vs real news.
- **Real-Time Predictions**: Enter any news article or headline to check if it's **REAL** or **FAKE**.
- **Customizable Dataset**: Replace the default dataset with your own to retrain the model.

## **Requirements**:
- Python 3.x
- Pandas
- Scikit-learn
- Regular Expressions (re)

Install the necessary dependencies:
```bash
pip install pandas scikit-learn
```

## **Steps to Run**:

### 1. Clone this Repository:
```bash
git clone https://github.com/sanjushri777/FAKE-NEWS-prediction-ML-.git
cd FAKE-NEWS-prediction-ML-
```

### 2. Prepare the Dataset:
Ensure you have the `fake_news_dataset.csv` in the same directory as the script, or update the script to point to the correct location of your dataset.

The dataset should have at least two columns:
- `news`: News article or headline.
- `subject`: Label of the article ('fake' or 'real').

### 3. Run the Script:
```bash
python fake_news_detector.py
```

### 4. Input Your News:
The program will prompt you to enter a news article or headline to check if it's **REAL** or **FAKE**. To quit, type `exit`.

---

## **How the Model Works**:

1. **Data Preprocessing**:
   - News content is converted to lowercase.
   - Special characters and extra spaces are removed.
   
2. **Vectorization**:
   - The `CountVectorizer` converts the text data into numerical format, with a maximum of 5000 features.

3. **Model Training**:
   - The model is trained using **Logistic Regression**.
   - The dataset is split into 80% training and 20% testing.

4. **Prediction**:
   - The model predicts whether the input text is **REAL** or **FAKE**.
   - The confidence score of the prediction is also displayed.

---

## **Pros**:
- Helps detect and classify fake news articles.
- User-friendly interface for real-time predictions.

## **Cons**:
- Accuracy depends on the quality of the dataset.
- Model could be improved with a larger, more diverse dataset.

---

## **License**:
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

