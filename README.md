# 🚗 Automobile Market Analytics Dashboard

A complete end-to-end data analytics project exploring the automobile market through exploratory data analysis (EDA) and an interactive Power BI dashboard. The project uncovers pricing trends, performance patterns, and market segmentation across 21 car brands.



## Project Overview

This project analyzes a real-world automobile dataset to answer key business questions around pricing, performance, and market positioning. The workflow covers data cleaning, exploratory analysis using Python, and building a business-ready interactive dashboard in Power BI.

**Core Questions Explored:**
- What factors drive automobile pricing?
- How do brands compare across price, performance, and fuel efficiency?
- What are the tradeoffs between engine type, body style, and fuel economy?
- Which segments dominate the market?

---

## Dataset Description

| Attribute | Details |
|-----------|---------|
| File | `Automobile.csv` |
| Records | 193 automobiles |
| Features | 25 columns |
| Missing Values | None |
| Target Variable | `price` |

### Feature Categories

**Identity & Classification**
| Column | Description |
|--------|-------------|
| `make` | Brand / manufacturer (21 unique) |
| `fuel_type` | Gas or Diesel |
| `aspiration` | Standard or Turbocharged |
| `num_of_doors` | 2 or 4 doors |
| `body_style` | Sedan, Hatchback, Wagon, Hardtop, Convertible |
| `drive_wheels` | FWD, RWD, 4WD |
| `engine_location` | Front or Rear |
| `symboling` | Insurance risk rating (−2 to +3) |

**Physical Dimensions**
| Column | Description |
|--------|-------------|
| `wheel_base` | Distance between axles (inches) |
| `length`, `width`, `height` | Car dimensions (inches) |
| `curb_weight` | Weight without passengers/cargo (lbs) |

**Engine & Performance**
| Column | Description |
|--------|-------------|
| `engine_type` | OHC, OHV, DOHC, etc. |
| `num_of_cylinders` | Cylinder count (3–12) |
| `engine_size` | Engine displacement (cc) |
| `fuel_system` | Fuel injection system type |
| `bore`, `stroke` | Engine bore and stroke dimensions |
| `compression_ratio` | Engine compression ratio |
| `horsepower` | Engine power output |
| `peak_rpm` | RPM at peak power |
| `city_mpg`, `highway_mpg` | Fuel efficiency ratings |
| `price` | Vehicle price in USD |



## Project Structure

```
automobile-analytics/
│
├── data/
│   └── Automobile.csv          # Raw dataset
│
├── screenshots/
│   └── Automobile_dashboard.png               # Exploratory Data Analysis dashboard
│
├── reports/
│   └── Automobile_Analysis_Dashboard.pbix   # Power BI dashboard file
│
└── README.md
```

---

## Key Insights

### 💰 Pricing
- Price ranges from **$5,118 to $45,400**, with an average of **$13,285**
- **Jaguar** ($34,600 avg), **Mercedes-Benz** ($33,647 avg), and **Porsche** ($31,400 avg) are the most expensive brands
- **Diesel vehicles** cost ~24% more than gas-powered equivalents on average, despite making up only 10% of the dataset

### 🏎️ Performance
- **Hardtops** (142 hp avg) and **convertibles** (132 hp avg) deliver the most power, far above sedans (104 hp) and hatchbacks (97 hp)
- **Turbocharged engines** produce more power but at the cost of fuel efficiency — averaging 3–4 MPG less than standard aspiration engines in both city and highway driving

### 📊 Market Distribution
- **Toyota** is the most represented brand with 32 models, followed by Nissan (18) and Honda/Mitsubishi (13 each)
- **Sedans** (92 cars) and **hatchbacks** (63 cars) dominate, making up over 80% of the dataset
- **Front-wheel drive** (FWD) is the most common drivetrain at 59%, while rear-wheel drive (RWD) dominates the premium segment

### ⚙️ Engine & Risk
- Most cars carry a **symboling (risk) score of 0 or 1** — moderate risk; only 23 carry the highest rating of +3
- **OHC engine type** is the most common (141 out of 193), and **MPFI fuel system** leads at 88 vehicles
- Average engine output is **103 hp** with a peak RPM of **5,099**

---

## Dashboard Highlights

The Power BI dashboard provides an interactive view of the dataset with the following pages / visuals:

- **Market Overview** — total records, brand count, price range, and body style breakdown
- **Brand Comparison** — average price, horsepower, and MPG by manufacturer
- **Price Analysis** — pricing distribution by fuel type, aspiration, drive wheels, and body style
- **Performance vs Efficiency** — horsepower vs city/highway MPG scatter analysis
- **Risk Rating Distribution** — symboling score breakdown across brands and body styles

---

### Viewing the Dashboard

Open `./screenshots/Automobile_dashboard.png` in **Power BI Desktop**.


## Results & Findings

| Metric | Value |
|--------|-------|
| Total Automobiles | 193 |
| Unique Brands | 21 |
| Features Analyzed | 25 |
| Missing Values | 0 |
| Avg Price | $13,285 |
| Avg Horsepower | 103 hp |
| Avg City MPG | 25.3 |
| Avg Highway MPG | 30.8 |
| Most Common Brand | Toyota (32 cars) |
| Most Common Body Style | Sedan (92 cars) |
| Most Common Drivetrain | FWD (59%) |

> ⭐ If you found this project useful, feel free to star the repository and share your feedback!
