# Assignment: Click Through Rate Prediction

An assignment for practical and production machine learning.

--------------------------
#### Directions for use

- Fork this repo.
- Version control your progress in your personal repository.
- Add your documentation to the docs directory.
- When you are ready, let us see and add our github user to your repository.

-----------------------

## Background

Marketplaces are a vital part of the free commerce eco-system. Historically, they were physical markets. More recently they have been known as classifieds and in present day, digital platforms for supporting the exchange of products and services for money. Fundamentally, we bring buyers to sellers.

Buyers visit our site in search of products and services. Sellers advertise their products and services. And when the buyer finds something they like, they click on the advertisement and show interest. This is known as a click through.

Click Through Rate (CTR) Prediction is a powerful tool for marketplaces, as a means to deliver even more value for sellers on our platform.

## Problem Statement

Build a Click Trough Rate (CTR) Prediction ML service.

You are provided with data representing a client site's products database. You are required to design a proof of concept, for a ML service where models predictions must be provided to client sites through an API.

### Tasks

- Simple Explaination of production system with flow diagrams.
- Training script (prepare, train, evaluate model).
- Serving script (serving model on localhost).
- Exploratory Analysis of model performance.

### Additional Tips

- Light explainations in the form of README are encouraged.
- Feel free to make assumptions, as long as you document them.
- Python code is expected.
- Do not persist your model. Your training script should create a model given provided data.
- Make your work portable. We may test it on Linux or Windows.
- More points are given for successfully modelling and explaining your model.

## Data

You are provided with a single train dataset. Which you can use as required to satisfy the project requirements.

#### Get Data

A link or set of links will be provided which will allow you to download the dataset.

Options to download data:
1. Navigate to link in your browser and download the contents into a file.
2. Use `wget` utility to download the contents.

For ease of use, a `make` command is provided here in `Makefile` which can streamline this process.
Run the following command on a PC or VM with `wget` installed:

```
    make download-data file=<dataset/to/download> url=<url/to/dataset>
```

#### Features

| Field Name | Description |
|--|--|
| id | listing Identifier for each listing advertisement |
| unix_timestamp | time when click event occured. |
| ui_component_position | Position on device where listing advertisement was displayed. |
| site_id | partner sites where ad was shown. |
| site_domain | domain/country where partner site operates in. |
| site_category | | 
| app_id | special identifier for app used |
| app_domain | |
| app_category | |
| device_id | special identifier for device used |
| device_ip | |
|device_model | |
| device_type | |
| device_conn_type | type of network connection used by device |
| f0-f8 | anonymized categorical variables |
| click | Target variable (0/1). Where 1 - clicked, 0 - not clicked |

**We're Rooting for you** :+1:

![We are rooting for you.](images/rooting4you.webp)
