# 🎬 Movie Recommendation System

An end-to-end Machine Learning project focused on building a personalized movie recommendation system using content-based filtering, collaborative filtering, and hybrid recommendation techniques.

The project explores the complete Machine Learning workflow, including data collection, exploratory data analysis, preprocessing, feature engineering, recommendation algorithms, model evaluation, application development, and deployment.

> **Project Status:** 🚧 In Development

---

## 📌 Overview

Movie recommendation systems help users discover relevant movies based on their interests, preferences, and interactions.

This project aims to develop a recommendation engine that combines movie metadata and user-rating patterns to generate meaningful and personalized movie suggestions.

The system will explore multiple recommendation approaches, evaluate their performance, and integrate the resulting models into an interactive web application.

The primary objective is to build a well-structured, modular, tested, and deployable Machine Learning project while developing a practical understanding of recommendation systems.

## 🎯 Project Objectives

- Understand the fundamentals of recommendation systems.
- Collect and analyze movie metadata and user-rating datasets.
- Perform exploratory data analysis (EDA).
- Clean, preprocess, and transform raw datasets.
- Develop different recommendation algorithms.
- Implement content-based and collaborative filtering.
- Explore hybrid recommendation techniques.
- Evaluate and compare recommendation models.
- Build an interactive movie recommendation application.
- Deploy the application for public access.
- Follow professional software development and Machine Learning practices.

## ✨ Planned Features

| Feature | Description | Status |
|---|---|---|
| Movie Exploration | Explore movie information, genres, and metadata | Planned |
| Popularity-Based Recommendations | Recommend movies using popularity and rating statistics | Planned |
| Content-Based Filtering | Recommend movies based on genres, descriptions, and other features | Planned |
| Collaborative Filtering | Generate recommendations using user-movie interactions | Planned |
| Hybrid Recommendations | Combine multiple recommendation approaches | Planned |
| Movie Search | Search for movies by title | Planned |
| Personalized Recommendations | Generate suggestions based on user preferences | Planned |
| Movie Details | Display movie information and posters | Planned |
| Interactive Web Application | Provide a user-friendly movie discovery interface | Planned |

*Features will be implemented and documented progressively.*

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Data Manipulation | NumPy, Pandas |
| Data Visualization | Matplotlib, Seaborn, Plotly |
| Machine Learning | Scikit-learn |
| Recommendation Techniques | TF-IDF, Cosine Similarity, Collaborative Filtering |
| Model Serialization | Joblib |
| Development Environment | Jupyter Notebook, VS Code |
| Web Application | Streamlit |
| Backend API | FastAPI (optional, if required) |
| Testing | Pytest |
| Code Quality | Ruff |
| Version Control | Git, GitHub |
| Deployment | Streamlit Community Cloud / Suitable Hosting Platform |

## 📊 Datasets

The project uses movie metadata and user-rating information from publicly available datasets.

### 1. MovieLens Latest Small Dataset

