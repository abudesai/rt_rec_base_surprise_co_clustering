Co-Clustering algorithm built in Scikit-Surprise for Recommender - Base problem category as per Ready Tensor specifications.

- sklearn
- Scikit-Surprise
- python
- pandas
- numpy
- scikit-optimize
- flask
- nginx
- uvicorn
- docker
- recommender system

This is a collaborative filtering algorithm based on co-clustering. See:
Thomas George and Srujana Merugu. A scalable collaborative filtering framework based on co-clustering. 2005.

The data preprocessing step includes indexing and standardization. Numerical values (ratings) are also scaled to [0,1] using min-max scaling.

During the model development process, the algorithm was trained and evaluated on a variety of datasets such as jester, anime, book-crossing, modcloth, amazon electronics, and movies.

This Recommender System is written using Python as its programming language. ScikitLearn-Surprise and ScikitLearn is used to implement the main algorithm, evaluate the model, and preprocess the data. Numpy, pandas, and feature_engine are used for the data preprocessing steps. SciKit-Optimize was used to handle the HPT. Flask + Nginx + gunicorn are used to provide web service which includes two endpoints- /ping for health check and /infer for predictions in real time.

Surprise library attribution:
@article{Hug2020,
doi = {10.21105/joss.02174},
url = {https://doi.org/10.21105/joss.02174},
year = {2020},
publisher = {The Open Journal},
volume = {5},
number = {52},
pages = {2174},
author = {Nicolas Hug},
title = {Surprise: A Python library for recommender systems},
journal = {Journal of Open Source Software}
}
