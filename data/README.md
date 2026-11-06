# Dataset Documentation

This directory contains the datasets used for developing and evaluating the Movie Recommendation System.

## Dataset Source

**Dataset:** MovieLens Latest Small

**Provider:** GroupLens Research

**Download:** https://grouplens.org/datasets/movielens/

**Format:** CSV

## Directory Structure

```text
data/
│
├── raw/
│   └── movielens-latest-small/
│       ├── movies.csv
│       ├── ratings.csv
│       ├── tags.csv
│       ├── links.csv
│       └── README.html
│
└── processed/
```

## Dataset Files

| File | Description |
|---|---|
| `movies.csv` | Movie IDs, titles, and genres |
| `ratings.csv` | User ratings and timestamps |
| `tags.csv` | User-generated movie tags |
| `links.csv` | IMDb and TMDB identifiers |

## Data Organization

- `raw/`: Stores original, unmodified datasets.
- `processed/`: Stores cleaned and transformed datasets generated during development.

## Usage Guidelines

- Preserve original datasets without modifications.
- Perform preprocessing on separate copies of the data.
- Do not commit downloaded dataset files to the public repository.
- Follow the dataset provider's licensing and usage conditions.

## Notes

Dataset exploration, preprocessing, feature engineering, and model development will be documented in the project's Jupyter notebooks.

For detailed information about the dataset structure and usage, refer to the original README included with the downloaded dataset.