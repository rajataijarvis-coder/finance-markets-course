# Module 21: Market Data & Indices

**Learning time:** 20-25 minutes  
**Prerequisites:** Module 20 (Market Regulation) — understanding how markets are measured and reported

---

## 🤔 The Big Question

When you hear "The S&P 500 rose 1.2%" or "FTSE 100 hits record high," what does that actually mean? How do we measure the performance of thousands of different stocks? And why should you care?

The answer: **market indices** — the tools we use to track how markets are doing, whether you're invested or not.

---

## 📖 What Is Market Data?

**Market data** is the information about trading:
- Prices
- Volumes
- Transactions
- Order flow

### Real-Time vs. Delayed Data

| Type | What It Is | Cost |
|------|------------|------|
| **Real-time** | Live prices as trades happen | Often expensive |
| **Delayed** | 15+ minutes old | Usually free |

**Example:** Bloomberg and Reuters provide real-time data (expensive). Yahoo Finance provides delayed data (free).

> 📊 **Why it matters:** Delayed data might show yesterday's price. If you're trading, you need real-time.

---

## 📈 What Is a Market Index?

A **market index** is a basket of stocks that represents a segment of the market.

### Why Indices Matter

1. **Measure performance** — "How did the market do today?"
2. **Benchmark returns** — How does your portfolio compare?
3. **Index funds** — Track an index to invest simply
4. **Derivatives** — Futures and options trade on indices

### Index Types

| Type | What It Tracks | Examples |
|------|----------------|-----------|
| **Broad market** | Large portion of market | S&P 500, FTSE All-Share |
| **Large cap** | Biggest companies | S&P 100, FTSE 100 |
| **Mid cap** | Medium companies | S&P 400, FTSE 250 |
| **Small cap** | Smaller companies | Russell 2000 |
| **Sector** | Specific industry | FTSE Technology, S&P Healthcare |
| **Style** | Growth vs. value | Russell 1000 Growth |
| **Global** | International | MSCI World, FTSE Global All Cap |

---

## 🌍 The Major Indices

### United States

| Index | Companies | What It Represents |
|-------|-----------|-------------------|
| **Dow Jones Industrial Average** | 30 | 30 largest US companies |
| **S&P 500** | 500 | 500 largest US companies (wide market) |
| **NASDAQ Composite** | 3,000+ | All NASDAQ stocks (tech-heavy) |
| **Russell 2000** | 2,000 | US small caps |
| **VIX** | — | Volatility index (fear gauge) |

**S&P 500 — The Big One:**
- Tracks 500 of the largest US companies
- ~80% of US market cap
- Weighted by market cap (bigger companies = bigger impact)
- Used as the primary benchmark for US stocks

```
S&P 500 WEIGHTING EXAMPLE (simplified)

Company          Market Cap      Weight in S&P 500
─────────────────────────────────────────────────
Apple            $3.0T           ~7.5%
Microsoft        $2.8T           ~7.0%
Amazon           $1.5T           ~3.8%
Nvidia           $1.2T           ~3.0%
Alphabet         $1.1T           ~2.8%
...and 495 more companies...
```

**The Dow:**
- Price-weighted (not cap-weighted)
- Sum of 30 stock prices divided by divisor
- Oldest US index (1896)
- Less representative than S&P 500

### United Kingdom

| Index | Companies | What It Represents |
|-------|-----------|-------------------|
| **FTSE 100** | 100 | Largest 100 UK companies |
| **FTSE 250** | 250 | Mid-cap UK companies |
| **FTSE 350** | 350 | Combined 100 + 250 |
| **FTSE All-Share** | ~600 | All UK main market stocks |
| **FTSE SmallCap** | Smaller | Small UK companies |
| **FTSE 100** | — | Often called "Footsie" |

> 🇬🇧 **UK Context:** FTSE 100 companies are often multinationals (BP, Shell, Unilever, HSBC). A falling FTSE 100 sometimes means the pound is strong (international earnings worth less in pounds).

### Europe

| Index | Companies | Region |
|-------|-----------|--------|
| **EURO STOXX 50** | 50 | Eurozone's 50 largest |
| **DAX** | 40 | Germany's largest |
| **CAC 40** | 40 | France's largest |
| **AEX** | 25 | Netherlands |
| **IBEX 35** | 35 | Spain |
| **FTSE MIB** | 40 | Italy |

**DAX (Germany):**
- Tracks 40 largest German companies
- SAP, Siemens, Deutsche Telekom, BMW
- Major European blue-chip index

**CAC 40 (France):**
- Tracks 40 largest French companies
- LVMH, TotalEnergies, Sanofi
- Named after "Cotation Assistée en Continu"

### Asia

| Index | Companies | Country |
|-------|-----------|--------|
| **Nikkei 225** | 225 | Japan |
| **TOPIX** | ~2,000 | Japan (broader) |
| **Hang Seng** | 80 | Hong Kong |
| **CSI 300** | 300 | China (Shanghai/Shenzhen) |
| **Nifty 50** | 50 | India |
| **KOSPI** | — | South Korea |

### Global/World Indices

| Index | Companies | Coverage |
|-------|-----------|----------|
| **MSCI World** | ~1,500 | Developed markets |
| **MSCI Emerging Markets** | ~1,400 | Developing markets |
| **FTSE Global All Cap** | ~5,000 | Global (developed + emerging) |

