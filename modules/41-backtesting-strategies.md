# Module 41: Backtesting Strategies

**Learning time:** 20-25 minutes  
**Prerequisites:** Modules 36-40 (Technical Analysis + Risk Management + Psychology)

---

## 🤔 Why Backtesting Matters

You have a strategy idea. It looks good on charts. But before risking real money, you need to know:

- Does it actually work historically?
- What's the win rate?
- What's the risk/reward?
- Does it work in different market conditions?

This is backtesting — testing your strategy on past data.

In this module, we'll cover:
- How to backtest properly
- What metrics to track
- Common backtesting mistakes
- Building confidence before trading live

---

## 📖 The Backtesting Process

### Step 1: Define Your Strategy

**Before testing, write down:**

```
Strategy: Bounce off support in uptrend

Entry Rules:
- Uptrend (higher highs, higher lows)
- Price touches support level
- Bullish reversal candle forms

Exit Rules:
- Stop: Below support by 1%
- Target: Previous high or 2:1 R/R

Timeframe: Daily
Market: Stocks, $1B+ market cap
```

> 💡 **Key insight:** If you can't write it down, you can't backtest it.

### Step 2: Collect Data

**Where to get data:**
- **Free:** Yahoo Finance, TradingView, Google Finance
- **Paid:** Ninjatrader, QuantConnect, Polygon

**What data you need:**
- OHLCV (Open, High, Low, Close, Volume)
- Date/time
- For as many symbols as possible

### Step 3: Run the Test

**Manual backtesting:**
- Scroll through charts
- Apply your rules
- Record every signal

**Automated backtesting:**
- Write code to test rules
- Run on historical data
- Get instant results

### Step 4: Analyze Results

**Key metrics to track:**

| Metric | What it tells you |
|--------|-------------------|
| Total trades | How often you trade |
| Win rate | Percentage of wins |
| Average win | Average profit |
| Average loss | Average loss |
| Profit factor | Gross wins / gross losses |
| Max drawdown | Largest peak-to-trough |

---

## 📊 Key Backtesting Metrics

### Win Rate

```
Win Rate = Wins / Total Trades
```

**Examples:**
- 60% win rate with 1:1 R/R = slight profit
- 40% win rate with 2:1 R/R = solid profit
- 30% win rate with 3:1 R/R = excellent profit

> 💡 **Key insight:** You don't need high win rate to make money. You need positive expectancy.

### Profit Factor

```
Profit Factor = Gross Profits / Gross Losses
```

**Interpretation:**
- > 1.5: Excellent
- 1.0-1.5: Good
- < 1.0: Losing money

**Example:**
```
20 wins × $100 = $2,000
20 losses × $50 = $1,000
Profit factor = $2,000 / $1,000 = 2.0
```

### Average Risk/Reward

```
Average R/R = Average Win / Average Loss
```

**Example:**
```
Average win: $150
Average loss: $75
Average R/R = 150 / 75 = 2:1
```

### Max Drawdown

```
Max Drawdown = (Peak - Trough) / Peak
```

**Example:**
```
Account peaks at $10,000
Drops to $8,000
Max drawdown = ($10,000 - $8,000) / $10,000 = 20%
```

**Why it matters:**
- A 50% loss requires 100% gain to recover
- Drawdown affects psychology

### Expectancy

```
Expectancy = (Win Rate × Avg Win) - (Loss Rate × Avg Loss)
```

**Example:**
```
50% win rate, 50% loss rate
Avg win: $100, Avg loss: $50
Expectancy = (0.5 × $100) - (0.5 × $50) = $50 - $25 = $25 per trade
```

**This is what matters.** Positive expectancy = edge.

---

## 🎯 The Backtest Checklist

### What to Test

1. **Total return:** Did you make money?
2. **Win rate:** How often do you win?
3. **Average win vs. loss:** Is R/R positive?
4. **Profit factor:** Is PF > 1.5?
5. **Max drawdown:** Can you survive the drawdown?
6. **Trades per year:** Is it tradable?
7. **Different market conditions:** Bull vs. bear vs. range

