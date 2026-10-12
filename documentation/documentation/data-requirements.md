# Data Requirements

## 1. Purpose

The purpose of this document is to define the data required to address the business and functional requirements identified for the ShopEase analysis.

The required data should support analysis of sales, products, customers, regions, discounts, delivery performance, customer satisfaction, and returns.

---

## 2. Required Data Domains

The analysis requires information from the following business areas:

1. Orders & Sales
2. Products
3. Customers
4. Geography
5. Discounts
6. Delivery
7. Customer Experience
8. Returns

---

## 3. Required Data Fields

| Field           | Description                            | Business Use               |
| --------------- | -------------------------------------- | -------------------------- |
| Order ID        | Unique identifier for each order       | Order analysis             |
| Customer ID     | Unique customer identifier             | Customer analysis          |
| Order Date      | Date the order was placed              | Trend analysis             |
| Product ID      | Unique product identifier              | Product analysis           |
| Product Name    | Name of the product                    | Product performance        |
| Category        | Product category                       | Category analysis          |
| Region          | Customer/order region                  | Regional analysis          |
| Quantity        | Number of units purchased              | Sales volume               |
| Unit Price      | Price per unit                         | Revenue calculation        |
| Discount        | Discount applied to order/product      | Discount analysis          |
| Revenue         | Revenue generated from order           | Revenue analysis           |
| Delivery Date   | Date order was delivered               | Delivery analysis          |
| Delivery Days   | Number of days taken for delivery      | Delivery performance       |
| Customer Rating | Customer rating for the order/product  | Customer experience        |
| Return Status   | Whether the order/product was returned | Return analysis            |
| Return Reason   | Reason for return                      | Return investigation       |
| Payment Method  | Payment method used                    | Customer behavior analysis |

---

## 4. Customer-Level Data

Customer-level information should support analysis of customer purchasing behavior.

Required information includes:

* Customer ID
* Order history
* Purchase frequency
* Total customer revenue
* Average order value
* Customer segment

Where appropriate, customers may be categorized into groups such as:

* High Value
* Medium Value
* Low Value

---

## 5. Product-Level Data

Product information should allow analysis of product and category performance.

Required information includes:

* Product ID
* Product name
* Product category
* Unit price
* Quantity sold
* Revenue
* Return status
* Return reason
* Customer rating

---

## 6. Regional Data

Regional information should allow comparison of business performance across geographic areas.

Required information includes:

* Region
* Orders
* Revenue
* Quantity sold
* Average Order Value
* Delivery performance
* Return rate

---

## 7. Delivery Data

Delivery information should support analysis of operational performance.

Required fields include:

* Order ID
* Order Date
* Delivery Date
* Delivery Days
* Region
* Customer Rating

The analysis will use these fields to identify delivery delays and investigate their potential relationship with customer satisfaction.

---

## 8. Return Data

Return information should support investigation of product return patterns.

Required fields include:

* Order ID
* Product ID
* Category
* Region
* Return Status
* Return Reason
* Customer Rating

---

## 9. Data Quality Requirements

The dataset should be checked for:

* Missing values
* Duplicate records
* Invalid dates
* Incorrect numerical values
* Inconsistent category names
* Invalid discount values
* Invalid ratings
* Incorrect or negative quantities
* Inconsistent return indicators

---

## 10. Data Granularity

The preferred dataset granularity is **order-level or transaction-level data**, where each record represents an individual order or order line.

This level of detail allows analysis to be performed across:

* Time
* Products
* Categories
* Customers
* Regions
* Discounts
* Delivery
* Returns

---

## 11. Data-to-Requirement Mapping

| Business Requirement             | Required Data                                           |
| -------------------------------- | ------------------------------------------------------- |
| BR-01: Overall Performance       | Order Date, Revenue, Quantity, Order ID                 |
| BR-02: Product Performance       | Product, Category, Revenue, Quantity, Returns           |
| BR-03: Regional Performance      | Region, Revenue, Orders, AOV                            |
| BR-04: Customer Behavior         | Customer ID, Orders, Revenue, Purchase Frequency        |
| BR-05: Discount Effectiveness    | Discount, Revenue, Quantity, Category                   |
| BR-06: Delivery Performance      | Order Date, Delivery Date, Delivery Days, Rating        |
| BR-07: Return Analysis           | Return Status, Return Reason, Product, Category, Region |
| BR-08: Improvement Opportunities | Combined analysis across all relevant data              |

---

## 12. Data Assumptions

For this portfolio case study:

* The dataset represents fictional or publicly available e-commerce transactions.
* No personally identifiable customer information will be used.
* Customer IDs will be anonymized identifiers.
* Revenue calculations will be based on the defined pricing and quantity fields.
* Business assumptions will be documented before analysis.
