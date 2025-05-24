# 🛍️ Price Anchoring Analysis on Amazon India

This project investigates **price anchoring effects in e-commerce** using a large dataset of real Amazon India transactions and pricing references. We apply advanced statistical analysis and behavioral economic theory to uncover how pricing influences consumer behavior.

---

## 📌 Executive Summary

Price anchoring is a cognitive bias where consumers use the first price they see (the "anchor") to evaluate value. In e-commerce, this is often reflected by showing inflated MRPs alongside discounted prices.

Although direct MRP-sale price comparison was not possible due to data structure differences, we adapted our analysis to uncover indirect anchoring effects by studying price tiers, sales volumes, and category-specific elasticities.

---

## 🎯 Research Question

**Original**:  
> Does price anchoring—defined as displaying a higher MRP compared to the actual selling price—lead to increased purchases on Amazon?

**Adapted**:  
> How do different price points influence consumer purchasing behavior, and what optimal pricing strategies can be derived from sales patterns across categories?

---

## 📁 Data Sources

- `Amazon Sale Report.csv`  
  > Contains 106,573 valid Amazon India orders (March–June 2022), including product SKUs, sale amounts, and quantities.

- `May-2022.csv` and `P_L March 2021.csv`  
  > Contain platform-specific MRP data across categories such as Kurta, Western Dress, and Blouse.

---

## 🧪 Methodology

### ✔️ Key Techniques
- SKU-level sales aggregation
- Price tier segmentation (`<300`, `300–500`, ..., `1200+`)
- Category-specific price elasticity calculation
- ANOVA tests for sales variation across price tiers
- Log-log modeling for elasticity estimation
- Weekly temporal elasticity tracking
- Cross-category correlation analysis

### ✔️ Statistical Methods
- Pearson correlation
- One-way ANOVA
- Log-log elasticity approximation
- Temporal performance tracking

---

## 📊 Key Results

### 🔹 Price Anchoring Insights
- **Positive correlation** between price and quantity sold (r = 0.0787 overall, 0.175 in log-log space)
- **Statistically significant price tier differences** (F = 22.52, p < 0.001)
- **Sweet spot** found in the ₹350–450 and ₹700–900 tiers for mass-market and premium segments

### 🔹 Category-Specific Elasticities
| Category        | Elasticity | Optimal Price Range | Strategy                        |
|----------------|------------|----------------------|---------------------------------|
| Kurta          | 0.015      | ₹632–₹1128           | Premium positioning             |
| Western Dress  | 0.085      | ₹717–₹747            | Precision pricing               |
| Blouse         | 0.566      | ₹586–₹701            | Competitive, price-sensitive    |

### 🔹 Temporal Trends
- **Week 14** had the highest price elasticity (0.237) during a promotional period
- **April** was the peak sales month (41,183 units)

### 🔹 Cross-Category Findings
- Strong **volume correlation** between Kurta and Set (0.884)
- **Complementary pricing** and bundling opportunities across traditional categories

---

## 💼 Business Recommendations

- **Kurta**: Emphasize quality through premium pricing
- **Western Dress**: Maintain prices in the ₹717–747 range for optimal sales
- **Blouse**: Compete aggressively on price; highly elastic market
- **Set**: Bundle with Kurta to leverage complementary purchasing behavior
- **Promotions**: Target Week 14-like periods for discount campaigns
- **Portfolio Optimization**: Balance high-margin and high-volume categories

---

## ⚠️ Limitations

- No direct mapping between SKU pricing and sales data
- Analysis limited to 3-month window
- Results specific to Amazon India and fashion categories

---

## 🔧 Technical Stack

- **Languages**: Python (Jupyter Notebook)
- **Libraries**: pandas, numpy, scipy, seaborn, matplotlib
- **Stats Techniques**: Correlation, ANOVA, log-log elasticity modeling

---

## 📈 Visual Outputs

Project includes:
- Category-specific elasticity charts
- Weekly price-volume trendlines
- Revenue-performance heatmaps
- Cross-category correlation matrices

---

## 🚀 Future Work

- A/B testing for real-time anchoring experiments
- Competitive analysis across platforms (Ajio, Flipkart, etc.)
- Customer segmentation and personalized pricing models
- Machine learning for dynamic pricing optimization

---

## 📬 Contact

For questions or collaboration:  
**Naeem Almohtaseb**  
[LinkedIn] | [GitHub] | [Email Placeholder]

---

