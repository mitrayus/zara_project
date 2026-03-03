# Zara Retail Strategy: Econometric Analysis of Placement & Pricing

## 📌 Executive Summary
This project utilizes the **Zara Fashion Products (US) 2024** dataset by Varisha to analyze the causal drivers of sales volume. By applying **Multivariate OLS Regression** and **Interaction Modeling**, the study moves beyond descriptive analytics to identify the "multiplier effects" of store placement.

## 🔍 Research Questions
1. **The Placement Myth:** Does high-visibility placement independently drive sales, or is its value conditional on product status?
2. **Price Elasticity:** How sensitive are Zara customers to price changes, and does this sensitivity vary by category?

## 🛠 Technical Methodology
As an Economics-focused analysis, this project prioritizes **interpretability and causal inference** over black-box prediction:

* **Multivariate Regression:** Used to estimate **Constant Elasticity of Demand**, allowing coefficients to be interpreted as percentage changes.
* **Treatment Effect Engineering:** Aggregated locations into a categorical variable `product_position` variable to isolate the Average Treatment Effect (ATE) of high-visibility zones.
* **Heterogeneous Treatment Effects:** Utilized interaction terms to identify synergies between merchandising and marketing levers.

**Key Findings:** Premium placement (Front of Store/End-caps) does not independently drive sales for items but acts as a **5.5% revenue multiplier** for promotional and **2.6% revenue multiplier** seasonal goods. More specifically, compared to Aisle, **End-cap** placement **boosts sales by 15.5% for promotional goods** and **by 16.5% for seasoanl goods**. On the other hand **Store-front** placement **boosts sales by 6% for seasonal goods** but hurts sales by 7% for promotional goods. 

Finally, overall price elasticity is **-0.08** suggesting inelastic demand and that the store has can earn more revenue by raising prices. When promotion is applied, compared to jackets, **sweaters have a 21.7% higher effect on sales** but **tshirts have a 15% lower effect**. 

Although **Statistical Significance** is a concern due to low sample size, the direction and magnitude of the coefficients provide a strong directional signal that warrants larger-scale tests.

## 💡 Strategic Recommendations

1.  **Dynamic Merchandising:** Reserve "End-cap" for both promotional and seasonal items, and "Store-front" for only seasonal items
2.  **Margin Protection:** Maintain full-price margins on "Staple" categories like T-Shirts, as the data shows these items are less sensitive to promotional discounting.
3.  **Pricing Headroom:** Given the low price elasticity (-0.08), Zara has the opportunity to test higher price points on high-demand items without risking significant volume loss.


