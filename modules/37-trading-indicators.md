# Module 37: Trading Indicators (RSI, MACD, Bollinger)

**Learning time:** 20-25 minutes  
**Prerequisites:** Module 36 (Technical Analysis 101)

---

## 🤔 Why Use Indicators?

In Module 36, we learned to read charts and spot patterns. But patterns can be subjective. That's where indicators come in.

Indicators are mathematical calculations applied to price and volume data. They help:
- Identify overbought/oversold conditions
- Confirm trends
- Spot divergences (when price and indicator disagree)

In this module, we'll cover the "Big Three" indicators:
- RSI (Relative Strength Index)
- MACD (Moving Average Convergence Divergence)
- Bollinger Bands

---

## 📊 Indicator Categories

### Momentum Indicators
Measure speed of price change.  
**Examples:** RSI, Stochastic, ROC

### Trend Indicators
Confirm direction of trend.  
**Examples:** Moving averages, MACD

### Volatility Indicators
Measure how much price moves.  
**Examples:** Bollinger Bands, ATR

### Volume Indicators
Confirm moves with volume.  
**Examples:** OBV, VWAP

> 💡 **Key insight:** Use ONE indicator from each category. Too many = confusion.

---

## 🔷 RSI (Relative Strength Index)

### What is RSI?

RSI measures how fast price is changing. Scale: 0-100.

```
RSI > 70:  Overbought (might pull back)
RSI < 30:  Oversold (might bounce)
RSI = 50:  Neutral
```

### How to Calculate

```
RSI = 100 - (100 / (1 + RS))

RS = Average gains / Average losses
(over 14 periods, default)
```

### Trading with RSI

**1. Overbought/Oversold:**
```
RSI > 70: Consider selling
RSI < 30: Consider buying

Example:
Stock rallies to $100, RSI hits 85
→ Overbought → expect pullback
```

**2. Divergences (Advanced):**
```
Price makes lower low, RSI makes higher low = BULLISH DIVERGENCE
Price makes higher high, RSI makes lower high = BEARISH DIVERGENCE
```

**Example:**
```
Stock falls from $100 → $80 → $70
RSI:       40       35       38
(RSI made higher low despite lower price)
→ Bullish divergence → potential reversal
```

### RSI Pro Tips

- **Don't use in strong trends:** In strong uptrend, RSI can stay overbought for long
- **Use with support/resistance:** RSI + support = higher probability
- **Default setting:** 14 periods works for most timeframes

---

## 🔶 MACD (Moving Average Convergence Divergence)

### What is MACD?

MACD shows the relationship between two moving averages. It's both a trend and momentum indicator.

```
Components:
- MACD Line:     12-period EMA - 26-period EMA
- Signal Line:   9-period EMA of MACD Line
- Histogram:     MACD Line - Signal Line
```

### How to Read MACD

**1. Crossovers:**
```
MACD crosses ABOVE signal line → BUY
MACD crosses BELOW signal line → SELL
```

```
         Buy                    Sell
          ↓                      ↓
   ───────╲                    ╱──────
          ╲──────╲          ╱──────
                ╲────────╱──
                       ↑
                    Zero line
MACD Line: ───────────────────────────
Signal:   ───────────────────────────
Histogram:   ██       ████████
              ██    ███
              ██ ███
```

**2. Zero line crossover:**
```
MACD crosses above 0 → bullish
MACD crosses below 0 → bearish
```

**3. Divergence:**
```
Price makes new high, MACD makes lower high = BEARISH DIVERGENCE
Price makes new low, RSI makes higher low = BULLISH DIVERGENCE
```

### MACD Pro Tips

- **Best in trending markets:** Not as useful in ranging markets
- **Use with other indicators:** MACD + RSI = confirm signals
- **Default settings:** 12, 26, 9 work for most charts
- **Watch for lag:** Moving averages are lagging indicators

---

## 🔵 Bollinger Bands

### What are Bollinger Bands?

Volatility bands around a moving average.

```
┌─────────────────────────────────────────────┐
│          Upper Band (+2 std dev)            │
├─────────────────────────────────────────────┤
│  20-period SMA                              │
├─────────────────────────────────────────────┤
│          Lower Band (-2 std dev)            │
└─────────────────────────────────────────────┘
```

