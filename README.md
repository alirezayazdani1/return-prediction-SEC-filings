# return-prediction-SEC-filings

This is a short tutorial on processing SEC-10K filing data to generate document embeddings, which in turn, can be used as sginals for predicting companies' returns post-filing date.

The process is presented in three steps using three separate notebooks:
1. `01_SEC_10k_embedding.ipynb` parses 4 sections of SEC filings, preprocesses the data and generate document embeddings using two different neural network models.
2. `02_stock_price_data.ipynb` downloads companies price data that are publicly available for a certain period of time and generates return data for those companies.
3. `03_SEC_predict_return.ipynb` trains a gradient boosting model using document vectors produced in the first notebook to predict returns post-filing date.
