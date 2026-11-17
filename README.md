# YouTube Content Portfolio Intelligence & Optimization
### A Statistical Approach to Content Resource Allocation and Audience Growth

## 1. Project Overview

This project analyzes YouTube channel performance to understand how different content categories contribute to audience growth, engagement, and overall channel performance.

The objective is not just to identify videos with the highest views. It is to understand:

- Which content categories perform better?
- Which categories attract and retain audience attention?
- Is performance consistent or highly variable?
- Does a category generate a higher share of views than its share of published videos?
- Are observed category-level differences statistically significant?
- How can these findings support better content planning and resource allocation?

The project uses Python, statistical analysis, data visualization, and business interpretation to convert YouTube Analytics data into actionable insights.

## 2. Business Problem

A YouTube channel has limited time and resources to produce content.

Publishing more videos in a category does not necessarily mean that category generates more audience value.

The central business question is:

**How should a YouTube channel allocate its content-production efforts across categories to improve audience performance and make better content decisions?**

This project investigates that question using historical channel data.

## 3. Dataset Overview

The dataset contains YouTube video-level performance information.

- 240 individual video records.
- 5 content categories.
- 1 aggregate channel-level Total record, handled separately from individual videos.
- Performance metrics including views, engaged views, subscribers, stayed-to-watch percentage, and average percentage viewed.

### Main content categories

- Cricket
- Movie Review
- Politics
- Geopolitics
- Pop-Culture

### Important metrics

| Metric | Business meaning |
|---|---|
| Views | Total video views |
| Engaged Views | Views meeting YouTube's engaged-view definition |
| Subscribers | Subscribers gained |
| Stayed-to-Watch % | Share of viewers who stayed rather than swiping away |
| Average Percentage Viewed | Average proportion of a video watched |
| Median Views | Typical video performance, less sensitive to extreme values |
| Coefficient of Variation | Relative variation in category performance |

## 4. Project Workflow

The project follows an analytical workflow:

### Stage 1 — Ask

Defined the business problem, analytical objectives, and key questions.

### Stage 2 — Prepare

Loaded the YouTube Analytics dataset and examined its structure, columns, data types, missing values, and aggregate records.

### Stage 3 — Process

Performed data cleaning and preparation:

- Separated the aggregate Total record from individual video records.
- Standardized column names and data types.
- Checked missing values and duplicate records.
- Validated important metrics.
- Investigated outliers.
- Prepared publishing-date and video-performance features.
- Created a structured analytical dataset.

### Stage 4 — Analyze

Conducted multiple levels of analysis.

**A. Overall Channel Performance**

Established channel-level performance benchmarks and examined the overall distribution of key metrics.

**B. Category Performance**

Compared content categories using:

- Video count
- Total and median views
- Average engagement metrics
- Subscriber contribution
- Performance variation

**C. Portfolio Contribution Analysis**

Compared each category's percentage of published videos against its percentage of total views.

This helps identify categories that contribute more or less view share relative to their publishing share.

**D. Engagement Analysis**

Examined stayed-to-watch and average percentage viewed to distinguish between attracting viewers and retaining their attention.

**E. Distribution and Correlation Analysis**

Investigated skewness, performance distributions, and relationships between selected metrics using correlation analysis.

Correlation is treated as association, not proof of causation.

**F. Statistical Testing**

Used the Kruskal-Wallis test to examine whether view distributions differ across content categories.

Used Dunn's post-hoc comparisons to investigate category pairs when appropriate.

Effect size was also considered so that statistical significance would not be interpreted without practical context.

### Stage 5 — Content Context Investigation

Introduced a separate content-context review framework.

The objective is to investigate what lies behind individual video performance, beyond category names and numerical metrics.

The proposed review dimensions include:

- Main topic
- Event or subject
- Context type
- Content angle
- Topic type (for example, trending or evergreen)
- Title-hook type
- Context notes

Video titles and available information can help identify potential context, but unclear cases should remain unclassified until verified.

**Important:** Context labels must be checked against the actual video or reliable event information. The project should not claim that a trend, controversy, event, or title hook caused higher views without suitable evidence.

### Stage 6 — Share

Prepared visual explanations of:

- Category performance
- Content share versus view share
- Audience engagement
- Performance distributions
- Video-duration relationships
- Statistical analysis
- Business decision-making workflow

The final decision-framework chart explains how analytical evidence moves towards business actions.

### Stage 7 — Act

Converted analytical findings into practical recommendations:

- Review categories generating higher view share than content share.
- Investigate categories with weaker relative contribution.
- Evaluate audience-retention performance separately from views.
- Identify consistency and volatility.
- Examine high- and low-performing videos within the same category.
- Design controlled content experiments.

## 5. Tools and Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy
- Google Colab
- Jupyter Notebook

### Statistical methods

- Descriptive statistics
- Median and distribution analysis
- Skewness
- Pearson correlation
- Spearman correlation
- Kruskal-Wallis H-test
- Dunn's post-hoc test
- Epsilon-squared effect size
- Coefficient of variation

## 6. Key Analytical Principles

This project follows several important principles:

1. Individual video records and aggregate channel totals are not mixed.
2. Median views are considered alongside averages because video performance can be highly skewed.
3. Views and audience retention are treated as different performance dimensions.
4. Average percentage viewed can exceed 100% for Shorts because viewers may replay content.
5. Statistical significance is not treated as proof of business importance.
6. Publishing age and timing can affect comparisons between videos.
7. Correlation and historical comparisons do not establish causation.

## 7. Business Recommendations

The analysis supports a decision framework rather than an automatic rule to publish more videos in the highest-view category.

Potential actions include:

- Investigate categories with stronger view contribution relative to content volume.
- Review audience-retention patterns to understand content quality.
- Compare successful and unsuccessful videos within the same category.
- Verify topic and event context before making content-level conclusions.
- Test alternative hooks, topics, and content angles.
- Track results across multiple videos before changing the publishing strategy.

## 8. Project Limitations

- Some individual audience metrics contain missing values.
- Historical performance does not guarantee future results.
- Video publishing age and timing may influence comparisons.
- Context labels require manual verification.
- Production costs and creator working hours are unavailable, so financial ROI cannot be calculated.
- Observational analysis cannot establish that a particular content category or feature caused higher performance.

## 9. Expected Business Value

The project provides a structured way to understand a YouTube content portfolio.

It moves beyond simple view counting and combines performance measurement, audience engagement, statistical testing, contextual investigation, and business recommendations.

The resulting framework can help a channel owner make more evidence-based decisions about content planning and future experiments.

## 10. Conclusion

**YouTube Content Portfolio Intelligence & Optimization** demonstrates how raw YouTube Analytics data can be transformed into structured business intelligence.

The project connects three important analytical questions:

1. What is happening in the channel?
2. What patterns can explain the observed performance?
3. What should the channel investigate or test next?

The final objective is to support smarter content decisions through data, statistical reasoning, and contextual understanding.

---

**Project Type:** End-to-End Data Analytics & Statistical Analysis  
**Domain:** Digital Media / YouTube Analytics  
**Primary Focus:** Content Performance, Audience Engagement, Portfolio Optimization  
**Author:** Nishant Kamal
