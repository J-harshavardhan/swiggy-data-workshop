
# swiggy-data-workshop# 🍔 Swiggy Orders — Data Analysis Workshop

> A hands-on Python data analysis workshop using a simulated Swiggy orders dataset. Learn how food-delivery platforms use data to track revenue, spot anomalies, and understand customer behaviour.

---

## 📁 Repository Structure

```
swiggy-workshop/
├── Swiggy_Workshop.ipynb      # Main workshop notebook
├── swiggy_orders.csv          # Raw dataset (2,050 orders)
├── swiggy_orders_clean.csv    # Cleaned dataset (output)
└── README.md
```

---

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
| `time_slot` | str | `breakfast` / `lunch` / `snacks` / `dinner` |
| `is_reorder` | bool | Whether it's a returning customer order |
| `discount_applied` | float | Discount amount (NaN = no discount) |
| `platform` | str | `iOS` / `Android` / `Web` |

**Shape:** 2,050 rows × 12 columns

---

## 📓 Workshop Sections

### 1 · NumPy Arrays & Vectorised Operations
- Convert order values to a NumPy array
- Compute **GMV**, **AOV**, median, and 90th percentile
- Segment orders into revenue tiers using boolean masks:

| Tier | Range | Description |
|---|---|---|
| Micro | < ₹200 | Low-value orders |
| Mid | ₹200 – ₹500 | Standard orders |
| Premium | ₹500 – ₹1000 | High-value orders |
| Whale | ≥ ₹1000 | Top spenders |

---

### 2 · Load & Inspect Real Datasets
- Read CSV with `parse_dates`
- Explore schema with `.info()`, `.describe()`, `.head()`
- Spot data anomalies:
  - Ratings > 5.0 (impossible values)
  - Negative delivery times (physically impossible)
  - Duplicate `order_id` entries

---

### 3 · Filter, Sort & Slice
- Boolean masks for multi-condition filtering
- `.loc` (label-based) vs `.iloc` (position-based) indexing
- Top 20 restaurants by total revenue
- Loyal dinner crowd: reorders with rating ≥ 4.0 and order ≥ ₹300
- Highest-value order per city

---

### 4 · GroupBy & Aggregations
- City-wise GMV breakdown with share %
- Category × Time Slot revenue matrix
- Pivot table: Category vs City revenue
- `.transform()` for within-group % contribution
- Reorder rate by time slot

---

### 5 · Handle Nulls, Duplicates & Dirty Data
- Full null audit per column
- Column-specific cleaning strategy:

| Column | Strategy |
|---|---|
| `discount_applied` | Keep NaN — means no discount was applied |
| `rating` | Fill with global median |
| `delivery_time_mins` | Fill with city-wise median |
| `time_slot` | Fill with mode |

- Fix bad ratings (> 5 → NaN) and negative delivery times
- Deduplicate on `order_id`, keep first occurrence
- Outlier detection via 3σ rule (flag, not removed — real whale orders)
- Export clean dataset to `swiggy_orders_clean.csv`

---

## 🔑 Key Metrics

| Metric | Formula |
|---|---|
| **GMV** (Gross Merchandise Value) | `sum(order_value)` |
| **AOV** (Average Order Value) | `GMV / number_of_orders` |
| **Whale Orders** | `order_value ≥ ₹1000` or top 5% (P95) |

---

## 🛠️ Requirements

```bash
pip install numpy pandas jupyter
```

---

## 🚀 Getting Started

```bash
git clone https://github.com/your-username/swiggy-workshop.git
cd swiggy-workshop
jupyter notebook Swiggy_Workshop.ipynb
```

---

## 📋 Pandas Quick Reference

| Task | Code |
|---|---|
| Load CSV | `pd.read_csv('file.csv', parse_dates=['col'])` |
| Shape | `df.shape` |
| Null audit | `df.isnull().sum()` |
| Filter | `df[df['col'] > value]` |
| Multi-filter | `df[(cond1) & (cond2)]` |
| Sort | `df.sort_values('col', ascending=False)` |
| GroupBy + agg | `df.groupby('col').agg({'val': ['sum', 'mean']})` |
| Pivot table | `pd.pivot_table(df, values, index, columns, aggfunc)` |
| Fill nulls | `df['col'].fillna(df['col'].median())` |
| Remove dupes | `df.drop_duplicates(subset='col', keep='first')` |
| Column to NumPy | `df['col'].values` |
| Vectorised sum | `np.sum(array)` |

---

## 📄 License

This project is for educational purposes. Dataset is synthetically generated.
