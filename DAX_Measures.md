# 🧮 DAX Measures

## Total Quantity

```DAX
Total_Quantity =
SUM(SalesData[Units Sold])
```

Calculates the total number of mobile phones sold.

---

## Total Sales

```DAX
Total_Sales =
SUMX(
    SalesData,
    SalesData[Price Per Unit] * SalesData[Units Sold]
)
```

Calculates total revenue generated from all transactions.

---

## Total Transactions

```DAX
Transactions =
COUNTROWS(SalesData)
```

Counts the total number of completed transactions.

---

## Average Price

```DAX
Average_Price =
AVERAGE(SalesData[Price Per Unit])
```

Calculates the average selling price of all mobile phones.

---

## Calendar Table

A Calendar Table was created to enable efficient time intelligence analysis including:

- Year
- Month
- Quarter
- Day
- Time-based filtering

This improves report performance and supports future time intelligence calculations.
