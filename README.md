# RBI-FSR-Sentiment-Analysis
A sentiment analysis project on the Reserve Bank of India Financial Stability Report (FSR). Using a dictionary-based approach, the project extracts positive and negative words from FSR documents, calculates a sentiment index, and analyzes its relationship with key macroeconomic indicators such as GDP growth, NPA, credit growth, and deposit growth.
Sentiment Analysis of RBI Financial Stability Report
# Project Overview
- This project analyzes the Reserve Bank of India’s Financial Stability Report (FSR) using sentiment analysis techniques.
- The main objective is to measure the sentiment expressed in FSR documents and study its relationship with macroeconomic indicators.
# Methodology
1.	Data Collection: Extracted RBI FSR PDFs (June & December editions).
2.	Dictionary Approach: Used an Excel file containing positive & negative words.
3.	Text Processing:
  o	Converted PDFs to text
  o	Tokenized words
  o	Counted positive, negative, and total words
4.	Sentiment Index Calculation: The sentiment index is calculated using a dictionary-based approach. Each word in the Financial Stability Report (FSR) is compared with a predefined list of positive and negative words.
The formula used is:
       <img width="630" height="77" alt="formula" src="https://github.com/user-attachments/assets/fda12f4c-7656-4573-b252-e25ecfafb1cd" />
      
        •	Positive Words → Words indicating optimism, growth, or stability
        
        •	Negative Words → Words indicating risk, stress, or instability
        
        •	Total Words → All valid words in the document after preprocessing
  
5.	Analysis:

        •	Time series of sentiment index
      
        •	Correlation with GDP growth, NPA, credit growth, deposit growth
      
        •	Granger causality with global indicators (VIX & SRISK)


