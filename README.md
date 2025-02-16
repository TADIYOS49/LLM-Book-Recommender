# LLM-Based Book Recommender

![Book Recommender](https://img.shields.io/badge/LLM-Book%20Recommender-blue)

## 📌 Project Overview
The **LLM-Based Book Recommender** is a machine learning-powered system that helps users find books based on various criteria, such as similarity in descriptions, emotional tone, and fiction/non-fiction classification. It utilizes **Large Language Models (LLMs)** and **vector search techniques** to provide accurate and personalized recommendations.

## 🚀 Features
1. **Data Preprocessing** 📊
   - Collected book data from **Kaggle** (found in `books.csv`).
   - Cleaned missing values and structured the dataset for better usability.

2. **Text Classification** 🏷️
   - Classified books into **Fiction** and **Non-Fiction** categories.
   - Used **BART zero-shot classifier** from **Meta** to label books based on descriptions.

3. **Vector Search** 🔍
   - Used **ChromaDB** to store vector embeddings of book descriptions.
   - Generated embeddings using **OpenAI's embedding model**.
   - Enabled **semantic search**, allowing users to find books based on meaning rather than just keywords.

4. **Sentiment Analysis** 😊😢😠
   - Used **RoBERTa's emotion classifier** to categorize books based on six emotions (e.g., happy, sad, anger, etc.).
   - Users can search for books by emotional tone.

5. **Gradio UI** 🎨
   - Built an **interactive Gradio UI** to allow users to search books by:
     - **Emotion-based filtering**
     - **Vector search (semantic similarity)**
     - **Fiction vs. Non-Fiction classification**

## 📁 Project Structure
```
│── books.csv                # Original dataset
├── notebooks/
│   ├── data_preprocessing.ipynb  # Data cleaning and preprocessing
│   ├── text_classification.ipynb # Fiction/Non-Fiction classification
│   ├── vector_search.ipynb       # Embedding and vector storage
│   ├── sentiment_analysis.ipynb  # Emotion classification
├── app/
│   ├── dashboard.py             # Gradio UI implementation
├── README.md                     # Project documentation
```

## 🔗 Notebooks & Code
You can find the main notebook for **Vector Search** [here](https://github.com/TADIYOS49/LLM-Book-Recommender/blob/main/vector_search.ipynb).

###Run Gradio UI
```bash
python dashboard.py
```

### 3️⃣ Example Usage
- **Search books based on emotions (e.g., happy, sad, excited).**
- **Find books with similar meaning using vector search.**
- **Filter books by Fiction or Non-Fiction.**

## 📚 Technologies Used
- **ChromaDB** - Vector search
- **OpenAI embeddings** - Semantic text similarity
- **BART Zero-Shot Classifier** - Text classification
- **RoBERTa Emotion Classifier** - Sentiment analysis
- **Gradio** - UI for interactive book search

## 🤝 Contributing
Feel free to fork the repo, submit issues, or create pull requests to improve the recommender system.

## 📜 License
This project is licensed under the MIT License.

---
📌 **Author**: [TADIYOS49](https://github.com/TADIYOS49)  
🎯 **Project Repository**: [LLM-Book-Recommender](https://github.com/TADIYOS49/LLM-Book-Recommender)

