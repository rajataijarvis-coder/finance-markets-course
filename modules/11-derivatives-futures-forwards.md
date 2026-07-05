# Module 11: Derivatives — Futures & Forwards

**Learning time:** 20-25 minutes  
**Prerequisites:** Modules 6-10 (Equity, Bonds, Money Markets, Forex, Commodities)

---

## 🤔 The Big Picture

**Derivatives** are financial contracts whose value derives from something else — a stock price, an interest rate, a commodity price. Think of them as bets about future prices.

**Futures** and **forwards** are the foundational derivatives — contracts to buy or sell something at a future date, at a price agreed today.

---

## 📖 What Are Futures & Forwards?

### Forward Contracts

A **forward** is a private agreement between two parties:

```
FORWARD CONTRACT EXAMPLE
──────────────────────────────────────────────────────
You (buyer) agree with Bank (seller):
• Asset:     1,000 barrels of Brent oil
• Price:    $80/barrel
• Delivery: In 3 months
• Total:    $80,000

In 3 months:
• If oil is $100 → You gain $20,000
• If oil is $60 → You lose $20,000
→ Either way, you pay $80,000
```

### Futures Contracts

A **futures** is a standardized forward traded on an exchange:

```
FUTURES VS FORWARD
──────────────────────────────────────────────────────
┌─────────────────┬──────────────────┬──────────────────┐
│ Feature         │ Forward          │ Futures          │
├─────────────────┼──────────────────┼──────────────────┤
│ Trading         │ OTC (private)    │ Exchange         │
│ Terms           │ Customized       │ Standardized     │
│ Counterparty    │ One party        │ Clearing house   │
│ Settlement      │ At expiration    │ Daily (mark-to) │
│ Size            │ Custom           │ Fixed            │
│ Regulation      │ Minimal          │ Heavily regulated│
└─────────────────┴──────────────────┴──────────────────┘
```

---

## 🏛️ How Futures Markets Work

### Major Exchanges

```
GLOBAL FUTURES EXCHANGES
──────────────────────────────────────────────────────
• CME Group (Chicago) — Largest globally
  → S&P 500 futures, crude oil, gold, corn

• Intercontinental Exchange (ICE)
  → Brent oil, natural gas, sugar

• Euronext Paris
  → CAC 40 futures, European commodities

• Liffe (London)
  → Euribor, cocoa, coffee
```

### Contract Specifications

```
S&P 500 FUTURES CONTRACT (ES)
──────────────────────────────────────────────────────
Exchange:  CME (Chicago)
Ticker:    ES
Size:      $50 × S&P 500 index
Tick:      0.25 = $12.50
Months:    Quarterly (Mar/Jun/Sep/Dec)
Margin:    ~$12,500 (5-10% of value)
Settlement: Cash (no physical delivery)
```

---

## 📊 Understanding Futures Pricing

### The Forward Price

The price of a futures contract isn't random — it's determined by:

```
FORWARD PRICE FORMULA
──────────────────────────────────────────────────────
Forward Price = Spot Price × e^(r × T)

Where:
• Spot = Current price
• r = Risk-free interest rate
• T = Time to maturity

Example:
• Oil spot = $80
• 3-month rate = 5%
• Forward = $80 × e^(0.05 × 0.25) = $81.01
```

### Why This Works

```
CASH AND CARRY ARBITRAGE
──────────────────────────────────────────────────────
If futures too expensive:
1. Buy spot oil, store it
2. Sell futures at higher price
3. Hold to expiry, deliver, profit

If futures too cheap:
1. Short sell spot oil
2. Buy futures cheaper
3. Profit from the spread

→ This keeps prices aligned
```

### Mark-to-Market

Futures settle **daily**:

```
DAILY SETTLEMENT (MARK-TO-MARKET)
──────────────────────────────────────────────────────
Day 1: You buy oil futures at $80
Day 2: Oil closes at $82 → You gain $2,000
        (Cash credited to your account)

Day 3: Oil closes at $79 → You lose $1,000
        (Cash debited from your account)

→ Your gains/losses are realized daily
→ No waiting until expiration
```

---

## 🌍 Common Futures Markets

### Index Futures

```
INDEX FUTURES EXAMPLES
──────────────────────────────────────────────────────
S&P 500 (ES):
• Underlying: S&P 500 index
• Size: $50 × index
• Value @ 5,000: $250,000

FTSE 100 (Z):
• Underlying: FTSE 100
• £10 × index
• Value @ 8,000: £80,000

DAX (FDA):
• Underlying: DAX index
• €25 × index
```

### Commodity Futures

```
MAJOR COMMODITY FUTURES
──────────────────────────────────────────────────────
Energy:
• WTI Crude Oil (CL): 1,000 barrels
• Brent Crude Oil (BZ): 1,000 barrels
• Natural Gas (NG): 10,000 mmBtu

Metals:
• Gold (GC): 100 troy ounces
• Silver (SI): 5,000 troy ounces
• Copper (HG): 25,000 lbs

Agriculture:
• Corn (ZC): 5,000 bushels
• Soybeans (ZS): 5,000 bushels
• Wheat (ZW): 5,000 bushels
```

### Interest Rate Futures

