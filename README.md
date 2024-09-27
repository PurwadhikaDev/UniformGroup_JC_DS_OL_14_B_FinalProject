# README

## CHAPTER 1: BUSINESS CONCEPT

### Company Overview
Olist is a technology company from Brazil operating in the e-commerce sector. Founded in 2015, Olist offers a SaaS (Software as a Service) platform that enables small and medium-sized businesses to sell their products online without the need to build a complex e-commerce infrastructure from scratch. Olist acts as an intermediary between sellers and buyers, providing various services such as order management, payments, logistics, and customer service.

As an online marketplace, Olist differentiates itself from competitors by focusing on seller reputation, strategic product placement, and a dedicated team supporting sales and customer service. Olist’s platform accelerates the onboarding process for new sellers, allowing them to start selling their products online quickly. This innovative business model has attracted many sellers in Brazil and established Olist as a key player in the country’s e-commerce industry.

### Introduction

#### Introduction to E-commerce
E-commerce, or electronic commerce, refers to the buying and selling of goods or services using the internet, along with the transfer of money and data to execute these transactions. It has revolutionized the retail landscape by enabling digital transactions between consumers and businesses. The growth of e-commerce has been driven by its convenience, speed, and broad range of products and services, making it a crucial component of modern trade.

#### Understanding the Marketplace Model
The marketplace model stands out within the e-commerce industry. A marketplace is an e-commerce site where product or service information is provided by multiple third parties, while transactions are processed by the marketplace operator. This model facilitates a vast network of buyers and sellers, fostering competitive prices and a diverse array of products. Notable examples include Amazon, eBay, and Alibaba, which have integrated countless small businesses into their platforms, offering customers a comprehensive shopping experience.

#### Olist: Pioneering E-commerce in Brazil
Olist connects small businesses across Brazil to major e-commerce platforms, providing merchants with a broader audience and streamlined logistics. By aggregating various sellers from numerous categories, Olist ensures that even smaller vendors can benefit from the scale and reach that large e-commerce platforms provide. This approach democratizes access to digital sales channels, enhancing product variety and competitiveness within the marketplace.

#### The Importance of Predicting Delivery Delays
In e-commerce, the efficiency of supply chain operations, particularly delivery times, plays a crucial role in shaping customer satisfaction and driving business success. Predicting delivery delays allows companies to manage customer expectations effectively by providing timely updates and improving transparency. This builds trust and strengthens customer loyalty. Additionally, anticipating delays helps businesses optimize logistics and distribution processes, ensuring smooth operations while reducing unnecessary costs. In a highly competitive market, consistently meeting or exceeding delivery expectations can provide a significant edge. Overall, predicting delivery delays enhances customer experience and improves operational efficiency and profitability.

### Problem Statement
Olist faces significant challenges related to delivery delays, which negatively impact both seller credibility and customer satisfaction. These delays erode customer trust and harm the marketplace's reputation, leading to lower retention rates and potentially reduced profitability. As Olist continues to grow, accurately predicting and managing delivery delays becomes critical for enhancing operational efficiency, improving customer relations, and sustaining a competitive edge. By integrating advanced predictive analytics into its operations, Olist can anticipate and mitigate potential delays, ensuring reliable service delivery and optimizing supply chain management.

### Stakeholders
1. Management Logistics of Olist

### Goals
1. Predict if an order would be delayed.
2. Identify key factors that contribute to delivery delays.

### Target & Metrics

#### Recall
Recall is a metric that indicates how well a model identifies positive instances, calculated using the formula:

Recall = TP / (TP + FN)

Where:
- **TP (True Positives)**: The number of correctly predicted positive instances.
- **FN (False Negatives)**: The number of actual positive instances incorrectly predicted as negative.

A high recall means we capture a significant portion of actual delayed orders, minimizing false negatives.

#### Precision
Precision measures the accuracy of the positive predictions made by the model, defined as:

Precision = TP / (TP + FP)

Where:
- **FP (False Positives)**: The number of actual negative instances incorrectly predicted as positive.

A high precision indicates that when the model predicts an order is delayed, it is likely correct.

### False Negatives and False Positives
- **False Negative**: This occurs when orders are predicted to be on time but are actually delayed, which can lead to lower rating scores and reduced customer satisfaction.
- **False Positive**: This happens when orders are predicted to be delayed but are actually on time. While this creates unnecessary concern, it is generally less damaging than false negatives.

### Why Focus on Recall?
Focusing on recall is critical in our context because capturing as many true positives as possible is essential. Since false negatives significantly impact customer perception and satisfaction, it is imperative to minimize their occurrence. By prioritizing recall, we ensure most delayed orders are correctly identified, enhancing customer trust and product ratings.

### Estimating Losses
To estimate potential losses incurred from false negatives, we can compare the raw losses to the actual price of the delayed orders. Analyzing the impact of missed delayed orders helps us understand the financial implications and the importance of our predictive model.

### Analytic Approach EDA
- Investigate if delays cause rating declines.
- Explore delivery delays per product category.
- Analyze order status distribution.
- Examine the impact of payment type on delivery.
- Assess the correlation between product dimensions and freight value.
- Analyze delays over time.
