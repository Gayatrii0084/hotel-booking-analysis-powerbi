
# Hotel Booking Analysis – Power BI Dashboard

## Project Overview
This is an end-to-end data analysis project built on a hotel booking dataset covering a **City Hotel** and a **Resort Hotel** over three years (2015–2017). The raw data was cleaned, wrangled, and modeled from scratch, then used to build an interactive Power BI dashboard comparing the two properties individually and against each other, with the goal of surfacing actionable business insights for the hotel group.

## Dataset
The dataset contains **119,389 rows and 32 columns**, including:

- `hotel` – Type of hotel (City or Resort)
- `is_cancelled` – Whether the booking was cancelled
- `lead_time` – Days between booking and arrival
- `arrival_date_year` / `arrival_date_month` / `arrival_date_week_number` / `arrival_date_day_of_month`
- `stays_in_weekend_nights` / `stays_in_week_nights`
- `adults` / `children` / `babies`
- `meal` – Type of meal booked
- `country` – Guest's country of origin
- `market_segment` / `distribution_channel`
- `is_repeated_guest`, `previous_cancellations`, `previous_bookings_not_cancelled`
- `reserved_room_type` / `assigned_room_type`
- `booking_changes`
- `deposit_type`
- `agent` / `company`
- `days_in_waiting_list`
- `customer_type`
- `adr` (Average Daily Rate)
- `required_car_parking_spaces`
- `total_of_special_requests`
- `reservation_status` / `reservation_status_date`

## Approach
1. **Data Cleaning** – Handled null values and removed duplicate records.
2. **Data Wrangling** – Structured and transformed the data for analysis in Power BI.
3. **Exploratory Analysis** – Compared City Hotel vs Resort Hotel performance across revenue, bookings, cancellations, seasonality, and guest behavior.
4. **Dashboard Design** – Built a multi-page interactive Power BI report with slicers for hotel type, year, booking status, customer type, season, and country.

## Dashboard

### Page 1 – Revenue & Booking Overview
KPIs for total revenue, booking count, average ADR, cancellation rate, and average lead time, along with booking share by hotel, revenue and ADR by market segment, and monthly revenue trends.
<img width="1097" height="637" alt="hotel_dash1" src="https://github.com/user-attachments/assets/f617b4d8-a52b-487f-95df-c7fd12bff4d4" />

### Page 1 (continued) – Weekly & Cancellation Trends
Booking volume and cancellation rate by week number, split by hotel, plus revenue and ADR trends across the year.

<img width="1105" height="612" alt="hotel_dash2" src="https://github.com/user-attachments/assets/04a60f2b-3ac5-419f-9cc1-e91ea1c321d4" />

### Page 2 – Guest Insights
Guest counts, room satisfaction, average stay length, repeat guest rate, and breakdowns by customer type, meal preference, market segment, and top guest countries.
<img width="1097" height="617" alt="hotel_dash3" src="https://github.com/user-attachments/assets/9af9bec5-3064-4f3a-ad24-5102f629062b" />


## Key Insights
- **61.07%** of guests preferred the City Hotel vs **38.93%** for the Resort Hotel.
- City Hotel bookings were higher in 2016 and 2017; the Resort Hotel saw a noticeable decline in 2017.
- City Hotels generate more revenue overall, driven by a higher ADR than Resort Hotels.
- **91.6%** of guests did not require a parking space; only **8.3%** needed one.
- City Hotel bookings had a longer average waiting time.
- Over **27%** of all bookings were cancelled.
- July and August were the peak booking months, likely due to summer vacation travel.
- Agents **9** and **240** drove the highest booking volumes; agents **1** and **6** the lowest.
- Most guests came from **Portugal, United Kingdom, France, and Spain**.
- **Online TA** and **Offline TA/TO** were the top booking channels.
- Room types **A** and **D** were the most frequently booked over the three years.
- Repeat guests made up a very small share of the overall client base.
- Average length of stay was **7 days** across both hotel types.
- **Bed & Breakfast (BB)** was the most preferred meal plan.
- `arrival_date_year` and `arrival_date_week_number` showed a negative correlation (**-0.51**); `stays_in_week_nights` and `total_stay` showed a strong positive correlation (**0.95**).
- ADR increases with total guest count, showing a direct relationship between group size and revenue per booking.

## Business Recommendations
- The Resort Hotel should invest in new strategies to attract more guests, since the City Hotel currently outperforms it in both bookings and revenue.
- Since BB is by far the most popular meal plan, both hotels should promote other meal options to diversify revenue.
- With most guests coming from Portugal, there's an opportunity to expand advertising in other countries to grow the international guest base.
- Since most guests don't need parking, hotels could redirect that investment toward amenities guests actually value.
- With cancellations above 27%, both hotels need clearer cancellation policies or incentives to reduce no-shows and last-minute cancellations.
- Since longer stays are linked to higher revenue, guest retention strategies (loyalty programs, extended-stay discounts) could help boost overall ADR.

## Tools Used
- **Power BI** – Data modeling, DAX measures, and interactive dashboard design
- **Excel/Power Query** – Data cleaning and wrangling

## Repository Contents
```
├── README.md
├── hotel_booking_analysis.pbix
└── images/
    ├── dashboard-page1-revenue-overview.png
    ├── dashboard-page1b-weekly-trends.png
    └── dashboard-page2-guest-insights.png
```

---
*Built independently as a self-driven data analytics project.
