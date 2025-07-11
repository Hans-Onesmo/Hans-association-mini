# Hans-association-mini

## Project Purpose
This project simulates fake transactional data and applies the Apriori algorithm to discover shopping patterns using association rules.

## Tools
- Python
- pandas
- mlxtend

## imulated Data
10 fake transactions were created using a pool of 8 items:
`Bread, Milk, Eggs, Cheese, Butter, Apples, Bananas, Yogurt`.

Each transaction includes 2–5 randomly selected items.

## Analysis
- One-hot encoding was applied to transactions.
- The Apriori algorithm was used to find frequent itemsets with support ≥ 0.3.
- Association rules were generated using confidence ≥ 0.7.

## Sample Rules (≥ 70% confidence)

1. **If a customer buys `Cheese`, they are likely to also buy `Bananas`.**  
   - Support: 0.3  
   - Confidence: 75%

2. **If a customer buys `Milk`, they are likely to also buy `Eggs`.**  
   - Support: 0.4  
   - Confidence: 80%

## Real-Life Meaning (Explanation of Rule 1)
This means that in 75% of the transactions where people bought Cheese, they also bought Bananas. A shop can use this pattern to:
- Place these two items closer on shelves.
- Offer them as a combo deal.
- Predict customer preferences for marketing.
