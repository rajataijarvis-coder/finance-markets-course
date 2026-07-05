# Module 12: Derivatives — Options

**Learning time:** 20-25 minutes  
**Prerequisites:** Module 11 (Futures & Forwards) — we build on derivatives concepts

---

## 🤔 The Big Picture

While futures give you an **obligation** to buy or sell, **options** give you the **right** — but not the obligation. This makes them fundamentally different: limited risk, unlimited reward potential.

Options are used for hedging, speculation, and generating income.

---

## 📖 What Are Options?

### Call Options (The Right to Buy)

```
CALL OPTION EXAMPLE
──────────────────────────────────────────────────────
You buy AAPL call option:
• Strike price: $180
• Expiry: 1 month
• Premium: $5 ($500 total for 100 shares)

At expiry:
• AAPL at $190 → You exercise, buy at $180, sell $190
  → Profit: $10/share - $5 premium = $5/share ($500)

• AAPL at $170 → You let it expire
  → Loss: $5 premium paid ($500)
```

### Put Options (The Right to Sell)

```
PUT OPTION EXAMPLE
──────────────────────────────────────────────────────
You buy AAPL put option:
• Strike price: $180
• Expiry: 1 month
• Premium: $4 ($400 total)

At expiry:
• AAPL at $160 → You exercise, buy at $160, sell $180
  → Profit: $20/share - $4 premium = $16/share ($1,600)

• AAPL at $190 → You let it expire
  → Loss: $4 premium paid ($400)
```

---

## 📊 Options Terminology

### Key Terms

| Term | Definition |
|------|------------|
| **Call** | Option to BUY the underlying |
| **Put** | Option to SELL the underlying |
| **Strike** | Price at which you can buy/sell |
| **Premium** | Cost to buy the option |
| **Expiry** | When option expires |
| **In the money (ITM)** | Option has intrinsic value |
| **Out of the money (OTM)** | Option is worthless at expiry |
| **At the money (ATM)** | Strike = current price |

### Intrinsic Value

```
INTRINSIC VALUE CALCULATION
──────────────────────────────────────────────────────
Call Option, Strike $100, Stock $120:
• Intrinsic = $120 - $100 = $20
• If premium paid = $5 → Profit at expiry = $15

Put Option, Strike $100, Stock $80:
• Intrinsic = $100 - $80 = $20
• If premium paid = $5 → Profit at expiry = $15

OTM options: Intrinsic = 0 (all premium is time value)
```

---

## 🌍 Options Markets

### Where Options Trade

| Exchange | Underlyings |
|----------|-------------|
| **CBOE (Chicago)** | Stock options, SPX (S&P 500) |
| **Eurex (Frankfurt)** | European stock options, Euro Stoxx 50 |
| **LSE (London)** | FTSE 100 options |
| **Euronext Paris** | French stock options |
| **NASDAQ** | Tech stock options |

### US Equity Options Example

```
APPLE (AAPL) OPTIONS CHAIN
──────────────────────────────────────────────────────
                CALLS                    PUTS
Strike   Price   Vol    Open Int    Price   Vol    Open Int
────────────────────────────────────────────────────────
$175     $8.40   12K    45K         $2.85   8K     62K    ← ITM
$180     $5.20   25K    89K         $4.10   15K    78K    ← ATM
$185     $2.95   38K   112K         $6.80   11K    54K    ← OTM
$190     $1.65   52K   156K         $9.50   7K     41K    ← OTM
```

---

## 💵 Options Strategies

### 1. Protective Put (Insurance)

```
PROTECTIVE PUT
──────────────────────────────────────────────────────
You own 100 shares of BP @ £4.50
Worried: Oil price might fall

Buy protective put:
• Strike: £4.50 (ATM)
• Premium: £0.20 (£20 total)
• Expiry: 3 months

At expiry:
• BP at £4.00 → Put exercised, sell £4.50
  → Only £0.50 loss instead of £0.50 + premium

• BP at £5.00 → Let put expire
  → Gain £0.50 - £0.20 = £0.30
  → Your stock is up, option loss limited to premium
```

### 2. Covered Call (Income)

```
COVERED CALL
──────────────────────────────────────────────────────
You own 100 shares of Shell @ £6.00
Want to generate income

Sell covered call:
• Strike: £6.50
• Premium received: £0.30 (£30)
• Expiry: 1 month

At expiry:
• Shell at £6.20 → Call expires worthless
  → Keep premium £30, still own shares

• Shell at £7.00 → Call exercised
  → Sell shares at £6.50
  → Profit: £0.50/share + £0.30 premium = £0.80
  → But you missed upside above £6.50!
```

### 3. Bull Call Spread

