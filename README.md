# Sentiment Analysis of RBI Financial Stability Report

## Project Overview
This project analyzes the **Reserve Bank of India’s Financial Stability Report (FSR)** using **sentiment analysis techniques**.  
The main objective is to measure the sentiment expressed in FSR documents and study its relationship with macroeconomic indicators.

## Methodology
1. **Data Collection**: Extracted RBI FSR PDFs (June & December editions).
2. **Dictionary Approach**: Used an Excel file containing positive & negative words.
3. **Text Processing**: 
   - Converted PDFs to text
   - Tokenized words
   - Counted positive, negative, and total words
4. **Sentiment Index Calculation**:
   The sentiment index is calculated using a dictionary-based approach. Each word in the Financial Stability Report (FSR) is compared with a predefined list of positive and negative words.
   
   The formula used is:

<img width="630" height="77" alt="formula" src="https://github.com/user-attachments/assets/4fe9eb77-aba8-4e73-b8f2-a3710e7b7b0b" />

   
- Positive Words → Words indicating optimism, growth, or stability

- Negative Words → Words indicating risk, stress, or instability

- Total Words → All valid words in the document after preprocessing
  
5. **Analysis**:
- Time series of sentiment index
- Correlation with GDP growth, NPA, credit growth, deposit growth
- Granger causality with global indicators (VIX & SRISK)

## Output
The output is stored in a CSV file containing:
- Total Negative Words
- Total Positive Words
- Total Words
- Sentiment Index

## Tools & Libraries
- Python (Jupyter Notebook)
- Libraries - pandas / numpy / PyPDF2 / pdfplumber / matplotlib / seaborn
- Excel for correlation analysis

## Repository Structure

RBI-FSR-Sentiment-Analysis/

**│── data/**

    └── fsr_pdfs/              # Folder for RBI FSR PDFs
    
    └── positive_negative.xlsx     # Dictionary file of positive & negative words


**│── notebooks/**

    └── sentiment_analysis.ipynb   # Jupyter notebook with main code
    

**│── output/**

    └── sentiment_index.csv    # Final results
    
    └── graphs/sentiment analysis_graph sentiment   # Visualizations, correlation plots
    
**│──srisk.xlsx**        # srisk data and output plot with graph

**│──visk.xlsx**          # visk data

**│──granger causality test**

    └──granger.xlsx    # Data for Granger causality test
    
    └──granger.ipynb    # Code for granger causality test
    
    └──granger_analysis_result.xlsx    # Output and graph


