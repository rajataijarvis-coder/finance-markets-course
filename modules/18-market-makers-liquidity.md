# Module 18: Market Makers & Liquidity

**Learning time:** 20-25 minutes  
**Prerequisites:** Module 17 (Clearing & Settlement) — understanding trade infrastructure helps explain why market makers matter

---

## 🤔 The Big Question

It's 2 PM on a Tuesday. You want to sell 500 shares of Tesla (TSLA). But who's going to buy them right now? What if no one wants to buy at this exact moment?

The answer: **market makers** — firms that always stand ready to buy or sell, ensuring you never have to wait for a counterparty.

---

## 📖 What Is a Market Maker?

A **market maker** is a firm (usually a bank or trading firm) that:
1. **Always quotes two prices** — a bid (buy price) and an ask (sell price)
2. **Always stands ready to trade** — at those prices, in either direction
3. **Makes money from the spread** — the difference between bid and ask

### The Simple Analogy

Think of a market maker like a currency exchange booth at an airport:

- They have **pounds** and **dollars** ready to trade
- They quote you a rate: "We'll buy your dollars at £0.78, sell you dollars at £0.82"
- The spread ( £0.04 ) is their profit
- They can do this all day because they have inventory

> 📊 **In stocks:** If a market maker quotes BP at £15.05 bid / £15.10 ask, they will buy at £15.05 and sell at £15.10 — regardless of whether other investors are currently trading.

---

## 🌍 How Market Makers Work

### The Bid-Ask Spread

```
Stock: BP

BID (Buy from them)      ASK (Sell to them)
£15.05                   £15.10
   │                        │
   └──── SPREAD = £0.05 ────┘

If you want to SELL 100 BP → Market maker buys at £15.05
If you want to BUY 100 BP  → Market maker sells at £15.10
```

### Who Are the Major Market Makers?

| Region | Market Makers |
|--------|----------------|
| **US** | Citadel Securities, Jane Street, Virtu Financial, Two Sigma |
| **UK/Europe** | UBS, Goldman Sachs, Morgan Stanley, Citi |
| **Multi-asset** | most major investment banks |

> 🥊 **Competition:** The more market makers competing for a stock, the tighter the spread (better for you as a trader).

---

## 💧 What Is Liquidity?

**Liquidity** simply means: *how easily can you buy or sell something without affecting its price?*

### High Liquidity

- You can trade large quantities instantly
- Prices move minimally when you trade
- Tight bid-ask spreads
- **Example:** Apple (AAPL) on NASDAQ — billions of shares trade daily

### Low Liquidity

- You might have to wait for a buyer/seller
- Your trade moves the price
- Wide bid-ask spreads
- **Example:** Small UK AIM stocks — might trade only a few times per day

```
HIGH LIQUIDITY (AAPL)          LOW LIQUIDITY (Small AIM stock)
─────────────────               ──────────────────────────────
Bid: £158.00                   Bid: £2.10
Ask: £158.05                   Ask: £2.40
Spread: £0.05 (0.03%)          Spread: £0.30 (14%)
                                
You can trade 10,000 shares    Trading 1,000 shares might
with almost no price impact    move price by 5%+
```

---

## 🔄 How Market Makers Provide Liquidity

### Continuous Presence

Market makers are obligated to provide quotes throughout the trading day:

- During market hours
- In normal market conditions
- Within certain size limits

This means **there's always someone on the other side of your trade.**

### The Process

```
1. Market maker receives order flow from many brokers
2. They balance their inventory (too many shares? they sell; too few? they buy)
3. They adjust quotes based on risk and inventory
4. They earn from the spread, not from predicting price direction
```

### Quote Example

```
BP shares trading around £15.00

Market Maker A quotes:
  Bid: £15.00  Ask: £15.05
  
Market Maker B sees this and quotes tighter:
  Bid: £15.02  Ask: £15.03
  
Competition drives spread to just £0.03!
(Better for traders — lower cost to trade)
```

---

## 📊 Why Liquidity Matters

### For Individual Investors

1. **You can always trade** — no waiting for a buyer/seller
2. **Fair prices** — you pay close to market price
3. **Lower costs** — tight spreads mean less "drag" on returns

### For Markets

1. **Price discovery works** — prices reflect actual supply/demand
2. **Market efficiency** — information is incorporated quickly
3. **Reduced volatility** — large trades don't move prices wildly

### The Cost of Poor Liquidity

Imagine trying to sell a property in a quiet town:

