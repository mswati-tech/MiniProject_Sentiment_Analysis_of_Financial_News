📊**Financial News Sentiment Analysis & Topic Modeling**

This project analyzes financial news headlines using a combination of lexicon-based, machine learning, deep learning, and topic modeling techniques. 
It compares the performance of VADER, LSTM, and FinBERT on a mini dataset and also applies Logistic Regression, SVM, and Naive Bayes on the full dataset. 
Finally, it uses LDA Topic Modeling to extract dominant topics.

🚀 **Features**

**Text Preprocessing**

Tokenization, stopword removal, lemmatization, and cleaning of financial news headlines.

**Lexicon-Based Sentiment Analysis**

NLTK’s VADER for quick baseline labeling of sentiment (positive, neutral, negative).

**Machine Learning Models**

Logistic Regression

Support Vector Machine (SVM)

Complement Naive Bayes (NB)

**Deep Learning Models**

LSTM (with Keras/TensorFlow)

FinBERT (HuggingFace Transformers – fine-tuned for financial sentiment)

**Topic Modeling**

Latent Dirichlet Allocation (LDA) with Gensim

pyLDAvis interactive visualization

📂**Project Structure**

├── FinNews.txt                # Input dataset (financial headlines)

├── code.py / code.ipynb   # Core code

├── Financial_News_with_topics.txt # Output file with sentiment + topics

├── README.md                  # Documentation

📊**Workflow**

**1. Data Input**

Reads FinNews.txt (line-separated financial news headlines).

Cleans, preprocesses, and stores in a Pandas DataFrame.

**2. Sentiment Analysis**

VADER labels each headline into @positive, @negative, or @neutral.

Visualized via bar charts and word clouds.

**3. Machine Learning Models**

Extracts features using TF-IDF (LR & SVM) and CountVectorizer (NB).

Trains & evaluates Logistic Regression, SVM, and ComplementNB.

**4. Deep Learning Models**

LSTM trained on a padded sequence representation.

FinBERT applied using HuggingFace pipeline for financial domain sentiment.

Compared against VADER (used as pseudo ground truth on mini dataset of 50 headlines).

**5. Topic Modeling**

Applies LDA to extract 3 key topics from the financial headlines.

**Example results:**

Topic 1: Corporate News & Market Moves

Topic 2: Business Services & Organizational Updates

Topic 3: Financial Performance & Earnings
