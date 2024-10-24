# Media Analysis of PSI-20 Companies

- [Slides 01](https://hugoverissimo21.github.io/FCD-project/slides01)

## structure: folders and files

```
│
│   README.md
│   data04.parquet                  [via 03_data_filtering.ipynb]
│   dtree01.joblib                  [via dtree01.ipynb] trained model to filter news 
│   main.py                         [not finished] given a companies dictionary, returns filtered news
│   noticias.csv                    news websites from where to extract news
│
└───assets
│   │   dtree01 (branches).svg
│   │   dtree01 (percentages).svg
│   │   newsLost.svg
│   │
│   └───dtree01_train                    
│       │   ...
│
└───data
│   │   data01.parquet              [via 01_api_request.ipynb]
│   │   data02.parquet              [via 02_extract_text.ipynb]
│   │   data03.parquet              [via 03_data_filtering.ipynb]
│   │   dtree01.csv                 dataset to train the decision tree model to filter the news
│   │   parquet.ipynb               makes reading parquet files easier
│
└───notebooks
│   │   01_api_request.ipynb        python scripts to do arquivo.pt api requests/extraction given a dictionary of companies
│   │   02_extract_text.ipynb       python script to extract text from arquivo.pt given linkToExtractedText urls
│   │   03_data_filtering.ipynb     applies dtree01.joblib, removes 90% duplicates, and some minor tweaks
│   │   dtree01.ipynb               decision tree model training/creation to filter news (ignore ads and news websites first pages)
│
└───slides01
│   │   index.qmd
│   │   index.html
│   │   ...
│
└───tests
│   │   newsLost v01.ipynb
│   │   newsVSstock v01.ipynb
│
└───zextra
│   │   ...
```