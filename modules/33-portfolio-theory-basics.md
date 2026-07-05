# Module 33: Portfolio Theory Basics

**Learning time:** 20-25 minutes  
**Prerequisites:** Modules 4, 31, 32 (Risk/Return + Company Analysis + Valuation)

---

## 🤔 The Big Picture

So far, we've covered:
- How to analyze a company (Module 31)
- How to value a stock (Module 32)

Now the question: **how do you build a portfolio of multiple investments?**

This is portfolio theory — the science of combining assets to optimize the risk-return trade-off.

In this module, we'll cover:
- Why diversification works
- The math behind portfolios
- Modern Portfolio Theory
- How to build a diversified portfolio

---

## 📖 The Power of Diversification

### The Intuition

Imagine you have $10,000 to invest. What's the safer approach?

**Approach A: All in one stock**
- Buy $10,000 of one company
- If it goes up 50% → you make $5,000
- If it goes down 50% → you lose $5,000

**Approach B: Spread across 10 stocks**
- Buy $1,000 each of 10 companies
- If one doubles and others stay flat → you make $1,000
- If one halves and others stay flat → you lose $500

**The result:** Same overall market exposure, but lower volatility.

> 💡 **Key insight:** Diversification reduces risk without necessarily reducing returns.

### The Math: Correlation

**Correlation** measures how two assets move together:
- **+1.0:** Perfect positive correlation (move together)
- **0.0:** No correlation (random)
- **-1.0:** Perfect negative correlation (move opposite)

**Why diversification works:**
- Correlated assets don't help (buying two oil stocks = same bet)
- Uncorrelated assets help (oil + tech = different drivers)
- Negative correlation is best (bonds + stocks)

### Real-World Example

```
Asset Class Correlations (approximate):
Stocks + Bonds:       ~0.1 (low)
Stocks + Gold:        ~0.0 (none)
US Stocks + UK Stocks: ~0.7 (high)
Tech + Energy:        ~0.3 (moderate)
```

**The takeaway:** Mix assets with low correlation.

---

## 🧮 Modern Portfolio Theory (MPT)

### What is MPT?

Developed by Harry Markowitz in 1952 (Nobel Prize winner), MPT shows how to construct portfolios that:
- Maximize return for a given level of risk
- Or minimize risk for a given level of return

### The Efficient Frontier

Imagine you could hold any combination of two assets:

```
Return
    │
 8% │                    ● Portfolio A
    │               ●        (high return, high risk)
 6% │            ●
    │         ●
 4% │      ●
    │   ●  (low return, low risk)
 2% │●
    └───────────────→ Risk (Std Dev)
       5%   10%   15%
```

The curve is the **efficient frontier** — the best portfolios for each risk level.

**Portfolios below the frontier** are inefficient (more risk, less return).
**Portfolios above the frontier** are impossible.

### The Magic of Diversification

Here's the key insight from MPT:

```
Portfolio Risk < Weighted Average of Individual Risks
(when correlation < 1)
```

**Example:**
```
Asset A: 10% return, 20% risk
Asset B: 5% return, 10% risk

50/50 Portfolio:
Expected return = 0.5 × 10% + 0.5 × 5% = 7.5%

If correlation = 1.0:
Portfolio risk = 0.5 × 20% + 0.5 × 10% = 15%

If correlation = 0.0:
Portfolio risk = 10.6% (diversification benefit!)

If correlation = -1.0:
Portfolio risk = 5% (perfect hedge!)
```

---

## 🎯 Building a Diversified Portfolio

### Step 1: Define Your Goals

Ask yourself:
- What's the investment horizon? (1 year? 10 years? 30 years?)
- What's the goal? (Retirement? House? Income?)
- What's your risk tolerance? (Lose 20% = fine? Or panic?)

### Step 2: Choose Asset Classes

**Core asset classes:**
- **Equities (stocks):** Growth
- **Fixed income (bonds):** Stability
- **Cash:** Liquidity
- **Alternatives:** Diversification (gold, real estate, commodities)

### Step 3: Allocate Across Asset Classes

**Typical allocations by age/risk:**

| Age | Stocks | Bonds | Cash |
|-----|--------|-------|------|
| 20s (aggressive) | 90% | 5% | 5% |
| 40s (moderate) | 70% | 25% | 5% |
| 60s (conservative) | 50% | 40% | 10% |
| 70s (retired) | 30% | 60% | 10% |

**The rule:** "100 minus your age in stocks"
- Age 30 → 70% stocks
- Age 60 → 40% stocks

> ⚠️ **This is a guideline, not a rule.** Your situation may differ.

### Step 4: Diversify Within Asset Classes

**Within stocks:**
- Geographic: US + UK + Europe + Asia
- Sector: Tech + healthcare + finance + consumer + energy
- Size: Large cap + mid cap + small cap

