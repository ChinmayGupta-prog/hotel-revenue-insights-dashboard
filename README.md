# Hotel Revenue Insights Dashboard

This project analyzes hotel revenue and booking data using Python, Pandas, and MySQL. It includes CSV datasets, a Jupyter Notebook for loading and processing data, and a dashboard preview image.

## Project Overview

The objective of this project is to understand hotel revenue performance using booking-related datasets. The analysis uses multiple dimension and fact tables such as hotels, rooms, dates, bookings, and aggregated bookings.

## Dataset Files

The project contains the following datasets inside the `data/` folder:

- `dim_date.csv`
- `dim_hotels.csv`
- `dim_rooms.csv`
- `fact_aggregated_bookings.csv`
- `fact_bookings.csv`

## Tools and Technologies Used

- Python
- Pandas
- SQLAlchemy
- PyMySQL
- MySQL
- Jupyter Notebook

## Project Structure

```text
Hotel_Revenue_Insights_Dashboard/
│
├── data/
│   ├── dim_date.csv
│   ├── dim_hotels.csv
│   ├── dim_rooms.csv
│   ├── fact_aggregated_bookings.csv
│   └── fact_bookings.csv
│
├── dashboard.jpg
├── main.ipynb
├── requirements.txt
├── .gitignore
└── README.md
```

## How to Run This Project

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/hotel-revenue-insights-dashboard.git
cd hotel-revenue-insights-dashboard
```

### 2. Create a virtual environment

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

### 3. Install required libraries

```bash
pip install -r requirements.txt
```

### 4. Open the Jupyter Notebook

```bash
jupyter notebook main.ipynb
```

### 5. MySQL Setup

The notebook uses MySQL through SQLAlchemy and PyMySQL. Create a MySQL database named:

```sql
CREATE DATABASE hotelRevenueDataBase;
```

Update the username, password, and database name in the notebook if needed:

```python
engine = create_engine("mysql+pymysql://{user}:{pw}@localhost:3306/{db}".format(
    user='root',
    pw='root',
    db='hotelRevenueDataBase'
))
```

## Dashboard Preview

![Dashboard Preview](dashboard.jpg)

## Note

The original project contained a local virtual environment folder named `hotelVenv`. It is intentionally excluded from this GitHub version because virtual environments should not be uploaded to GitHub. Dependencies are listed in `requirements.txt` instead.