**Source:** [GroupLens – MovieLens Datasets](https://grouplens.org/datasets/movielens/)

Provides movie information, user ratings, tags, and external movie identifiers.

| File | Description |
|---|---|
| `movies.csv` | Movie IDs, titles, and genres |
| `ratings.csv` | User ratings and timestamps |
| `tags.csv` | User-generated movie tags |
| `links.csv` | IMDb and TMDB movie identifiers |

**Primary use cases:**
- Collaborative filtering.
- User-movie interaction analysis.
- Rating-based evaluation.
- Mapping MovieLens movie IDs to external movie identifiers.

### 2. The Movies Dataset

**Source:** [The Movies Dataset – Kaggle](https://www.kaggle.com/datasets/rounakbanik/the-movies-dataset)

The project also uses the `movies_metadata.csv` file, which provides additional movie information.

Relevant fields include:

- Movie titles and original titles.
- Genres.
- Movie descriptions and overviews.
- Popularity scores.
- Vote averages and vote counts.
- Release dates.
- Poster paths.
- Original language.

**Primary use cases:**
- Content-based filtering.
- Movie feature extraction.
- Genre and description analysis.
- Movie information and metadata enrichment.

### Dataset Integration

MovieLens and The Movies Dataset may be connected through external movie identifiers.

The intended mapping is:

`MovieLens links.csv (tmdbId) → movies_metadata.csv (id)`

The identifiers will be validated before merging datasets.

> **Data handling:** Original datasets will remain unchanged in the local `data/raw/` directory. Downloaded datasets and generated data files will not be committed to the public repository. Dataset sources and applicable usage conditions will be documented.

## 🧠 Recommendation Approaches

The project will progressively implement and compare the following techniques.

### 1. Popularity-Based Filtering

Recommends movies using popularity indicators such as rating counts and average ratings.

### 2. Content-Based Filtering

Recommends movies based on similarities between their features.

Potential techniques include:
- Genre-based similarity.
- Text vectorization using TF-IDF.
- Cosine similarity.
- Movie description and metadata analysis.

### 3. Collaborative Filtering

Uses user-movie interaction patterns to identify movies that may interest a particular user.

Potential techniques include:
- User-based collaborative filtering.
- Item-based collaborative filtering.
- Matrix factorization.
- Singular Value Decomposition (SVD).

### 4. Hybrid Recommendation System

Combines multiple recommendation approaches to generate more balanced and personalized recommendations.

## 📂 Project Structure

The repository will follow a modular structure as the project develops.

```text
Movie-Recommendation-System/
│
├── data/
│   ├── raw/
│   │   ├── movielens-latest-small/
│   │   └── the-movies-dataset/
│   ├── processed/
│   └── README.md
│
├── notebooks/
│   ├── 01-data-understanding.ipynb
│   ├── 02-exploratory-data-analysis.ipynb
│   └── 03-data-preprocessing.ipynb
│
├── src/
│   ├── data/
│   ├── features/
│   ├── recommenders/
│   └── evaluation/
│
├── models/
│
├── app/
│
├── tests/
│
├── docs/
│
├── reports/
│
├── README.md
├── requirements.txt
├── .gitignore
└── LICENSE
```

*This represents the planned project structure. Additional modules and files will be added when required.*

## 🔄 Development Workflow

The project will follow these development stages:

| Phase | Development Stage |
|---|---|
| 01 | Project Setup and Repository Configuration |
| 02 | Dataset Collection and Understanding |
| 03 | Exploratory Data Analysis |
| 04 | Data Cleaning and Preprocessing |
| 05 | Feature Engineering |
| 06 | Popularity-Based Recommendation |
| 07 | Content-Based Filtering |
| 08 | Collaborative Filtering |
| 09 | Hybrid Recommendation System |
| 10 | Model Evaluation and Comparison |
| 11 | Application Development |
| 12 | Testing and Optimization |
| 13 | Deployment |
| 14 | Documentation and Final Release |

## ⚙️ Installation and Setup

### Prerequisites

- Python 3.10 or later.
- Git.
- Jupyter Notebook or Jupyter support in VS Code.

### 1. Clone the repository

```bash
git clone https://github.com/gursimranai/Movie-Recommendation-System.git
```

### 2. Navigate to the project directory

```bash
cd Movie-Recommendation-System
```

### 3. Create a virtual environment

```bash
python -m venv .venv
```

### 4. Activate the virtual environment

**Windows PowerShell:**

```powershell
.venv\Scripts\Activate.ps1
```

### 5. Install dependencies

```bash
python -m pip install --upgrade pip
pip install -r requirements.txt
```

### 6. Launch Jupyter Notebook

```bash
jupyter notebook
```

> Dataset download and placement instructions will be documented in `data/README.md`.

## 📈 Model Evaluation

Recommendation models will be evaluated according to their respective tasks.

### Ranking and Recommendation Metrics

- Precision@K
- Recall@K
- Mean Average Precision (MAP@K)
- Normalized Discounted Cumulative Gain (NDCG@K)

### Rating Prediction Metrics

- Mean Absolute Error (MAE)
- Root Mean Squared Error (RMSE)

The evaluation process will also consider recommendation diversity, coverage, and the quality of suggested movies where appropriate.

## 🧪 Testing and Code Quality

The project will use automated testing and code quality tools to improve reliability and maintainability.

- **Pytest:** Unit and integration testing.
- **Ruff:** Python linting and code quality checks.
- **Modular architecture:** Reusable components and separation of concerns.
- **Documentation:** Clear explanations of implementation decisions and experiments.

## 🚀 Deployment

The final recommendation system is intended to be available through an interactive web application.

Planned deployment activities include:

- Integrating recommendation models.
- Developing the application interface using Streamlit.
- Managing dependencies and configuration.
- Testing application functionality.
- Deploying the application to a suitable hosting platform.

**Live Demo:** Coming Soon

## 🗺️ Project Roadmap

- [x] Initialize the project folder structure.
- [x] Collect and place the initial datasets locally.
- [ ] Complete repository documentation.
- [ ] Configure the development environment.
- [ ] Create and complete data understanding notebook.
- [ ] Perform exploratory data analysis.
- [ ] Implement data cleaning and preprocessing.
- [ ] Develop popularity-based recommendations.
- [ ] Implement content-based filtering.
- [ ] Implement collaborative filtering.
- [ ] Develop a hybrid recommendation system.
- [ ] Evaluate and compare recommendation approaches.
- [ ] Build the interactive web application.
- [ ] Add automated tests.
- [ ] Deploy the application.
- [ ] Complete technical documentation.

## 📚 Documentation

Technical documentation, experiment results, architecture diagrams, and implementation notes will be maintained in the `docs/` and `reports/` directories as development progresses.

## 🤝 Contributions

Suggestions, improvements, and contributions are welcome.

If you discover an issue or have an idea for improving the project, feel free to open an issue or submit a pull request.

## 📄 License

The project license will be specified before the public release. Please refer to the dataset providers' terms for the applicable dataset usage conditions.

---

## 👨‍💻 Author

**Gursimran Singh**

- GitHub: [@gursimranai](https://github.com/gursimranai)

---

⭐ If you find this project interesting, consider giving the repository a star.

**Built with Python, Machine Learning, and curiosity.**