### How to Calculate

- **Middle Band:** 20-period SMA
- **Upper Band:** SMA + (2 × standard deviation)
- **Lower Band:** SMA - (2 × standard deviation)

### Trading with Bollinger Bands

**1. Mean Reversion:**
```
Price hits lower band → potential BUY
Price hits upper band → potential SELL
```

**2. Squeeze:**
```
Bands narrow = low volatility (setup for move)
Bands expand = high volatility (trend developing)
```

**3. Trend Identification:**
```
Price rides upper band = strong uptrend
Price rides lower band = strong downtrend
```

### Real Example

```
AAPL, Daily (2023):

Upper band: $195
Price:      $192 (near upper, possible pullback)
20 SMA:     $180
Lower band: $165

RSI: 68 (overbought)
MACD: Bullish cross (recent)
→ Mixed signals: Overbought but trending up
```

### Bollinger Pro Tips

- **Best for ranging markets:** In strong trends, price rides bands
- **Combine with RSI:** Double-check overbought/oversold
- **Squeeze is a setup:** Narrow bands often precede big moves

---

## 🎯 Combining Indicators

### The "Triple Confirmation" Strategy

Use three indicators from different categories:

| Category | Indicator | Signal |
|----------|-----------|--------|
| Momentum | RSI | Overbought/Oversold |
| Trend | MACD | Crossover |
| Volatility | Bollinger Bands | Touch bands |

**Example Entry (Long):**
```
1. RSI < 30 (oversold)
2. MACD crosses above signal (bullish)
3. Price hits lower Bollinger Band (value)
= Triple confirmation = Higher probability setup
```

### Indicator Conflict

What if indicators disagree?

```
RSI: Overbought (sell signal)
MACD: Bullish crossover (buy signal)
Bollinger: Riding upper band (sell signal)

→ RSI + Bollinger agree (sell)
→ MACD is wrong or early
→ Wait for MACD to confirm
```

> 💡 **Key insight:** When in doubt, default to the trend. In an uptrend, buy on dips. In a downtrend, sell on rallies.

---

## ⚠️ Indicator Pitfalls

### 1. Analysis Paralysis
Too many indicators = no clear signal. Use 1-2 per category.

### 2. Repainting
Some indicators (especially in crypto) can repaint. Use daily closes.

### 3. Lag
All moving average-based indicators lag. They're confirmation, not prediction.

### 4. Optimizing to Death
Adjusting parameters to fit past data = curve fitting. Doesn't work going forward.

### 5. Ignoring the Chart
Indicators are derived from price. Always look at the actual price chart first.

---

## 🔑 Key Takeaways

1. **Three indicator categories:**
   - Momentum (RSI)
   - Trend (MACD)
   - Volatility (Bollinger Bands)

2. **RSI:**
   - 0-100 scale
   - Overbought > 70, Oversold < 30
   - Divergences = early warning

3. **MACD:**
   - 12/26/9 default settings
   - Crossovers = entry signals
   - Zero line = trend direction

4. **Bollinger Bands:**
   - 20 SMA ± 2 standard deviations
   - Bands touch = potential reversal
   - Squeeze = setup for move

5. **Best practice:**
   - Use 1-2 indicators from different categories
   - Don't overcomplicate
   - Always check price chart first

---

## ✅ Quick Check

Test your understanding:

1. **If RSI is at 80, what does that tell you?**  
   _Hint: It's been moving fast in one direction_

2. **What's a "golden cross" involving MACD?**  
   _Hint: When the MACD line crosses above something_

3. **What does a Bollinger Band "squeeze" indicate?**  
   _Hint: Something is about to happen_

4. **Why is it dangerous to use 10 different indicators?**  
   _Hint: Analysis = no action_

---

## 📚 Further Reading

- "Trading in the Zone" by Mark Douglas (mindset)
- "Technical Analysis of the Financial Markets" by John Murphy
- TradingView indicators documentation
- "How I Made $2,000,000 in the Stock Market" by Nicolas Darvas

---

*Next up: Module 38 — Price Action & Support/Resistance*

---

*Phase 6: Active Trading is 2/10 complete!*