```
BULL CALL SPREAD (Limited risk bullish play)
──────────────────────────────────────────────────────
Buy call: Strike $180, Premium $5
Sell call: Strike $190, Premium $2
Net premium: $3 ($300)

At expiry:
• Stock at $200 → Long call in: $20 gain
  Short call out: $10 loss
  → Net: $17 profit ($1,700) = 567% return

• Stock at $175 → Both expire worthless
  → Loss: $300 (premium paid)

→ Limited risk, limited reward
```

### 4. Iron Condor (Neutral)

```
IRON CONDOR (Bet on range-bound prices)
──────────────────────────────────────────────────────
Sell put: Strike $170, Buy put: Strike $160 (protection)
Sell call: Strike $190, Buy call: Strike $200 (protection)

Net credit: $1.50 ($150)

At expiry:
• Stock at $175-185 → All options expire worthless
  → Keep $150

• Stock at $160 → Put exercised (loss $10/share)
  → Net loss after credit: $850

→ Profitable in range, limited loss outside
```

---

## ⚠️ Key Risks

### 1. Time Decay (Theta)

```
THETA ERODES OPTION VALUE
──────────────────────────────────────────────────────
Options lose value as expiry approaches:

Day 1: Option worth $5.00
Day 30: Option worth $0.50 (if stock unchanged)
Day 31: Option worth $0 (expiry)

→ The longer you hold, the more value you lose
→ Theta is highest for ATM options
```

### 2. Volatility Risk (Vega)

```
VEGA: OPTIONS HATE LOW VOLATILITY
──────────────────────────────────────────────────────
High volatility = Higher option prices
Low volatility = Lower option prices

If you buy options and volatility crashes:
• You can lose even if stock moves your way
• Time value plummets

Example: COVID crash 2020:
• Volatility spiked → Options surged
• Then cratered → Options lost value fast
```

### 3. Leverage Risk

```
OPTIONS LEVERAGE EXAMPLE
──────────────────────────────────────────────────────
Stock moves 10%: $100 → $110
Call option (2 months to expiry):
• Might move 50%+ (from $5 to $7.50)

That's 10x leverage!
But also: Stock falls 10% → Option might lose 80%
→ Leverage cuts both ways
```

### 4. Assignment Risk

```
EARLY ASSIGNMENT (AMERICAN OPTIONS)
──────────────────────────────────────────────────────
You sold a covered call
Stock suddenly spikes
Buyer exercises → You must sell stock NOW

Problem: You wanted to hold the stock!
This happens at worst times (when stock is high)
```

---

## 📈 Options vs Futures

```
OPTIONS VS FUTURES
──────────────────────────────────────────────────────
┌──────────────────┬──────────────────┬──────────────────┐
│                  │ Options          │ Futures          │
├──────────────────┼──────────────────┼──────────────────┤
│ Obligation?      │ Right, not duty  │ Obligation       │
│ Risk (buyer)     │ Limited to premium│ Unlimited       │
│ Leverage         │ High             │ Very high        │
│ Upfront cost     │ Premium only     │ Margin           │
│ Time decay       │ Yes (bad for buyers)│ None         │
│ Settlement       │ At expiry        │ Daily (mark-to) │
└──────────────────┴──────────────────┴──────────────────┘
```

---

## 💡 Key Takeaways

1. **Options = Rights, not obligations** — You can walk away

2. **Calls = Right to buy** — Profitable if stock rises above strike + premium

3. **Puts = Right to sell** — Profitable if stock falls below strike - premium

4. **Time decay is real** — Options lose value as expiry approaches

5. **Strategies abound** — Protective puts, covered calls, spreads, condors

6. **Leverage is significant** — 10x+ is common; risk is capped (buyer)

7. **Volatility matters** — High vol = expensive options; low vol = cheap

---

## 🧪 Quick Check

1. If you buy a call option with strike $100 and the stock rises to $120, what's your profit (excluding premium)?  
   *(Answer: $20 per share)*

2. What's the difference between a call and a put?  
   *(Answer: Call = right to buy; put = right to sell)*

3. What is "time decay" in options?  
   *(Answer: Options lose value as expiry approaches)*

4. Why might someone buy a protective put?  
   *(Answer: To insure against stock falling while still keeping upside)*

---

## 📚 Next Up

**Module 13: Derivatives — Swaps** — Custom agreements to exchange cash flows.

---

## 🤔 Questions?

Common ones:
- "Should I trade options?" (Start with understanding; options are complex)
- "What's theta decay?" (Time value erosion; biggest enemy of option buyers)
- "How do I know which strike to choose?" (ITM = more expensive, more protection; OTM = cheaper, more speculative)

**Reply: "Done with Module 12" when ready!**