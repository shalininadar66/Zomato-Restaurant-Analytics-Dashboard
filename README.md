# Zomato Restaurant Analytics Dashboard

A Power BI dashboard for exploring and analyzing restaurant data using interactive filters, KPI cards, charts, a scatter plot, and a geographic map.

The dashboard is designed as a two-page analytical report with a clean light theme and a consistent red visual style.

## Dashboard Preview

### Page 1 — Zomato Restaurant Analytics

![Page 1 - Zomato Restaurant Analytics](page-1-dashboard.png)

### Page 2 — Ratings and Cost Deep Dive

![Page 2 - Ratings and Cost Deep Dive](page-2-dashboard.png)

## Project Overview

The Zomato Restaurant Analytics Dashboard provides an interactive view of restaurant information such as:

- Restaurant count
- Average restaurant rating
- Average cost for two
- Total votes
- Top cities by restaurant count
- Price-range distribution
- Restaurant geographic locations
- Top cuisines
- Average rating by price range
- Relationship between votes and ratings
- Average cost across top cities
- Online delivery availability
- Table booking availability

The dashboard contains two pages so that high-level restaurant information and deeper rating/cost analysis can be viewed separately.

## Dashboard Pages

### Page 1 — Zomato Restaurant Analytics

The first page provides an overview of the restaurant dataset.

**KPI Cards**
- Total Restaurants
- Avg Rating
- Avg Cost for Two
- Total Votes

**Visuals**
- Top 10 Cities
- Price Range Split
- Restaurant Locations Map
- Top 10 Cuisines

**Filters**
- City
- Price Range
- Online Delivery
- Table Booking

### Page 2 — Ratings and Cost Deep Dive

The second page focuses on restaurant ratings, votes, delivery/booking availability, and cost.

**KPI Cards**
- Avg Votes / Restaurant
- Online Delivery %
- Table Booking %

**Visuals**
- Avg Rating by Price Range
- Votes vs Rating Scatter Plot
- Avg Cost by Top 10 Cities

The filters are synchronized between the two pages.

## Key Metrics

The dashboard uses Power BI measures to calculate metrics dynamically based on the selected filters.

The main metrics include:

| Metric | Dashboard Value |
|---|---:|
| Total Restaurants | 9,551 |
| Average Rating | 2.89 |
| Average Cost for Two | 1.20K |
| Total Votes | Approximately 1.5M |
| Average Votes per Restaurant | 156.91 |
| Online Delivery Availability | 26% |
| Table Booking Availability | 12% |

*Note: Values are based on the dashboard screenshots with the default filters selected. Some values are rounded or visually estimated. The Total Votes KPI should be checked in Power BI because its current display shows 1M, whereas the average votes and restaurant count imply approximately 1.5M.*

## Key Analytical Findings

The dashboard provides several insights into restaurant distribution, pricing, cuisines, ratings, customer engagement, and service availability.

### 1. Restaurant Distribution by City

The Top 10 Cities visualization shows that:

- New Delhi has the highest restaurant representation, with approximately 5,500 restaurants.
- Gurugram and Noida follow, with approximately 1,000–1,100 restaurants each.
- The remaining cities have considerably fewer restaurant records.

**Business Insight:**

The dataset has a strong concentration of restaurants in New Delhi. This means that overall results may be influenced more heavily by restaurants from New Delhi than by smaller cities.

This analysis helps identify cities with a higher concentration of restaurants and understand the geographical distribution of the available data.

### 2. Restaurant Distribution by Price Range

The price-range distribution shows the following results:

| Price Range | Restaurant Count | Percentage |
|---|---:|---:|
| 1 | 4,440 | 46.53% |
| 2 | 3,110 | 32.59% |
| 3 | 1,410 | 14.74% |
| 4 | 590 | 6.14% |

**Key Findings:**

- Price Range 1 accounts for the largest share of restaurants at 46.53%.
- Price Ranges 1 and 2 together represent approximately 79.12% of all restaurants.
- Only 6.14% of restaurants belong to Price Range 4.

**Business Insight:**

The dataset is dominated by restaurants in the lower price categories, indicating that affordable restaurant options have the largest representation.

This information can help businesses understand the pricing distribution of restaurants in the dataset.

### 3. Most Represented Cuisines

The Top 10 Cuisines visualization highlights the following observations:

