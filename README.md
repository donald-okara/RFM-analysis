# RFM Analysis with Python

RFM (Recency, Frequency, Monetary) analysis is a valuable technique for customer segmentation and understanding customer behavior. This README provides instructions on how to conduct an RFM analysis using Python with sample data.


## Requirements
To run this RFM analysis, you need the following:
- Python (3.x recommended)
- Pandas library (`pip install pandas`)
- datetime library (usually included with Python)

## Usage
1. Clone or download this repository to your local machine.
2. Prepare your customer transaction data in a CSV file, similar to the provided `RFM.csv`.
3. Update the data file path in the Python script if necessary.
4. Run the Python script.

## Steps
Here are the steps to conduct the RFM analysis:

### 1. Import Libraries
```python
import pandas as pd
import datetime as dt
```

### 2. Load Data
Load your customer transaction data into a DataFrame.

### 3. Data Preprocessing
- Convert the 'PurchaseDate' column to a datetime format.
- Calculate the total monetary value for each customer.

### 4. Calculate Recency
- Calculate the most recent purchase date.
- Calculate the number of days since the most recent purchase for each customer.

### 5. Calculate Frequency
- Count the number of transactions for each customer.

### 6. Merge DataFrames
Combine the Recency, Frequency, and Monetary DataFrames into one.

### 7. RFM Scoring
- Create quartiles for Recency, Frequency, and Monetary columns to score customers.

### 8. Calculate RFM Score
Combine the individual R, F, and M scores to create an RFM score.

## RFM Scoring
The RFM scoring assigns scores to each customer based on quartiles. The higher the score, the better the customer's RFM value for that category.

- Recency (R): 4 - Best, 1 - Worst
- Frequency (F): 1 - Worst, 4 - Best
- Monetary (M): 1 - Worst, 4 - Best

## Output
After running the script, you'll have an RFM score for each customer, which can be used for customer segmentation and marketing strategies.

Feel free to customize the script and adapt it to your specific data and requirements.