**Within bonds:**
- Government + corporate
- Short-term + long-term
- UK gilts + US Treasuries + European bonds

### Step 5: Rebalance Periodically

Markets change. Your allocation drifts. Rebalance to stay on target.

**Example:**
```
Target: 60% stocks / 40% bonds
After a year: 70% stocks / 30% bonds (stocks went up)
Action: Sell stocks, buy bonds to get back to 60/40

Result: "Buy low, sell high" automatically
```

---

## 🌍 Practical Portfolio Construction

### The Three-Fund Portfolio

The simplest diversified portfolio:

| Fund | What it is | Examples |
|------|------------|----------|
| US Stock Fund | Total US market | Vanguard S&P 500, iShares Core S&P 500 |
| International Stock Fund | Total world ex-US | Vanguard FTSE Global, iShares MSCI ACWI |
| Bond Fund | Total bond market | Vanguard Global Bond, iShares Global Aggregate |

**Three-fund example:**
```
60% Vanguard S&P 500 ETF (VOO)
20% Vanguard FTSE Global ETF (VEU)
20% Vanguard Total Bond Market ETF (BND)
```

### The Risk-Parity Approach

Don't allocate by %, allocate by risk contribution.

**How it works:**
- Bonds are less volatile than stocks
- To get equal risk contribution:
  - More in bonds, less in stocks
  - Or use leverage on bonds

**Result:** A portfolio that's less vulnerable to crashes.

### The All-Weather Portfolio

Popularized by Ray Dalio, the "All-Weather" portfolio aims to perform well in all economic environments:

```
Traditional All-Weather:
30% Stocks (US + international)
40% Long-term bonds
15% Intermediate bonds
7.5% Gold
7.5% Commodities
```

---

## 📊 Risk Metrics for Portfolios

### Volatility (Standard Deviation)

Measures how much returns swing:
- High volatility = large swings (risky)
- Low volatility = steady returns (safer)

**Benchmarks:**
- S&P 500: ~15% annual volatility
- Bonds: ~5% annual volatility
- 60/40 portfolio: ~10% annual volatility

### Sharpe Ratio

Risk-adjusted return:

```
Sharpe = (Portfolio Return - Risk-Free Rate) / Portfolio Volatility
```

**Interpretation:**
- > 1.0: Good
- > 2.0: Excellent
- < 0.5: Poor

**Example:**
```
Portfolio return: 10%
Risk-free rate: 3%
Volatility: 12%
Sharpe = (10 - 3) / 12 = 0.58
```

### Maximum Drawdown

The biggest peak-to-trough decline.

**Example:**
```
Portfolio hits $100,000 (peak)
Market crashes
Portfolio drops to $70,000 (trough)
Recovery to $100,000 (trough)
Maximum drawdown = -30%
```

---

## 🧪 Testing Your Portfolio

### Stress Testing

Ask: "How would this portfolio perform in..."

| Scenario | What to check |
|----------|---------------|
| 2008 crash | Stocks -40%, bonds +5% |
| 2022 inflation | Stocks -20%, bonds -15% |
| UK recession | GDP -2%, unemployment +5% |
| Interest rate spike | Bonds -10%, stocks -15% |

### The "Sleep Test"

Can you hold this portfolio through a 50% market drop?

- If yes → right risk level
- If no → too aggressive, add more bonds/cash

---

## 🔑 Key Takeaways

1. **Diversification:**
   - Don't put all eggs in one basket
   - Mix assets with low/negative correlation
   - Diversify across asset classes, geographies, sectors

2. **Modern Portfolio Theory:**
   - Can reduce risk without sacrificing return
   - Efficient frontier = best risk-return combinations
   - Correlation is key

3. **Portfolio construction:**
   - Define goals first
   - Choose asset allocation
   - Diversify within asset classes
   - Rebalance periodically

4. **Simple portfolios work:**
   - Three-fund portfolio
   - All-weather portfolio
   - Target-date funds

5. **Metrics:**
   - Volatility (standard deviation)
   - Sharpe ratio (risk-adjusted return)
   - Maximum drawdown

---

## ✅ Quick Check

Test your understanding:

1. **Why does diversification reduce risk?**  
   _Hint: It's about correlation_

2. **What's the efficient frontier?**  
   _Hint: The best risk-return combinations_

3. **If you're 30 years old, what allocation does the "100-age" rule suggest?**  
   _Hint: 100 - 30 = ?_

4. **Why should you rebalance your portfolio?**  
   _Hint: To maintain your target allocation_

---

## 📚 Further Reading

- "Portfolio Selection" by Harry Markowitz (original paper)
- "The Four Pillars of Investing" by William Bernstein
- Bogleheads wiki (bogleheads.org)
- Vanguard portfolio allocation guides

---

*Next up: Module 34 — Behavioral Finance*

---

*Phase 5 Practical Applications is now 5/7 complete!*