# Mug Material Classification (Hierarchical Clustering and Self-Training)

This repository provides the implementation of Hierarchical Clustering and Self-Training algorithms. The implementation is performed on a dataset containing features of three types of mugs (height, diameter, weight, and hue).

## Getting Started

### Prerequisites

- Python 3.7 or later
- numpy
- matplotlib
- pandas

## Data

The data directory should contain two csv files:

- `dataset.csv`: The dataset, including given columns

| Height | Diameter | Weight | Hue | Type |
| --- | --- | --- | --- | --- |

## Project Description

The project is divided into two parts:

1. Hierarchical Agglomerative Clustering: Implement hierarchical agglomerative clustering for an unlabeled dataset of three types of mugs. The implementation allows the option to use single (minimum) linkage, and complete (maximum) linkage. The clusters are evaluated for their ability to reflect the type of mug using the original data labels.
2. Self-Training: Implement a self-training system using a K-nearest neighbor classifier. The labeled data consists of the first 10 data items from each class, while the remaining data items are treated as unlabeled data. The self-training algorithm allows to change the number of data items that are being added to the labeled data set in each iteration.

## Results

The purity of the clusters formed by the Hierarchical Agglomerative Clustering algorithm and the accuracy of the classifier developed by the self-training system are displayed in the code cells
