# Superstore Plus Kenya: The Discount Cliff

> The customer got the deal. But did the business?

## Overview

This Tableau data storytelling project explores how retail profitability varies across discount levels, product categories, and price segments.

The story moves beyond headline sales figures to identify where margins turn negative and which products are most exposed to deep discounts.

## Project Snapshot

| Metric | Value |
|---|---:|
| Net sales | KES 668.1M |
| Net profit | KES 129.0M |
| Overall net margin | 19.3% |

**Important:** The 19.3% overall margin covers the business as a whole. The 24.4% margin below applies specifically to transactions with no discount.

## Business Questions

- How does net profit margin vary across discount levels?
- Which categories have the highest share of loss-making transaction lines?
- Are high-price products more vulnerable to deep discounts?
- What discount guardrails does the analysis suggest?

## Key Findings

### 1. The Discount Cliff

| Discount | Net profit margin |
|---|---:|
| 0% | 24.4% |
| 5% | 18.6% |
| 10% | 14.9% |
| 15% | 8.5% |
| 20% | 6.4% |
| 25% | -5.1% |

At a 25% discount, the transaction group recorded a negative margin. Strong total sales therefore did not mean every sale was profitable.

### 2. Technology Was Especially Vulnerable

At a 25% discount, the share of transaction lines losing money was:

| Category | Loss-making transaction lines |
|---|---:|
| Technology | 56.9% |
| Office Supplies | 28.3% |
| Furniture | 5.5% |

These percentages describe **transaction-line counts**, not the share of revenue lost.

Technology subcategories also started with relatively thin full-price margins: Accessories at 14.0%, Computers at 14.2%, Networking and Power at 15.2%, and Printing at 18.8%.

### 3. High-Price Items Fell Furthest

- High-price items started with a 23.3% margin at full price and crossed into losses beyond 20% off.
- Mid-price items were near break-even at 25% off.
- Low-price items retained approximately a 13% margin at 25% off.

The same discount was not equally sustainable across all price segments.

### 4. One Transaction Makes the Risk Tangible

The **Nuru Solar Charging Kit Standard** illustrates what happens when discounted revenue falls below product cost:

| Metric | Amount |
|---|---:|
| Gross sales | KES 82,750 |
| Sales after 25% discount | KES 62,063 |
| Cost of goods sold | KES 65,882 |
| Reported loss | KES 3,819 |

*Amounts are presented as rounded in the Tableau story.*

The customer received the discount. The business absorbed the loss.

## Story Structure

1. **The Illusion of Volume** — headline sales, profit, and margin.
2. **Falling Off the Discount Cliff** — profitability across discount levels.
3. **Technology Hits the Cliff First** — category-level exposure and starting margins.
4. **The Price Tag Sets the Depth of the Fall** — differences across price segments.

## Recommendation

**Do not ban discounts. Manage them.**

The story recommends a **15% discount cap for Technology and high-price items**, alongside product-level profitability checks before approving deeper promotions.

This is a proposed guardrail based on the observed results, **not a proven optimal discount rate**. Any operational policy should also consider demand, inventory objectives, and the full cost structure.

## Tools and Analytical Approach

- **Tool:** Tableau
- **Output:** Four-part visual data story
- **Comparisons:** Net margin by discount level, loss-making transaction lines by category, and margin by price segment
- **Supporting example:** A transaction where discounted sales fell below cost of goods sold

## Interpretation and Limitations

- The charts compare observed transaction groups. They do not establish that discounts alone caused the differences in profitability.
- Product mix and other characteristics may differ across discount groups.
- The story does not quantify whether additional sales volume offsets the margin lost through discounting.
- The source story labels profitability as “net profit” and “net margin.” Its full cost definition is not documented in the supplied presentation; the transaction example specifically compares sales with cost of goods sold.
- Dataset provenance, reporting period, and low/mid/high price-segment thresholds are not specified in the supplied presentation.
- Findings should be interpreted within this dataset rather than generalized to all Kenyan retailers.

## Portfolio Takeaway

This project demonstrates how visual storytelling can connect headline business performance to transaction-level risk and a practical pricing recommendation.

**The question is not only “How much did we sell?” It is “How much profit did we keep?”**
