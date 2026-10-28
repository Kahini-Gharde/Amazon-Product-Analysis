Amazon Product Review Analysis
SI Lab Project | Semester V | B.Tech CSE (AI & DS)
Ramdeobaba University, Nagpur

A Python-based project that analyses Amazon product reviews using statistical techniques and machine learning. It explores customer ratings, preprocesses review text, studies patterns in feedback, and predicts whether a review is Positive, Neutral, or Negative. A Gradio interface allows users to analyse one review or multiple reviews.
Dataset
- Dataset: Amazon Reviews Multi (English)
- Source: Hugging Face — SetFit/amazon_reviews_multi_en
- The notebook downloads the training data directly from Hugging Face.
- Ratings are mapped from the dataset labels to a 1–5 star scale.
Features
- Dataset loading and exploratory data analysis
- Missing-value and duplicate checks
- Review-text cleaning and sentiment labelling
- Stratified sampling and rating distribution analysis
- Statistical analysis, including sampling, Central Limit Theorem, confidence intervals, hypothesis testing, correlation, and chi-square testing
- Frequent-word analysis by sentiment
- TF-IDF feature extraction
- Comparison of Multinomial Naive Bayes, Logistic Regression, and Linear SVM
- Evaluation using accuracy, precision, recall, F1-score, macro F1, and a confusion matrix
- Gradio interface for single-review and batch predictions
Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- SciPy
- NLTK
- Scikit-learn
- Joblib
- Gradio
- Jupyter Notebook / Google Colab
How to Run
Option 1: Google Colab
1. Upload Amazon-Product-Review-Analysis.ipynb to Google Colab.
2. Run the notebook cells from top to bottom.
3. Allow the notebook to download the dataset and required NLTK stopwords.
4. Review the statistical analysis and model-comparison outputs.
5. Run the Gradio interface cell to launch the review sentiment analyzer.
Option 2: Run Locally
1. Install Python 3.10 or a compatible version.
2. Install the required packages:
   pip install gradio pandas numpy matplotlib seaborn scipy nltk scikit-learn joblib jupyter
3. Open the notebook:
   jupyter notebook Amazon-Product-Review-Analysis.ipynb
4. Run all cells in order. An internet connection is required to download the dataset and NLTK stopwords.
Sentiment Labels
Rating	Sentiment
1–2 stars	Negative
3 stars	Neutral
4–5 stars	Positive


Model Evaluation
The notebook compares the implemented models using the held-out test set. The best model is selected using Macro F1-score. Evaluation values depend on the data and execution; check the notebook output for the actual results rather than assuming fixed scores.

After training, the notebook saves:
- best_model.pkl — selected trained classifier
- tfidf_vectorizer.pkl — fitted TF-IDF vectorizer
These files are used by the Gradio interface. Run the training and saving cells before running the interface.
Using the Interface
- Single review: Enter a product review and click Analyze to view its predicted sentiment and class scores.
- Multiple reviews: Enter one review per line to analyse several reviews together.
- Model results: View the model evaluation results and confusion matrix, if included in the running notebook.
Limitations
- Predictions depend on the dataset and training process.
- Sarcasm, ambiguous wording, very short reviews, and overlap between neutral and other sentiments can reduce accuracy.
- The dataset and text processing are English-focused.
- Confidence scores shown in the interface should be treated as model scores, not guarantees that a prediction is correct.
Project Structure
Amazon-Product-Review-Analysis/
├── Amazon-Product-Review-Analysis.ipynb
├── best_model.pkl              # generated after model training
├── tfidf_vectorizer.pkl        # generated after model training
└── README.md
Project Author
Kahini Gharde
B.Tech CSE (Artificial Intelligence and Data Science)
Ramdeobaba University, NagpurAmazon Product Review Analysis
SI Lab Project | Semester V | B.Tech CSE (AI & DS)
Ramdeobaba University, Nagpur

A Python-based project that analyses Amazon product reviews using statistical techniques and machine learning. It explores customer ratings, preprocesses review text, studies patterns in feedback, and predicts whether a review is Positive, Neutral, or Negative. A Gradio interface allows users to analyse one review or multiple reviews.
Dataset
- Dataset: Amazon Reviews Multi (English)
- Source: Hugging Face — SetFit/amazon_reviews_multi_en
- The notebook downloads the training data directly from Hugging Face.
- Ratings are mapped from the dataset labels to a 1–5 star scale.
Features
- Dataset loading and exploratory data analysis
- Missing-value and duplicate checks
- Review-text cleaning and sentiment labelling
- Stratified sampling and rating distribution analysis
- Statistical analysis, including sampling, Central Limit Theorem, confidence intervals, hypothesis testing, correlation, and chi-square testing
- Frequent-word analysis by sentiment
- TF-IDF feature extraction
- Comparison of Multinomial Naive Bayes, Logistic Regression, and Linear SVM
- Evaluation using accuracy, precision, recall, F1-score, macro F1, and a confusion matrix
- Gradio interface for single-review and batch predictions
Technologies Used
- Python
- Pandas, NumPy
- Matplotlib, Seaborn
- SciPy
- NLTK
- Scikit-learn
- Joblib
- Gradio
- Jupyter Notebook / Google Colab
How to Run
Option 1: Google Colab
1. Upload Amazon-Product-Review-Analysis.ipynb to Google Colab.
2. Run the notebook cells from top to bottom.
3. Allow the notebook to download the dataset and required NLTK stopwords.
4. Review the statistical analysis and model-comparison outputs.
5. Run the Gradio interface cell to launch the review sentiment analyzer.
Option 2: Run Locally
1. Install Python 3.10 or a compatible version.
2. Install the required packages:
   pip install gradio pandas numpy matplotlib seaborn scipy nltk scikit-learn joblib jupyter
3. Open the notebook:
   jupyter notebook Amazon-Product-Review-Analysis.ipynb
4. Run all cells in order. An internet connection is required to download the dataset and NLTK stopwords.
Sentiment Labels
Rating	Sentiment
1–2 stars	Negative
3 stars	Neutral
4–5 stars	Positive


Model Evaluation
The notebook compares the implemented models using the held-out test set. The best model is selected using Macro F1-score. Evaluation values depend on the data and execution; check the notebook output for the actual results rather than assuming fixed scores.

After training, the notebook saves:
- best_model.pkl — selected trained classifier
- tfidf_vectorizer.pkl — fitted TF-IDF vectorizer
These files are used by the Gradio interface. Run the training and saving cells before running the interface.
Using the Interface
- Single review: Enter a product review and click Analyze to view its predicted sentiment and class scores.
- Multiple reviews: Enter one review per line to analyse several reviews together.
- Model results: View the model evaluation results and confusion matrix, if included in the running notebook.
Limitations
- Predictions depend on the dataset and training process.
- Sarcasm, ambiguous wording, very short reviews, and overlap between neutral and other sentiments can reduce accuracy.
- The dataset and text processing are English-focused.
- Confidence scores shown in the interface should be treated as model scores, not guarantees that a prediction is correct.
Project Structure
Amazon-Product-Review-Analysis/

   Amazon-Product-Review-Analysis.ipynb
  
   best_model.pkl
  
  
   README.md

  
Project Author
Kahini Gharde
B.Tech CSE (Artificial Intelligence and Data Science)
Ramdeobaba University, Nagpur
