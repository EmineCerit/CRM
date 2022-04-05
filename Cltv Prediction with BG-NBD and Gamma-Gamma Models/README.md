
# CLTV PREDICTION WITH BG/NBD AND GAMMA&GAMMA MODELS

## Table of contents
* [Introduction](#Introduction)
* [Context](#Context)
* [Business Problem](#Business_Problem)
* [Task Details](#Task_Details)
* [Attribute Information](#Attribute_Information)

<a id="Introduction"></a>
## Introduction
**What is CLTV (Customer Life Time Value)?**  
Customer lifetime value (CLTV), represents the total amount of money a customer is expected to spend in your business, or on your products, during their lifetime.

Focusing on CLTV helps you design an efficient strategy with concise budget planning. However, some customers bring your business more value than the others. That’s why it’s crucial to know which ones you should focus on first and invest in.

With CLTV calculation, you can take a picture of today, but with CLTV prediction, you make time projections such as 3 months, 1 year.

![image](https://user-images.githubusercontent.com/83332641/161739393-59dac255-ea17-4723-8b18-2de051864dbc.png)


**BG/NBD (Beta Geometric / Negative Binomial Distribution) Model** will model each customer’s purchase behaviours’ distribution and will predict the expected number of transactions for each customer. It is also known as “Buy Till You Die” Model.

BG/NBD model, models 2 processes as

**Transaction Process (Buy)**
During the customer is alive, the number of will have made by the customer, will be distributed poison by transaction rate parameter  
During the customer is alive, they will be purchasing around their own transaction rate  
Transaction rates will change for each customer and they will be distributed gamma (r,α)

**Dropout Process (Till You Die)**
Each customer has their own dropout rate by p probability  
The customer will be a dropout by p probability  
Dropout rates will change for each customer and they will be distributed beta (a,b) for the mass

**Gamma-Gamma Submodel** will model the expected average profit distribution and will predict the expected average profit for each customer.

<a id="Context"></a>
## Context

The dataset named Online Retail II was obtained from a UK-based online store and includes sales from 01/12/2009 to 09/12/2011.

This company sells souvenirs and most of their customers are also wholesalers. Within the scope of this study, only 2010-2011 sales will be consedered.

<a id="Business_Problem"></a>
## Business Problem

Our aim is to identify the customers who can generate the most revenue within the 6-month time period.

<a id="Task_Details"></a>
## Task Details

* Importing Libraries and Data
* Data Preprocessing
* Preparation of CLTV Data Structure
* Establishing the BG-NBD Model
* Establishing the Gamma Gamma Model
* Calculation of CLTV with BG-NBD and GG model.

<a id="Attribute_Information"></a>
## Attribute Information:

**InvoiceNo:** Invoice number. The unique number of each transaction, that is, the invoice. Aborted operation if it starts with C.  
**StockCode:** Product code. Unique number for each product.  
**Description:** Product name  
**Quantity:** Number of products. It expresses how many of the products on the invoices have been sold.  
**InvoiceDate:** Invoice date and time.  
**UnitPrice:** Product price (in GBP)  
**CustomerID:** Unique customer number  
**Country:** Country name. Country where the customer lives.
