# Book_recommender_LLM
## Semantic Book Recommender using the power of LLMs

### Pipeline
This repo consists of 5 parts as follows:
* Part 1: Data exploration and cleaning : Given the 7k-books-with-metadata Kaggle dataset, we perform some EDA and cleaning of the dataset to get books_cleaned.csv.
*  Part 2: Vector Search : We build a vector database using books description Chroma library which can be used to do semantic search.
*  Part 3: Text Classification : We do zero shot classification using LLM (facebook/bart-large-mnli) model from hugging face library. Using this we create a broad category of fiction and non-fiction books which can be used for filtering. We save it as books_with_categories.csv.
*  Part 4: Sentiment Analysis: We use the power of LLM model (j-hartmann/emotion-english-distilroberta-base) to do sentiment analysis in books description. We categorise the books into 7 emotion classes.We save this as books_with_emotions.csv.
*  Part 5: Gradio web application: Finally we create a web application using python Gradio, which can easy to use and generate a public link of the web application which can be shared with your collegues.


### Requirements
Project was tested with Python 3.11 version. The requirements.txt file contains all the dependencies which is required for successfull implementation of this project.


### Additional Improvements
Coming soon....


### Acknowledgements
This codebase is built upon [Book_recommender](https://github.com/t-redactyl/llm-semantic-book-recommender/tree/main)
