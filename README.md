# Movie Recommender System 

This is a Streamlit web application that recommends similar movies based on user interests. The model uses **Cosine Similarity** to find and recommend movies based on the content of the movies in the dataset.

## Demo




## Workflow

1. **Cosine Similarity** is used to measure the similarity between movies based on their attributes (such as genres, plot, etc.).
2. The dataset is processed and vectorized to generate numerical representations (vectors) of movies.
3. Cosine Similarity is calculated between the movie vectors to recommend similar movies.
4. The result is a value between 0 and 1, where:
   - `0` means completely different.
   - `1` means identical.

## Dataset

The dataset used for this project can be found at:
https://www.kaggle.com/datasets/tmdb/tmdb-movie-metadata


## How to Run the Project

### 1. Clone the Repository

Clone the repository using the following command:

```bash
git clone https://github.com/entbappy/Movie-Recommender-System-Using-Machine-Learning.git
```

### 2. Create a Conda Environment

Create and activate a Conda environment for the project:

```bash
conda create -n movie python=3.7.10 -y
conda activate movie
```

### 3. Install Requirements

Install the required dependencies:

```bash
pip install -r requirements.txt
```

### 4. Generate the Model

Run the following Jupyter Notebook to generate the models:

```bash
Movie Recommender System Data Analysis.ipynb
```

### 5. Run the Application

Start the Streamlit application with the following command:

```bash
streamlit run app.py
```