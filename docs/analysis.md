## Business Problem 
The goal of this analysis is to understand why customers stop ordering and identify behavioral signals that indicate churn risk in an e-commerce marketplace. 

For this project, churn is defined as a customer who has not placed an order within 120 days of the most recent purchase date in the dataset. 

---

## Data Preparation 
- Analysis is limited to delivered orders only.
- Data was aggregated to a customer-level table using MySQL.
- Each row represents a sinal customer with behavioral features such as order count, revenue, review score, and delivery performance.
- The resulting dataset was exported and analyzed in Python using Pandas.

--- 

## Churn Definition 
A customer is considered churned if they have not placed an order within 120 days of the dataset's most recent purchase date. 

This definition is intentionally simple and transparent to ensure interpretability. 

--- 

## Key Findings 

### 1. Customer satisfaction is the strongest signal of churn 
Customers who churn consistently leave lower review scores than active customers. 
While the numerical difference appears modest, even small drops in average review score represent meaningful dissatisfaction on a 1 to 5 scale. 

This suggests overall experience quality plays a central role in repeat purchasing behavior. 

--- 

### 2. Late deliveries contribute to churn risk 
Late deliveries are relatively rare across the dataset, but they occur more frequently among churned customers. 

Although the average difference is small, delivery delays likely act as high-impact negative events that reduce customer satisfaction and discourage repeat purchases. 

--- 

### 3. Revenue and order value are weak predictors 
Total revenue and average order value show minimal separation between churned and active customers. 

Most customers place only a single order, meaning spend-based metrics primarily reflect one-time purchasing behavior rather than long-term engagement. 

---

### 4. Order frequency offers limiteed insight
Order counts are nearly identical between churned and active customers, reinforcing that this marketplace is dominated by one-time buyers. 

Retention challenges appear driven more by experience quality than purchasing volume. 

---

## Recommendation 
Retention efforts should focus on improving the early customer experience, particularly delivery reliability and issue resolution. 

Customers who experience delays or leave lower review scores are significantly less likely to return, while spend-based icentives are unlikely to meaningfully reduce churn in a predominantly one-time purchase marketplace. 

--- 

## Limitations 
- Churn is inferred based on inactivity rather than explicit cancellation or opt-out behavior.
- The dataset is time-bound, which may misclassify recently acquired customers as active.
- Review data is not available for all orders, which may underrepresent dissatisfaction in some cases.

--- 

## Conclusion 
This analysis shows that customer churn in this marketplace is primarily driven by experience-related factors rather than revenue or order size. 

Improving reliability and customer satisfaction early in the purchase lifecycle is likely to have a greater impact on retention than pricing or promotional strategies. 
