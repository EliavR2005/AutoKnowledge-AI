# AutoKnowledge AI

### Intelligent Document Classification & Semantic Search

**Turning unstructured business information into organized, searchable and meaningful knowledge.**

AutoKnowledge AI is an artificial intelligence project designed to improve how organizations classify, organize and retrieve business information. It combines supervised machine learning and semantic search techniques to transform textual reports into structured knowledge that can be accessed more efficiently.

The project explores how Natural Language Processing (NLP), text classification and sentence embeddings can work together to build a smarter document management and information retrieval solution.

---

## Project Overview

Organizations generate large amounts of textual information every day, including technical incidents, financial reports and human resources requests. Manually organizing this information can be time-consuming and makes it difficult to locate relevant documents.

AutoKnowledge AI addresses this challenge through an intelligent pipeline that:

- Automatically classifies business reports into predefined categories.
- Processes textual information using Natural Language Processing techniques.
- Evaluates supervised machine learning models.
- Converts documents into numerical vector representations.
- Retrieves semantically related documents using natural-language queries.

## Key Features

| Feature | Description |
|---|---|
| Document Classification | Automatically categorizes business reports. |
| Text Preprocessing | Tokenization, stopword removal and lemmatization. |
| TF-IDF Representation | Converts text into numerical features for machine learning. |
| Supervised Learning | Trains and evaluates classification algorithms. |
| Model Evaluation | Uses accuracy, precision, recall, F1-score and confusion matrices. |
| Sentence Embeddings | Represents documents as 384-dimensional vectors. |
| Semantic Search | Retrieves relevant documents based on meaning rather than exact keyword matches. |

## Technologies & Tools

**Programming Language**
- Python

**Machine Learning & NLP**
- Scikit-learn
- Sentence Transformers
- spaCy
- Pandas
- NumPy

**Development Environment**
- Google Colab
- Jupyter Notebook
- Git & GitHub

**Models and Algorithms**
- Multinomial Naive Bayes
- Linear Support Vector Machine (LinearSVC)
- TF-IDF
- `paraphrase-multilingual-MiniLM-L12-v2`

## System Workflow

The solution follows a document processing and retrieval pipeline:

1. **Data Preparation:** Load and organize business reports with predefined categories.
2. **Text Preprocessing:** Clean and normalize textual information.
3. **Feature Extraction:** Transform documents into TF-IDF numerical vectors.
4. **Model Training:** Train supervised classification algorithms.
5. **Model Evaluation:** Compare performance using classification metrics.
6. **Embedding Generation:** Encode documents into 384-dimensional semantic vectors.
7. **Semantic Retrieval:** Compare user queries against stored document embeddings using cosine similarity.
8. **Result Ranking:** Return the three most relevant documents.

## Model Evaluation

Two supervised learning algorithms were evaluated using a stratified training and testing split.

| Algorithm | Accuracy |
|---|---:|
| Multinomial Naive Bayes | 80% |
| Linear SVM | 80% |

Both models achieved the same accuracy on the test dataset. Linear SVM was selected as the final model according to the project's original algorithm selection.

**Evaluation metrics:**
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

## Semantic Search

AutoKnowledge AI uses the multilingual Sentence Transformer model:

`paraphrase-multilingual-MiniLM-L12-v2`

Each document is transformed into a numerical embedding with **384 dimensions**.

When a user enters a natural-language query, the system generates its embedding and calculates cosine similarity against the stored document vectors.

The three most similar reports are returned, allowing users to discover related information even when the wording differs from the original documents.

## Project Dataset

The project uses a dataset of **100 business reports** divided into three categories:

- Finance
- Human Resources
- Technical Support

The supervised classification dataset was divided into:
- 80% training data.
- 20% testing data.

An additional evaluation was performed using five new reports, all of which received their expected categories.

*Note: Results correspond to this project's experimental dataset and do not represent production-level performance.*

## Repository Structure

```text
AutoKnowledge-AI/
│
├── notebooks/
│   └── AutoKnowledge_Clasificacion_Modelos.ipynb
│
├── docs/
│   └── project-documentation.md
│
├── images/
│   └── results/
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Getting Started

### Requirements

- Python 3.10 or newer.
- Jupyter Notebook or Google Colab.
- Internet connection to download the pretrained language model.

### Run the Project

1. Clone the repository:

```bash
git clone https://github.com/EliavR2005/AutoKnowledge-AI.git
```

2. Open the project notebook:

```text
notebooks/AutoKnowledge_Clasificacion_Modelos.ipynb
```

3. Run the notebook cells in order.

Google Colab can also be used to execute the notebook without configuring a local Python environment.

## Future Improvements

Potential improvements include:

- Expanding the dataset with more business documents.
- Improving category labeling and dataset quality.
- Testing additional classification algorithms.
- Implementing a persistent vector database.
- Developing a web interface for document classification and search.
- Integrating the solution into a document management platform.

## Learning Outcomes

This project provided practical experience with:

- Supervised machine learning.
- Natural Language Processing.
- Text preprocessing and feature engineering.
- Model evaluation and error analysis.
- Sentence embeddings and semantic similarity.
- Information retrieval systems.

## Author

**Eliav Reyes**

Software Development Engineering Student

GitHub: [@EliavR2005](https://github.com/EliavR2005)

---

*AutoKnowledge AI — Making business information easier to organize, understand and retrieve.*