- It might take months to find a buyer
- You might have to accept below-asking price
- Legal fees and agent commissions add up

**Stocks can be the same** — illiquid stocks cost more to trade and take longer to sell.

---

## 🌍 Market Making Around the World

### US Equity Markets

- **NASDAQ** is a "dealer market" — dominated by market makers
- Major market makers: Citadel, Virtu, Jane Street
- **Spreads are tiny** — often just $0.01 for popular stocks
- **High-frequency trading (HFT)** firms now do most market making

### UK Equity Markets

- **LSE** uses order book + market makers
- **SETS** (Stock Exchange Electronic Trading Service) matches orders
- **SETSqx** combines order book for FTSE 250 + market maker quotes for smaller stocks
- Major banks provide liquidity as market makers

### European Markets

- **Euronext** (Paris, Amsterdam, Brussels) — hybrid model
- **Xetra** (Frankfurt) — mostly electronic order book
- MiFID II regulations govern market making activities

### Multi-Asset

Many market makers operate across asset classes:

```
Stocks   │  Bonds   │  FX      │  Commodities
─────────┼──────────┼──────────┼──────────────
Citadel  │  Citadel │  Citadel │  Glencore
Virtu    │  JPM     │  UBS     │  Trafigura
Jane St  │  GS      │  Citi    │  Vitol
```

---

## ⚠️ Potential Issues

### Market Manipulation Concerns

Market makers have a privileged position — they see order flow. Rules exist to prevent abuse:

- **Naked short selling** — selling shares you don't own (banned in UK/EU, restricted in US)
- **Quote stuffing** — flooding with fake quotes to slow competitors (illegal)
- **Layering** — placing fake orders to move price (illegal)

### Conflicts of Interest

Sometimes market makers are also:

- Brokers (they handle your orders)
- Investment bankers (they advise companies)
- Hedge fund managers (they trade for themselves)

> 🔍 **Regulation:** MiFID II (EU) and SEC rules (US) require transparency and prevent conflicts. But they still exist.

---

## 📈 How This Affects You

### Finding Liquidity

Before trading a stock, check:

1. **Average daily volume (ADV)** — higher = more liquid
2. **Bid-ask spread** — tighter = cheaper to trade
3. **Market maker presence** — more firms = more competition

### Example: BP vs. Small Oil Explorer

| Metric | BP (FTSE 100) | Small Oil Explorer (AIM) |
|--------|---------------|--------------------------|
| Daily Volume | 20-30 million shares | 50,000 shares |
| Bid-Ask Spread | £0.01-0.02 | £0.10-0.20 |
| Market Makers | 10+ | 1-2 |
| Impact of £100k trade | <0.1% price move | 5-10% price move |

---

## 💡 Key Takeaways

1. **Market makers provide quotes to buy and sell** — ensuring there's always a counterparty

2. **The bid-ask spread is their profit** — they make money without predicting price direction

3. **Liquidity = ease of trading** — high liquidity means tight spreads and minimal price impact

4. **Major market makers:** Citadel, Virtu (US); UBS, Goldman (UK/Europe)

5. **UK markets:** LSE uses SETS (order book) for FTSE stocks, SETSqx (market makers) for smaller stocks

6. **More competition = better prices** — more market makers = tighter spreads = lower costs for you

7. **Illiquid stocks cost more** — wide spreads and potential price impact add to trading costs

---

## 🧪 Quick Check (Answer in your head)

1. What is the "bid-ask spread"?  
   *(Answer: The difference between the price a market maker will buy at (bid) and sell at (ask))*

2. Why are market makers important for liquidity?  
   *(Answer: They always stand ready to trade, so you never have to wait for another investor)*

3. What's the difference between a highly liquid stock (like AAPL) and an illiquid one?  
   *(Answer: High liquidity = tight spreads, large volume, minimal price impact; illiquid = wide spreads, low volume, large price impact)*

4. How do market makers make money?  
   *(Answer: From the spread — buying at the bid and selling at the ask)*

---

## 📚 Next Up

**Module 19: Trading Mechanisms** — How orders actually travel from your phone to the exchange, and the different ways markets can function.

---

## 🤔 Questions?

Ask away! Common questions:
- "Can market makers refuse to trade with me?"
- "Do market makers ever lose money?"
- "What's the difference between a market maker and a broker?"
- "How do HFT firms affect regular traders?"

**When you're ready, reply: "Done with Module 18" or ask your questions!**