```
RATE FUTURES
──────────────────────────────────────────────────────
• US Treasury Note Futures (TY)
• UK Gilt Futures (GLEN)
• Euro-Bund Futures (DE)

These bet on future interest rates!
If you think rates will fall → buy rate futures
```

---

## 💵 Trading Futures

### Long vs Short

```
GOING LONG (BUYER)
──────────────────────────────────────────────────────
• You expect price to RISE
• Buy futures, profit if price goes up
• Risk: Unlimited (price could fall forever)

GOING SHORT (SELLER)
──────────────────────────────────────────────────────
• You expect price to FALL
• Sell futures, profit if price drops
• Risk: Unlimited (price could rise forever)
```

### Margin Requirements

```
FUTURES MARGIN
──────────────────────────────────────────────────────
Instead of paying full value, you pay a margin:
• Contract value: $250,000 (S&P 500)
• Required margin: $12,500 (~5%)

This is leverage — control $250K with $12.5K
→ 20:1 leverage!

WARNING: You can lose MORE than margin posted
```

### Breakeven Calculation

```
BREAKEVEN EXAMPLE
──────────────────────────────────────────────────────
You buy S&P 500 futures at 5,000
You pay $12.50 per point = $6,250 per 1% move

To profit:
• Must cover commission
• Must exceed any contango costs

Let's say commission = $5/contract
Breakeven = 5,000 + (5/12.50) = 5,000.4
```

---

## ⚠️ Key Risks

### 1. Leverage Risk (MAJOR)

```
LEVERAGE GONE WRONG
──────────────────────────────────────────────────────
You buy S&P 500 futures at 5,000
Next day: Market falls 2% (to 4,900)

Your loss:
• 100 points × $50 = $5,000
• Your margin: $12,500
→ 40% loss in ONE DAY

→ Leverage cuts both ways dramatically
```

### 2. Counterparty Risk (Forwards)

```
OTC RISK
──────────────────────────────────────────────────────
You have a forward contract with a bank
Bank goes bankrupt → They might not pay

2008 crisis: Many forwards/derivatives defaulted
→ This is why clearing houses exist for futures
```

### 3. Basis Risk

```
BASIS RISK
──────────────────────────────────────────────────────
Basis = Spot Price - Futures Price

If you're hedging, basis can move against you:
• You hedge oil price risk
• But your specific oil doesn't match futures grade
• Hedge isn't perfect
```

### 4. Liquidity Risk

```
ILLIQUID CONTRACTS
──────────────────────────────────────────────────────
• Far-dated contracts often illiquid
• Can't exit position when you want
• Must hold to expiration
• Slippage can be massive
```

---

## 💡 Uses of Futures & Forwards

### 1. Hedging

```
HEDGING EXAMPLE: AIRLINE
──────────────────────────────────────────────────────
Airline needs 1M gallons of jet fuel in 6 months
Current price: $3/gallon
Worried: Price might spike to $4

Hedge: Buy 6-month fuel futures at $3.10
Result:
• If fuel → $4 → Futures profit offsets higher cost
• If fuel → $2.50 → Loss, but cheaper fuel offsets

→ Lock in price, eliminate uncertainty
```

### 2. Speculation

```
SPECULATION EXAMPLE
──────────────────────────────────────────────────────
You think tech stocks will rise
Buy S&P 500 futures

If you're right:
• 10% index gain → $25,000 on $12,500 margin
→ 200% return!

If wrong:
• 10% index loss → 200% loss
→ Margin exhausted, position closed
```

### 3. Arbitrage

```
ARBITRAGE OPPORTUNITY
──────────────────────────────────────────────────────
If futures mispriced vs spot:
• Buy spot, sell futures (cash and carry)
• Risk-free profit until prices align
→ Professional traders monitor this constantly
```

---

## 💡 Key Takeaways

1. **Derivatives derive value** — From underlying asset (stock, oil, rate)

2. **Forwards are OTC** — Custom private contracts; higher counterparty risk

3. **Futures are exchange-traded** — Standardized, cleared, daily settlement

4. **Leverage is massive** — 10-20x is common; small moves = big returns/losses

5. **Three main uses** — Hedging (risk management), speculation, arbitrage

6. **Daily settlement** — Mark-to-market means gains/losses realized daily

7. **Unlimited risk** — Both long and short can lose无限 (in theory)

---

## 🧪 Quick Check

1. What's the main difference between a forward and a futures?  
   *(Answer: Forwards are OTC/custom; futures are exchange-traded/standardized)*

2. If you expect oil prices to fall, what do you do with oil futures?  
   *(Answer: Go short — sell futures, profit if price drops)*

3. Why is leverage dangerous in futures trading?  
   *(Answer: Small price moves cause large percentage gains/losses on your margin)*

4. What is "mark-to-market"?  
   *(Answer: Daily settlement of gains/losses; your account balance changes daily)*

---

## 📚 Next Up

**Module 12: Derivatives — Options** — The right (not obligation) to buy or sell.

---

## 🤔 Questions?

Common ones:
- "Should I trade futures?" (Only if you understand leverage fully)
- "How do I hedge with futures?" (Match your exposure to underlying)
- "What's contango?" (When futures > spot — normal market)

**Reply: "Done with Module 11" when ready!**