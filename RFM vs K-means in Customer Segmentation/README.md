## Table of contents
* [Introduction](#Introduction)
* [Context](#Context)
* [Business Problem](#Business_Problem)
* [Attribute Information](#Attribute_Information)
* [Task Details](#Task_Details)

![image](https://user-images.githubusercontent.com/83332641/161737124-7065934a-8608-4352-9867-907e987b4079.png)

## Introduction

Identification of customers based on their choices and other behaviors is an important strategy in any organization. This identification may help in approaching customers with specific offers and products. An organization with a large number of customers may experience difficulty in identifying and placing into a record each customer individually. A huge amount of data processing and automated techniques are involved in extracting insights from the large information collected on customers.

There are various methods of customer segmentation. In this notebook we will focus on the segmentation of customers using two clustering techniques – K-Means clustering and RFM. We will see the result of clustering when we implement these techniques in Python. Finally, we will discuss the comparison between these two clustering techniques.

These are the metrics that will be considered for both techniques.

**Recency** How recently did the customer purchase? Highest score refers to the customer with the nearest last shopping date

**Frequency** How often do they purchase?Total number of purchases. this value can be the number of Invoices or the number of products in an invoice or the number of website visits. In other words, it can be not only purchasing the product, but also using the service.

**Monetary Value** How much do they spend?

## Context 

The dataset named Online Retail II was obtained from a UK-based online store and includes sales from 01/12/2009 to 09/12/2011.  
This company sells souvenirs and most of their customers are also wholesalers. Within the scope of this study, only 2010-2011 sales will be consedered.

## Business Problem

Rule-based customer segmentation method RFM and machine learning method K-Means will be compared for customer segmentation.

## Task Details

* Data Preprocessing
* Customer Segmentation with RFM
* Customer Segmentation with K-Means
* Comparison

## Attribute Information:

**InvoiceNo:** Invoice number. The unique number of each transaction, that is, the invoice. Aborted operation if it starts with C.  
**StockCode:** Product code. Unique number for each product.  
**Description:** Product name  
**Quantity:** Number of products. It expresses how many of the products on the invoices have been sold.  
**InvoiceDate:** Invoice date and time.  
**UnitPrice:** Product price (in GBP)  
**CustomerID:** Unique customer number  
**Country:** Country name. Country where the customer lives.