---

## 🏗️ How Indices Are Calculated

### 1. Price-Weighted

**Formula:** Sum of all stock prices ÷ Number of stocks

**Used by:** Dow Jones Industrial Average

**Problem:** A $100 stock has more impact than a $10 stock, regardless of company size.

### 2. Market Cap-Weighted (Most Common)

**Formula:** Each stock weighted by its market cap ÷ Total market cap

**Used by:** S&P 500, FTSE 100, most modern indices

**How it works:**
- Apple ($3T market cap) has more weight than a $10B company
- Reflects actual market representation
- Automatically rebalances as stocks grow/shrink

### 3. Equal-Weighted

**Formula:** Each stock gets equal weight regardless of size

**Used by:** Some S&P equal-weighted variants

**Example:** In an equal-weighted S&P 500, Apple and a $100M company both get 0.2% weight.

### 4. Fundamental-Weighted

**Formula:** Weight by fundamentals (earnings, dividends, book value)

**Used by:** Some smart-beta indices

---

## 📊 Index Calculation Example

Let's build a simple index:

```
DAY 1: Index starts
Stock A: £100 × 10M shares = £1,000M market cap
Stock B: £50  × 20M shares = £1,000M market cap
Stock C: £25  × 20M shares = £500M  market cap
Total: £2,500M
Index value: 100 (base)

DAY 2: Prices change
Stock A: £110 (+10%) → £1,100M
Stock B: £48  (-4%)  → £960M
Stock C: £30  (+20%) → £600M
Total: £2,660M

Index change: (2660/2500 - 1) = +6.4%
Index value: 106.4
```

---

## 🎯 Why Indices Matter to You

### 1. Benchmarking

Did your portfolio return 8% this year? That's only good if the S&P 500 returned 5%. If it returned 15%, you underperformed.

```
YOUR PORTFOLIO vs BENCHMARK
─────────────────────────────────────────────────
Your return:           +8%
S&P 500 return:       +15%
FTSE 100 return:      +4%
                           
You: Outperformed FTSE 100 ✓
You: Underperformed S&P 500 ✗
```

### 2. Index Funds and ETFs

Instead of picking stocks, you can buy an index fund:

| Fund Type | What It Does | Examples |
|-----------|--------------|----------|
| **Index mutual fund** | Directly tracks index | Vanguard S&P 500, Fidelity FTSE 100 |
| **ETF (Exchange-Traded Fund)** | Trades like stock, tracks index | iShares Core S&P 500 (IVV), Vanguard FTSE 100 (VUKE) |

**Benefits:**
- Low fees (often under 0.1%)
- Diversification instant
- Simple, passive approach
- Historically beats most active managers

### 3. Derivatives

Indices enable hedging and speculation:

- **Index futures** — Bet on future index level
- **Index options** — Buy protection or speculation
- **Contracts for Difference (CFDs)** — Trade index movements

> 📈 **Popular:** The "E-mini" S&P 500 futures (ES) is the most traded futures contract in the world.

---

## 🔄 Index Providers

| Provider | Indices | Examples |
|----------|---------|----------|
| **S&P Dow Jones Indices** | S&P 500, Dow, | S&P 500, Dow Jones, S&P/ASX 200 |
| **MSCI** | MSCI indices | MSCI World, MSCI Emerging Markets |
| **FTSE Russell** | FTSE indices | FTSE 100, FTSE 250, Russell 2000 |
| **STOXX** | European indices | EURO STOXX 50, DAX |
| **Bloomberg** | Bloomberg indices | Bloomberg World, Bloomberg Commodity |
| **ICE** | ICE indices | ICE US 100, ICE BofA indices |

---

## 💡 Key Takeaways

1. **Market indices track groups of stocks** — representing different market segments

2. **S&P 500** tracks 500 largest US companies — weighted by market cap

3. **FTSE 100** tracks 100 largest UK companies — called "Footsie"

4. **Most indices are market-cap weighted** — bigger companies have more impact

5. **Indices enable passive investing** — index funds and ETFs let you track the whole market cheaply

6. **Use indices as benchmarks** — compare your portfolio performance against relevant index

7. **Global indices exist** — MSCI World, FTSE Global All Cap track international markets

---

## 🧪 Quick Check (Answer in your head)

1. What's the difference between FTSE 100 and FTSE 250?  
   *(Answer: FTSE 100 = 100 largest UK companies; FTSE 250 = next 250 largest (mid-cap))*

2. How is the S&P 500 weighted?  
   *(Answer: By market capitalization — bigger companies have more impact)*

3. Why use an index as a benchmark?  
   *(Answer: To compare your portfolio performance against "the market")*

4. What's an ETF?  
   *(Answer: Exchange-Traded Fund — trades like a stock, tracks an index)*

---

## 📚 Next Up

**Module 22: Electronic Trading** — How technology transformed markets, from the first computer trades to today's high-frequency trading.

---

## 🤔 Questions?

Ask away! Common questions:
- "Why does the S&P 500 matter more than the Dow?"
- "Can I buy an index directly, or do I need a fund?"
- "What's the difference between MSCI and FTSE Russell?"
- "Do index funds really beat active managers?"

**When you're ready, reply: "Done with Module 21" or ask your questions!**