- North Indian cuisine has the highest representation, with approximately 3,000 restaurant records.
- Chinese cuisine ranks second, with approximately 800 records.
- Fast Food, Bakery and Cafe are also among the highly represented cuisines.
- Other represented cuisines include American, South Indian, Mithai, Street Food and Continental.

**Business Insight:**

North Indian cuisine has significantly greater representation than the other cuisines in the dataset.

This provides an overview of the cuisine mix across the locations covered by the data. However, the number of restaurants does not necessarily indicate customer demand, sales or profitability.

### 4. Relationship Between Price Range and Restaurant Ratings

The average-rating comparison shows an increasing pattern across price categories.

| Price Range | Approximate Average Rating |
|---|---:|
| 1 | 2.4 |
| 2 | 3.1 |
| 3 | 3.7 |
| 4 | 3.9 |

**Key Findings:**

- Price Range 1 has the lowest average rating.
- Price Range 4 has the highest average rating.
- Average ratings increase as the price category increases.

**Business Insight:**

Higher-priced restaurant categories have higher average ratings in the displayed dataset.

This suggests a positive relationship between restaurant price category and average customer ratings. However, it does not establish that higher prices cause better ratings. Other factors, such as food quality, service and restaurant type, may also influence customer ratings.

### 5. Online Delivery and Table Booking Availability

The dashboard shows the following service availability:

| Service | Availability |
|---|---:|
| Online Delivery | 26% |
| Table Booking | 12% |

**Key Findings:**

- Approximately 26% of restaurants offer online delivery.
- Approximately 12% of restaurants offer table booking.
- Online delivery is more commonly available than table booking.

**Business Insight:**

Online delivery has greater representation than table booking among the restaurants analyzed.

This highlights the difference in availability of these two restaurant services and helps understand the service offerings of restaurants in the dataset.

### 6. Average Cost for Two Across Cities

The second dashboard page compares the average cost for two across the selected top 10 cities.

The approximate ranking shown is:

| Rank | City |
|---:|---|
| 1 | Hyderabad |
| 2 | Pune |
| 3 | Jaipur |
| 4 | Kolkata |
| 5 | Bangalore |
| 6 | Goa |
| 7 | Gurugram |
| 8 | New Delhi |
| 9 | Noida |
| 10 | Faridabad |

**Key Findings:**

- Hyderabad has the highest displayed average cost for two, at approximately 1,350.
- Pune and Jaipur follow.
- Faridabad has the lowest displayed average cost among the selected cities, at approximately 450.

**Business Insight:**

The displayed average cost varies considerably across cities. This comparison can help identify differences in restaurant pricing across locations.

**Data Limitation:**

The source dataset contains records from multiple countries and currencies. City-wise cost comparisons should only be interpreted after verifying that the selected cities use a common currency or that currency conversion has been applied.

### 7. Relationship Between Restaurant Votes and Ratings

The scatter plot explores the relationship between the total votes received by restaurants and their average ratings.

**Key Findings:**

- Most restaurants are concentrated in the lower vote-count range.
- Many restaurants have ratings between approximately 3 and 4.5.
- A smaller number of restaurants receive thousands of votes, with some reaching approximately 10,000 votes.
- Restaurants show varying ratings across different vote counts.

**Business Insight:**

Customer engagement, measured through votes, is unevenly distributed across restaurants. A small number of restaurants receive substantially more votes than most others.

The scatter plot helps identify patterns between votes and ratings, but it does not establish a causal relationship between them.

## Key Metrics

The dashboard uses Power BI measures to calculate metrics dynamically based on the selected filters.

Examples include:

- Total number of restaurants
- Average rating
- Average cost for two
- Total votes
- Average votes per restaurant
- Percentage of restaurants offering online delivery
- Percentage of restaurants offering table booking

Because the calculations are dynamic, KPI values and chart results can change when users interact with the filters.

## Dataset

The dashboard was created using a restaurant dataset containing fields such as:

- RestaurantID
- City
- Cuisines
- Price_range
- Has_Online_delivery
- Has_Table_booking
- Votes
- Average_Cost_for_two
- Rating
- Latitude
- Longitude
- Currency

The dataset contains approximately 9,551 restaurant records.

