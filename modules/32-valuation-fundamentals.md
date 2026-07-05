# Module 32: Valuation Fundamentals

**Learning time:** 20-25 minutes  
**Prerequisites:** Module 31 (Company Analysis Basics)

---

## 🤔 The Core Question

In Module 31, we learned how to analyze a company. Now the question is: **how do we know if a stock is expensive or cheap?**

This is valuation — the art and science of determining what a company is worth.

In this module, we'll cover:
- Why valuation matters
- The two main approaches (relative and absolute)
- Key valuation multiples
- How to value a company from scratch
- Common mistakes to avoid

---

## 📖 Why Valuation Matters

### The Price vs. Value Gap

Every stock has:
- **Market price:** What investors pay today
- **Intrinsic value:** What the company is actually worth

```
If market price < intrinsic value → UNDERVALUED (buy)
If market price > intrinsic value → OVERVALUED (sell)
If market price ≈ intrinsic value → FAIRLY VALUED (hold)
```

> 💡 **Key insight:** Markets can stay irrational longer than you can stay solvent. But over time, prices converge to value.

### Why It's Hard

1. **Future is uncertain:** We don't know what'll happen in 5-10 years
2. **Multiple valid methods:** Different approaches give different answers
3. **Qualitative factors:** Brand, moat, management are hard to quantify
4. **Market emotions:** Fear and greed move prices away from fair value

---

## 📊 The Two Valuation Approaches

### Approach 1: Relative Valuation

**What it is:** Compare the stock to similar companies or historical averages

**Pros:**
- Quick and easy
- Market-informed (what investors currently pay)
- Works well for comparable companies

**Cons:**
- Assumes the "peer group" is fairly valued
- Can miss extremes
- Doesn't give an "absolute" fair price

**Common multiples:**
- P/E (price to earnings)
- P/S (price to sales)
- EV/EBITDA
- P/B (price to book)

### Approach 2: Absolute Valuation (DCF)

**What it is:** Calculate what the company is worth based on future cash flows

**Pros:**
- Gives a specific fair value
- Based on fundamentals
- Works for any company

**Cons:**
- Requires assumptions about the future
- Sensitive to small input changes
- Can be complex

**Method:**
- Discounted Cash Flow (DCF)
- Dividend Discount Model (DDM)

---

## 🔢 Key Valuation Multiples

### 1. Price-to-Earnings (P/E)

```
P/E = Stock Price / Earnings Per Share
```

**Types:**
- **Trailing P/E:** Based on last 12 months earnings
- **Forward P/E:** Based on next 12 months earnings

**How to use:**
```
Stock price = EPS × P/E
```

**Example:**
```
Apple stock: $180
EPS (TTM): $6.13
P/E = 180 / 6.13 = 29.4x
```

**Is 29x expensive?**
- Compare to: S&P 500 (~20x), sector average, historical P/E
- Consider: Growth rate (higher growth justifies higher P/E)

### 2. Price-to-Sales (P/S)

```
P/S = Market Cap / Revenue
     or
P/S = Stock Price / Revenue per Share
```

**Best for:**
- Companies without earnings (startups, unprofitable)
- Comparing across profit margins

**Example:**
```
Apple:
Revenue/share = $24.50
Stock price = $180
P/S = 180 / 24.5 = 7.3x

Amazon:
Revenue/share = $6.50
Stock price = $180
P/S = 180 / 6.5 = 27.7x
```

### 3. EV/EBITDA

```
EV = Market Cap + Debt - Cash
EBITDA = Earnings + Interest + Taxes + Depreciation + Amortization
```

**Why use it:**
- Neutral to capital structure (debt vs. equity)
- Compares operating performance
- Useful for leveraged industries (banks, telecoms)

**Example:**
```
Company X:
EV: $100 billion
EBITDA: $10 billion
EV/EBITDA = 10x
```

### 4. Price-to-Book (P/B)

```
P/B = Stock Price / Book Value per Share
```

**Best for:**
- Financial companies (banks, insurers)
- Asset-heavy companies (real estate, utilities)

**Example:**
```
UK Banks (typical):
Barclays P/B: ~0.5x
HSBC P/B: ~0.7x
Lloyds P/B: ~0.9x
```

> ⚠️ **Warning:** A P/B below 1x can indicate problems. "Tobin Q" suggests fair value is around 1x.

---

## 🧮 Absolute Valuation: The DCF Method

### What is DCF?

Discounted Cash Flow calculates the present value of all future cash flows.

**The concept:**
```
$100 today = $100
$100 in 1 year (at 10% discount) = $90.91
$100 in 2 years (at 10% discount) = $82.64
```

### The Steps

**Step 1: Forecast Free Cash Flow (FCF)**
- Estimate next 5-10 years of FCF
- Assume growth rate (can vary)

**Step 2: Determine Discount Rate**
- Usually WACC (Weighted Average Cost of Capital)
- Typical: 8-12% for mature companies
- Higher for riskier companies

