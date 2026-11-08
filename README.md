# Py-LLM-Book
- A Semantic book Recommendation Dashboard built-based off the llm reading and modeling since I followup on my Data engineering lets also see if i can scale this to embed a pipeline 


  - Initial build ( no pipeline )
  - Later build ( yes maybe)

- Made by me🃏 and for me 🛠️ but everyone seeing this should understand the codepiece and also the build so happy reading

- the info about the dataset(copy-pasting info cause i am lazy writing schema):
 #   Column                 Non-Null Count  Dtype  
---  ------                 --------------  -----  
 0   book_id                57332 non-null  str    
 1   title                  57332 non-null  str    
 2   subtitle               1760 non-null   str    
 3   series_name            408 non-null    str    
 4   series_position        393 non-null    str    
 5   authors                55428 non-null  str    
 6   description            1125 non-null   str    
 7   genres                 57097 non-null  str    
 8   language               50091 non-null  str    
 9   format                 14046 non-null  str    
 10  first_published_year   55881 non-null  float64
 11  publication_date       866 non-null    str    
 12  pages                  1060 non-null   float64
 13  rating                 1145 non-null   float64
 14  ratings_count          903 non-null    float64
 15  reviews_count          1174 non-null   float64
 16  price_usd              271 non-null    float64
 17  isbn                   680 non-null    str    
 18  thumbnail_url          26443 non-null  str    
 19  source_url             56896 non-null  str    
...
 23  date_ingested          57332 non-null  str    
 24  approx_sales_millions  165 non-null    float64

### Technical Terms:
 - NLP
 - Vector-Based Search
 - LLM(Classification)
 - Sentiment Anlaysis(making sure we put in the emotions filled for readers joy )

 ## Stuff it takes to build this :
 - I'll Breif this up in very descriptive manner.
  - Gradio:
  - Python:
  - Langchain:


## Sequence:

- ### 1) First we need data(oil) hence we got datasits(set):
  - https://www.kaggle.com/datasets/drahulsingh/best-selling-books
  - https://www.kaggle.com/datasets/ayushiiisahu/goodreads-books-dataset
  - https://www.kaggle.com/datasets/anayatasinha/open-library-books-dataset-60k-records
  - https://www.kaggle.com/datasets/thomaskonstantin/top-270-rated-computer-science-programing-books

    -Just so we are clear this datasets is not structured in proper attribute so i will be using AI for the heavy unification of this sits👁️.

- ### 2) Setting up tools and other libraries:
  - seaborn
  - ollama 3.2
  - pandas
  - langchain
  - ipykernel
  - langchain chroma
  - nomic-embed-text
  - transformers 
  - Gradio 
  - ipywidgets
  - python dotenv

  - TOTAL=(1.64GB🥀)

- ### 3) the dataset has hell lot of gaps and duplicates so we will have lot of cleaning stuff to do eventhough AI unified it (pointless):
-