### Timeframes to Test

- **Minimum:** 1 year (to see different conditions)
- **Better:** 3-5 years
- **Best:** 10+ years (multiple cycles)

### Markets to Test

Test your strategy across different markets:

| Market | Example |
|--------|---------|
| Bull market | 2020-2021 |
| Bear market | 2022 |
| High volatility | 2020 COVID |
| Low volatility | 2017 |
| Ranging | 2015-2016 |

**Good result:** Works in most conditions  
**Bad result:** Only works in one condition

---

## ⚠️ Common Backtesting Mistakes

### Mistake 1: Overfitting

**What it is:** Tuning parameters to fit past data perfectly

**Example:**
```
Adjusting parameters: 
"Use RSI < 15 only, on Tuesdays, with AAPL only"
→ Perfect backtest, terrible live results
```

**The fix:**
- Test on out-of-sample data
- Use simple rules
- Less is more

### Mistake 2: Look-Ahead Bias

**What it is:** Using information that wouldn't be available at the time

**Example:**
```
"Buy before earnings because EPS will be high"
→ But you didn't know EPS before the report!
```

**The fix:**
- Only use data available at signal time
- Account for slippage

### Mistake 3: Survivorship Bias

**What it is:** Only testing stocks that still exist

**Example:**
```
Only test current S&P 500 stocks
→ Ignores companies that went bankrupt
→ Results are inflated
```

**The fix:**
- Include delisted stocks
- Test on wide universe

### Mistake 4: Ignoring Costs

**What it is:** Backtest without trading costs

**Example:**
```
Ignoring: commissions, spreads, slippage
→ 2% per trade costs = huge impact
```

**The fix:**
- Subtract realistic costs from results
- 0.1% per trade is reasonable

### Mistake 5: Curve Fitting

**What it is:** Adjusting the strategy until it "looks right"

**The fix:**
- Define rules before testing
- Don't change rules based on results
- Use out-of-sample validation

---

## 🧪 Paper Trading vs. Backtesting

### Backtesting (Historical)

**Pros:**
- Test many years quickly
- See performance across conditions
- Identify weaknesses

**Cons:**
- Historical ≠ future
- Can't trust execution quality
- No psychological preparation

### Paper Trading (Live Simulation)

**Pros:**
- Real-time experience
- Test execution quality
- Builds confidence

**Cons:**
- Takes time
- Doesn't test psychology fully
- Can have execution issues vs. real trading

### The Ideal Path

```
1. Define strategy → 2. Backtest → 3. Paper trade → 4. Live trade
```

---

## 🔑 Key Takeaways

1. **Backtesting:**
   - Test strategy on historical data
   - Before risking real money

2. **Key metrics:**
   - Win rate, profit factor, max drawdown
   - Expectancy (most important)

3. **What to test:**
   - Multiple market conditions
   - Different timeframes
   - Realistic costs

4. **Common mistakes:**
   - Overfitting
   - Look-ahead bias
   - Ignoring costs

5. **The process:**
   - Define rules → Backtest → Paper trade → Live

---

## ✅ Quick Check

Test your understanding:

1. **What's the difference between "overfitting" and a good strategy?**  
   _Hint: One fits past data perfectly, one has genuine edge_

2. **What's "profit factor" and why does it matter?**  
   _Hint: Gross wins divided by gross losses_

3. **Why is testing across different market conditions important?**  
   _Hint: You need to know if it works everywhere_

4. **What's the most important metric in backtesting?**  
   _Hint: Tells you if you have an edge_

---

## 📚 Further Reading

- "Quantitative Trading" by Ernest Chan
- "Advances in Financial Machine Learning" by Marcos López de Prado
- QuantConnect (quantconnect.com) — free backtesting
- Backtrader (backtrader.com) — Python backtesting

---

*Next up: Module 42 — Building a Trading System*

---

*Phase 6: Active Trading is 6/10 complete!*