**Step 3: Calculate Terminal Value**
- Value beyond forecast period
- Assume perpetual growth (typically 2-3%)
- Formula: Terminal FCF / (Discount Rate - Growth Rate)

**Step 4: Discount All Cash Flows**
- Present value = Future value / (1 + r)^n

**Step 5: Sum and Compare**
- Sum all present values = Intrinsic value
- Compare to current market cap

### Simplified Example

```
Company Y:
Current FCF: $100 million
Growth: 5% for 5 years
Terminal growth: 2.5%
Discount rate: 10%

Year 1: $105M / 1.1 = $95M
Year 2: $110M / 1.1² = $91M
Year 3: $116M / 1.1³ = $87M
Year 4: $122M / 1.1⁴ = $83M
Year 5: $128M / 1.1⁵ = $80M

Terminal: $128M × 1.025 / (0.10 - 0.025) = $1.75 trillion
Terminal PV: $1.75T / 1.1⁵ = $1.09 trillion

Total PV: $95 + $91 + $87 + $83 + $80 + $1,090B = ~$1,446B

Intrinsic value: $1.4 trillion
Current market cap: $1.0 trillion
→ UNDERVALUED by ~40%
```

---

## 🎯 How to Value Any Company

### The Framework

1. **Choose your method:**
   - Relative (quick, market-informed)
   - Absolute (fundamental, specific)

2. **Gather data:**
   - Financial statements (3-5 years)
   - Peer comparisons
   - Analyst estimates

3. **Apply method:**
   - Calculate multiples
   - Build DCF model

4. **Make a decision:**
   - What's the margin of safety?
   - Does it fit your thesis?

---

## 🌍 Valuation by Sector

Different sectors trade at different multiples:

| Sector | Typical P/E | Why |
|--------|-------------|------|
| Tech (growth) | 25-50x | High growth, high margins |
| Consumer | 15-25x | Stable, moderate growth |
| Financials | 8-15x | Cyclical, leverage |
| Energy | 6-12x | Cyclical, commodity |
| Utilities | 10-18x | Stable, regulated |
| Healthcare | 15-30x | Demographics, patents |

**UK examples:**
```
Shell:    P/E ~8x (cyclical, commodity risk)
Unilever: P/E ~18x (steady consumer)
AstraZeneca: P/E ~25x (pharma moat)
Vodafone: P/E ~10x (telecom, high yield)
```

---

## ⚠️ Common Valuation Mistakes

### Mistake 1: Ignoring Growth
A high P/E is OK if growth is high. Compare P/E to growth (PEG ratio).

### Mistake 2: Using Trailing vs. Forward
Trailing P/E uses past earnings. Forward P/E uses expected earnings. Know which you're looking at.

### Mistake 3: Comparing Different Industries
Tech and banks trade at completely different multiples. Don't compare across sectors.

### Mistake 4: Ignoring Balance Sheet
A company can look cheap on P/E but be uninvestable if debt is too high. Check net debt/EBITDA.

### Mistake 5: Anchoring to Historicals
"Just because it's historically cheap doesn't mean it's cheap now."

### Mistake 6: Not Considering Margins
Two companies can have same revenue but different profits. Margins matter for valuation.

---

## 📱 Tools for Valuation

### Free Tools
- Yahoo Finance — P/E, P/B, growth rates
- Morningstar — Fair value estimates
- Finviz — Stock screener
- GuruFocus — DCF calculator

### Professional Tools
- Bloomberg (expensive)
- FactSet
- S&P Capital IQ

### Spreadsheet
- Build your own DCF model
- Excel/Google Sheets templates available

---

## 🔑 Key Takeaways

1. **Two approaches:**
   - Relative: Compare to peers/historicals
   - Absolute: DCF to find fair value

2. **Key multiples:**
   - P/E (earnings)
   - P/S (sales)
   - EV/EBITDA (operating cash flow)
   - P/B (book value)

3. **DCF steps:**
   - Forecast FCF
   - Choose discount rate
   - Calculate terminal value
   - Discount and sum

4. **Common mistakes:**
   - Ignoring growth
   - Wrong P/E type
   - Comparing across sectors
   - Ignoring debt

5. **The goal:** Find a margin of safety — buy below fair value

---

## ✅ Quick Check

Test your understanding:

1. **What's the difference between "trailing P/E" and "forward P/E"?**  
   _Hint: One looks back, one looks forward_

2. **Why might a tech stock have a P/E of 40x while a bank has a P/E of 8x?**  
   _Hint: Think about growth and risk_

3. **What does "margin of safety" mean?**  
   _Hint: Buy for less than what it's worth_

4. **If a stock's P/E is below its 10-year average, is it automatically a bargain?**  
   _Hint: There could be a reason why it's cheap_

---

## 📚 Further Reading

- "Security Analysis" by Benjamin Graham and David Dodd
- "The Intelligent Investor" by Benjamin Graham
- Damodaran Online (Aswath Damodaran) — free valuations
- Investopedia valuation guides

---

*Next up: Module 33 — Portfolio Theory Basics*

---

*Phase 5 Practical Applications is now 4/7 complete!*