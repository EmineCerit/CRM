# Customer Segmentation with RFM Analyse

![image](https://user-images.githubusercontent.com/83332641/161731504-75f4a765-0e68-4abb-863a-79539403d75e.png)

## Table of contents
* [Introduction](#Introduction)
* [Context](#Context)
* [Business Problem](#Business_Problem)
* [Task Details](#Task_Details)
* [Attribute Information](#Attribute_Information)

## Introduction

Customer segmentation is the division of customers into groups based on common characteristics in order to increase sales through personalized content tailored to the respective segment.

There are various methods of customer segmentation, including clustering, RFM segmentation and predictive models.In this notebook we will focus on customer segmentation with RFM. The “RFM” in RFM analysis stands for recency, frequency and monetary value. These are the metrics that will be considered.

**Recency :** How recently did the customer purchase? Highest score refers to the customer with the nearest last shopping date

**Frequency :** How often do they purchase?Total number of purchases. this value can be the number of Invoices or the number of products in an invoice or the number of website visits. In other words, it can be not only purchasing the product, but also using the service.

**Monetary Value :** How much do they spend?

## Context  
The dataset named Online Retail II was obtained from a UK-based online store and includes sales from 01/12/2009 to 09/12/2011.

This company sells souvenirs and most of their customers are also wholesalers. Within the scope of this study, only 2010-2011 sales will be consedered.

## Business Problem  
Our aim is to apply RFM analysis to the online retail II dataset and to include customers with common behaviors in the same groups and segment them to develop special sales and marketing techniques for these groups.

The company believes that marketing activities specific to customer segments with common behaviors will increase revenue. For example, it is desired to organize different campaigns for new customers and different campaigns to retain customers, which are very profitable for the company.

## Task Details
* Data Preprocessing
* Calculating RFM Metrics
* Calculating RFM Scores
* Creating RFM Segments

## Attribute Information:
**InvoiceNo:** Invoice number. The unique number of each transaction, that is, the invoice. Aborted operation if it starts with C.  
**StockCode:** Product code. Unique number for each product.  
**Description:** Product name  
**Quantity:** Number of products. It expresses how many of the products on the invoices have been sold.  
**InvoiceDate:** Invoice date and time.  
**UnitPrice:** Product price (in GBP)  
**CustomerID:** Unique customer number  
**Country:** Country name. Country where the customer lives.  
