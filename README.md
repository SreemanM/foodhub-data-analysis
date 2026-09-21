# FoodHub Order Data Analysis

## Project Overview

This project analyzes order data from **FoodHub**, an online food delivery platform serving customers in New York. The goal is to understand customer ordering behavior, restaurant performance, cuisine preferences, delivery performance, ratings, and revenue-related patterns so that the business can make data-driven decisions.

The analysis was completed in Python using a Jupyter/Google Colab notebook and includes data cleaning, exploratory data analysis, business-oriented questions, visualizations, and actionable recommendations.

## Business Context

FoodHub connects customers with restaurants through an online food delivery platform. As the number of restaurants and delivery orders grows, the business needs to understand:

- Which restaurants and cuisines receive the most orders
- Customer ordering patterns across weekdays and weekends
- Order cost and revenue opportunities
- Food preparation and delivery performance
- Restaurant ratings and customer feedback
- Which restaurants may qualify for promotional campaigns

## Dataset

The dataset used in this project is `foodhub_order.csv`.

It contains **1,898 orders and 9 variables**:

| Column | Description |
|---|---|
| `order_id` | Unique identifier for each order |
| `customer_id` | Unique identifier for each customer |
| `restaurant_name` | Name of the restaurant |
| `cuisine_type` | Cuisine category |
| `cost_of_the_order` | Cost of the order |
| `day_of_the_week` | Whether the order was placed on a weekday or weekend |
| `rating` | Customer rating for the order |
| `food_preparation_time` | Time taken by the restaurant to prepare the food |
| `delivery_time` | Time taken to deliver the order |

## Key Analysis Performed

The notebook covers:

- Dataset structure, dimensions, and data types
- Missing-value handling
- Univariate analysis of important variables
- Restaurant and cuisine popularity
- Weekend vs weekday ordering patterns
- High-value order analysis
- Delivery-time analysis
- Customer ordering frequency
- Restaurant rating analysis
- Promotional eligibility analysis
- Revenue estimation based on commission rules
- End-to-end delivery-time analysis
- Business conclusions and recommendations

## Key Findings

Some of the important findings from the analysis are:

- The dataset contains **1,898 orders**.
- **American cuisine** is the most popular cuisine on weekends.
- Approximately **29.24% of orders cost more than $20**.
- Average delivery time is approximately **24.16 minutes**.
- Weekday delivery is slower than weekend delivery by roughly **5.87 minutes** on average.
- Approximately **10.54% of orders take more than 60 minutes** when food preparation and delivery times are combined.
- A large number of orders are unrated, which limits feedback-driven analysis.
- Several high-volume, highly rated restaurants qualify for promotional campaigns.
- Estimated net revenue under the provided commission rules is approximately **$6,166.30**.

## Business Recommendations

- Focus marketing campaigns on **weekends**, when order volume is highest.
- Improve **weekday delivery operations** through better driver allocation, routing, and pickup coordination.
- Promote consistently high-rated and high-volume restaurants more prominently in the application.
- Encourage more customers to leave ratings through reminders or small incentives.
- Continue investing in popular cuisines such as **American, Japanese, Italian, and Chinese**, while also promoting high-rated niche cuisines.
- Use high-value orders and customer-ordering frequency to design loyalty and targeted promotion programs.

## Repository Structure

```text
FoodHub/
├── FoodHub_Data_Analysis.ipynb
├── foodhub_order.csv
├── requirements.txt
└── README.md
```

## Technologies Used

- Python
- NumPy
- pandas
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab

## How to Run the Project

### Option 1: Google Colab

1. Clone this repository or download it as a ZIP file.
2. Upload `FoodHub_Data_Analysis.ipynb` and `foodhub_order.csv` to the same folder in Google Drive, or upload both directly to Colab.
3. Open the notebook in Google Colab.
4. Run the package-installation cell if required.
5. Restart the runtime if Colab asks you to do so.
6. Run all notebook cells sequentially.

If the notebook cannot find the CSV file automatically, update the dataset path to the location where you stored `foodhub_order.csv`.

### Option 2: Run Locally

#### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/foodhub-data-analysis.git
cd foodhub-data-analysis
```

#### 2. Create a virtual environment

Windows:

```bash
python -m venv venv
venv\Scripts\activate
```

macOS/Linux:

```bash
python3 -m venv venv
source venv/bin/activate
```

#### 3. Install the required packages

```bash
pip install -r requirements.txt
```

#### 4. Start Jupyter Notebook

```bash
jupyter notebook
```

Open:

```text
FoodHub_Data_Analysis.ipynb
```

and run the cells from top to bottom.

## Install Dependencies Directly

If you do not want to use `requirements.txt`, install the main libraries with:

```bash
pip install numpy pandas matplotlib seaborn jupyter
```

## Notes

- Keep `foodhub_order.csv` in the same directory as the notebook for the simplest setup.
- The notebook contains both code and written business observations.
- Results may vary slightly if package versions differ from those originally used.

## Author

**Sreeman Mandava**

This project was completed as part of an applied data science / machine learning course portfolio.
