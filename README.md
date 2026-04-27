## 🗂️ Dataset — `swiggy_orders.csv`

| Column | Type | Description |
|---|---|---|
| `order_id` | int | Unique order identifier ⚠️ has duplicates |
| `restaurant_name` | str | Name of the restaurant |
| `city` | str | One of 12 Indian cities |
| `category` | str | Cuisine category |
| `order_value` | float | Order amount in ₹ |
| `delivery_time_mins` | int | Delivery duration ⚠️ has nulls + negatives |
| `rating` | float | Customer rating 1–5 ⚠️ has nulls + values > 5 |
| `order_date` | datetime | Date and time of order |
| `time_slot` | str | breakfast / lunch / snacks / dinner |
| `is_reorder` | bool | Whether it's a returning customer order |
| `discount_applied` | float | Discount amount (NaN = no discount) |
| `platform` | str | iOS / Android / Web |

**Shape:** 2,050 rows × 12 columns

---

## 📓 Workshop Sections

### 1 · NumPy Arrays & Vectorised Operations
- Convert order values to a NumPy array
- Compute **GMV**, **AOV**, median, and 90th percentile
- Segment orders into revenue tiers using boolean masks

| Tier | Range |
|---|---|
| Micro | < ₹200 |
| Mid | ₹200 – ₹500 |
| Premium | ₹500 – ₹1000 |
| Whale | ≥ ₹1000 |

### 2 · Load & Inspect Real Datasets
- Read CSV with `parse_dates`
- Explore schema with `.info()`, `.describe()`, `.head()`
- Spot anomalies: ratings > 5, negative delivery times, duplicate order IDs

### 3 · Filter, Sort & Slice
- Boolean masks for multi-condition filtering
- `.loc` (label-based) vs `.iloc` (position-based)
- Top 20 restaurants by revenue
- Loyal dinner crowd segment

### 4 · GroupBy & Aggregations
- City-wise GMV with share %
- Category × Time Slot revenue matrix
- Pivot table: Category vs City
- `.transform()` for within-group % contribution
- Reorder rate by time slot

### 5 · Handle Nulls, Duplicates & Dirty Data
- Null audit + column-specific cleaning strategy
- Fix bad ratings and negative delivery times
- Deduplicate on `order_id`
- Outlier detection via 3σ rule
- Export clean dataset

---

## 🔑 Key Metrics

| Metric | Formula |
|---|---|
| **GMV** | `sum(order_value)` |
| **AOV** | `GMV / number_of_orders` |
| **Whale Orders** | `order_value ≥ ₹1000` or top 5% (P95) |

---

## 🛠️ Requirements

pip install numpy pandas jupyter


---

## 🚀 Getting Started

git clone https://github.com/J-harshavardhan/swiggy-data-workshop.git
cd swiggy-data-workshop
jupyter notebook Swiggy_Workshop.ipynb


---

## 📋 Pandas Quick Reference

| Task | Code |
|---|---|
| Load CSV | `pd.read_csv('file.csv', parse_dates=['col'])` |
| Null audit | `df.isnull().sum()` |
| Filter | `df[df['col'] > value]` |
| Multi-filter | `df[(cond1) & (cond2)]` |
| GroupBy + agg | `df.groupby('col').agg({'val': ['sum', 'mean']})` |
| Pivot table | `pd.pivot_table(df, values, index, columns, aggfunc)` |
| Fill nulls | `df['col'].fillna(df['col'].median())` |
| Remove dupes | `df.drop_duplicates(subset='col', keep='first')` |

---

## 📄 License

This project is for educational purposes. Dataset is synthetically generated.