> **Note:** The dataset contains restaurant records from multiple locations, countries and currencies. Currency differences must be considered when comparing restaurant costs. Average cost comparisons across cities should use a common currency or appropriate currency conversion to avoid misleading conclusions.

The analysis reflects the available dataset and should not be treated as a complete representation of the restaurant industry.

## Tools and Technologies

- **Microsoft Power BI Desktop** — dashboard creation, visualization and interactive analysis
- **Microsoft Excel** — source dataset
- **Power Query** — data loading and preparation
- **DAX** — calculated measures and KPI calculations

## Power BI Concepts Used

This project demonstrates the use of:

- KPI/Card visuals
- Slicers
- Clustered column/bar charts
- Donut charts
- Scatter plots
- Map visualization
- Top N filters
- Visual-level filters
- Synchronized slicers
- DAX measures
- Aggregations such as Count, Sum and Average
- Data formatting
- Dashboard layout and visual design

## Important Measures

Examples of the measures used in the dashboard include:

### Total Restaurants

```DAX
Total Restaurants =
DISTINCTCOUNT('Sheet1'[RestaurantID])
```

### Average Rating

```DAX
Avg Rating =
AVERAGE('Sheet1'[Rating])
```

### Average Cost

```DAX
Avg Cost =
AVERAGE('Sheet1'[Average_Cost_for_two])
```

### Total Votes

```DAX
Total Votes =
SUM('Sheet1'[Votes])
```

### Average Votes per Restaurant

```DAX
Avg Votes per Restaurant =
AVERAGE('Sheet1'[Votes])
```

### Online Delivery Percentage

```DAX
Online Delivery % =
DIVIDE(
    CALCULATE(
        DISTINCTCOUNT('Sheet1'[RestaurantID]),
        'Sheet1'[Has_Online_delivery] = "Yes"
    ),
    DISTINCTCOUNT('Sheet1'[RestaurantID])
)
```

### Table Booking Percentage

```DAX
Table Booking % =
DIVIDE(
    CALCULATE(
        DISTINCTCOUNT('Sheet1'[RestaurantID]),
        'Sheet1'[Has_Table_booking] = "Yes"
    ),
    DISTINCTCOUNT('Sheet1'[RestaurantID])
)
```

## Dashboard Design

The dashboard follows a light, minimal visual design.

### Main Colors

| Element | Color |
|---|---|
| Header / primary red | `#B23A3A` |
| Dark red text | `#8F2525` |
| KPI card background | `#FCEAEA` |
| KPI card border | `#F1CACA` |
| Page background | `#F7F8FA` |
| Visual background | `#FFFFFF` |
| Main text | `#1F2937` |

The dashboard intentionally uses a consistent red color family instead of using different colors for different KPI cards.

## How to Use

1. Download or clone this repository.
2. Open the `.pbix` file using **Power BI Desktop**.
3. If Power BI asks for the dataset location, update the Excel file path in the data source settings.
4. Refresh the data if required.
5. Use the slicers on the left side to filter the dashboard.
6. Navigate between the two report pages using the tabs at the bottom.
7. Hover over charts and data points to view additional information.

## Repository Structure

```text
Zomato-Restaurant-Analytics-Dashboard/
│
├── README.md
│
├── Zomato-Restaurant-Analytics.pbix
│
├── data/
│   └── restaurant_data.xlsx
│
└── screenshots/
    ├── page-1-dashboard.png
    └── page-2-dashboard.png
```

## Notes

- The `.pbix` file is the main Power BI project file.
- The Excel file is the source dataset, if redistribution is permitted by its source/license.
- If the dataset is not legally redistributable, keep it out of the public repository and document the original source instead.
- If the `.pbix` file is too large for normal GitHub browser upload, use Git from the command line or Git LFS as appropriate.
- Values estimated visually from chart screenshots are marked as approximate and should be verified against the underlying Power BI data before being treated as exact figures.

## Future Improvements

Possible future additions include:

- More detailed cuisine analysis
- Restaurant-level drill-through pages
- Additional geographic analysis
- Time-based analysis if historical data becomes available
- Additional comparison measures
- More advanced DAX calculations
- Currency standardization for more reliable cost comparisons
- Deeper analysis of restaurant ratings across cities and cuisines

## Author

**Shalini Nadar**

BSc Data Science Student

Mumbai, India

---

## Project Type

**Data Analytics | Business Intelligence | Power BI | Data Visualization**
