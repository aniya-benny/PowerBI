# Flight Booking & Travel Data Analysis — Power BI

An interactive business intelligence dashboard built using **Microsoft Power BI**, analysing flight booking patterns, ticket pricing, passenger demographics, payment behaviour, and travel class distribution across multiple airlines and global departure cities.

---

## Key Metrics at a Glance

| Metric | Value |
|---|---|
| Total Bookings | 250 |
| Total Ticket Revenue | $0.64M |
| Average Passenger Age | 45.60 years |
| Total Distance Covered | 1.89M km |
| Average Flight Duration | 11.04 hours |
| Average Ticket Price | $2.58K |

---

## Dashboard Visuals

The dashboard is built on a single interactive page with an **Airline slicer** at the top right that filters all visuals simultaneously.

### 1. KPI Cards — Summary Metrics
Six KPI cards across the top provide an instant snapshot of the dataset:
- **Count of Bookings** — total number of flight bookings recorded
- **Sum of Ticket Price** — cumulative revenue from all tickets ($0.64M)
- **Average Passenger Age** — mean age of all passengers (45.60)
- **Sum of Distance (km)** — total flight distance across all bookings (1.89M km)
- **Average Flight Duration** — mean flight time in hours (11.04)
- **Average Ticket Price** — mean price per ticket ($2.58K)

---

### 2. Sum of Ticket Price by Airline
A horizontal bar chart ranking airlines by total ticket revenue generated:

| Airline | Revenue |
|---|---|
| B Airlines | $0.13M |
| S Airlines | $0.11M |
| E Airlines | $0.11M |
| L Airlines | $0.10M |
| Air I | $0.10M |

B Airlines leads in total ticket revenue, with S Airlines and E Airlines closely following.

---

### 3. Sum of Ticket Price by Departure City
A column chart comparing total ticket revenue across 8 major global departure cities:

| Departure City | Revenue |
|---|---|
| Mumbai | $98K |
| London | $91K |
| Delhi | $83K |
| Singapore | $81K |
| Frankfurt | $78K |
| Paris | $76K |
| Dubai | $73K |
| New York | $65K |

Mumbai generates the highest ticket revenue among all departure cities, followed by London and Delhi. New York records the lowest despite being a major hub, suggesting fewer bookings or shorter-haul routes in the dataset.

---

### 4. Count of Bookings by Travel Class
A horizontal bar chart showing booking distribution across four travel classes (out of 250 total):

| Travel Class | Count | Share |
|---|---|---|
| Premium Business | 69 | ~27.6% |
| First | 63 | ~25.2% |
| Business | 62 | ~24.8% |
| Economy | 56 | ~22.4% |

Bookings are remarkably evenly distributed across all four classes, with Premium Business slightly ahead. Economy has the fewest bookings, suggesting a dataset skewed toward premium travellers.

---

### 5. Ticket Price by Payment Method
A treemap showing total ticket revenue split by payment method:

| Payment Method | Revenue |
|---|---|
| Credit Card | $120.92K |
| Net Banking | $120.65K |
| Cash | $117.78K |
| PayPal | $111.43K |
| Debit Card | $99.26K |
| UPI | $74.53K |

Credit Card and Net Banking are the top two payment methods by revenue, contributing nearly equally. UPI generates the least revenue, indicating lower adoption or lower-value transactions.

---

### 6. Bookings by Payment Method
A donut chart showing the share of total bookings by payment method. Credit Card, Cash, Net Banking, and PayPal make up the four most-used methods, with UPI and Debit Card forming the smaller segments.

---

### 7. Sum of Ticket Price by Passenger Age (Bins)
A column chart grouping total ticket revenue by passenger age ranges:

| Age Bin | Revenue |
|---|---|
| ~30s | $9K |
| ~40s | $90K |
| ~50s | $69K |
| ~55–60 | $47K |
| ~60–65 | $46K |
| ~65+ | $58K |

Passengers in the **40s age group** generate the highest ticket revenue by a significant margin ($90K), followed by the 50s group ($69K). Younger passengers in the 30s contribute the least ($9K).

---

## Dataset

The dataset contains flight booking records with the following key fields:

| Field | Description |
|---|---|
| Booking_ID | Unique identifier for each booking |
| Airline | Name of the airline |
| Departure_City | City from which the flight departs |
| Travel_Class | Class of travel (Economy, Business, First, Premium Business) |
| Ticket_Price | Price paid for the ticket in USD |
| Payment_Method | Method used for payment (Credit Card, Cash, Net Banking, PayPal, Debit Card, UPI) |
| Passenger_Age | Age of the passenger |
| Distance_km | Flight distance in kilometres |
| Flight_Duration | Duration of the flight in hours |

---

## Tools and Technologies

| Tool | Purpose |
|---|---|
| Microsoft Power BI Desktop | Dashboard design and visualisation |
| Power BI DAX | Calculated measures for KPI cards (Sum, Average, Count) |
| Power BI Slicers | Interactive Airline filter applied across all visuals |
| Power BI Treemap | Payment method revenue breakdown |
| Power BI Donut Chart | Booking share by payment method |

---

## How to Open

1. Download the `.pbix` file from this repository.
2. Open it in **Microsoft Power BI Desktop** (free download from Microsoft).
3. The dataset is embedded inside the `.pbix` — no separate file is needed.
4. Use the **Airline slicer** (top right) to filter all charts by a specific airline.

---

## Key Insights from the Dashboard

- **Mumbai and London are the top revenue-generating departure cities**, together contributing $189K — nearly 30% of total revenue.
- **Premium Business is the most booked travel class**, slightly ahead of First and Business class, suggesting a high-spending traveller segment.
- **Credit Card and Net Banking are nearly tied as the preferred payment methods** — both exceeding $120K in revenue, indicating strong digital payment adoption.
- **Passengers aged 40–50 are the highest-spending age group**, generating $90K in ticket revenue — a key demographic for targeted airline marketing.
- **UPI contributes the least revenue ($74.53K)** despite being a popular payment method in India, possibly reflecting lower-value domestic routes.
- **Revenue is fairly spread across airlines**, with no single carrier dominating — B Airlines leads with $0.13M but the gap to the last airline ($0.10M) is narrow.
- **Average flight duration of 11.04 hours** and average distance of 1.89M km confirm the dataset primarily represents long-haul international routes.

---

## Author

Created as part of a Data Analytics learning project using simulated flight booking data.

