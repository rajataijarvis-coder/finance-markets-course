# Module 19: Trading Mechanisms

**Learning time:** 20-25 minutes  
**Prerequisites:** Module 18 (Market Makers & Liquidity) — understanding how liquidity is provided helps you understand how orders are matched

---

## 🤔 The Big Question

When you press "Buy" on your trading app, what actually happens? How does your order travel from your phone to the exchange? And once it's there, how does the exchange decide when and at what price to fill it?

The answer lies in **trading mechanisms** — the different ways markets can match buyers and sellers.

---

## 📖 The Journey of an Order

```
YOUR ORDER'S ADVENTURE
────────────────────────────────────────────────────────────

1. YOU
   Click "Buy 100 BP at £15.00"

          ▼
2. YOUR BROKER (Hargreaves Lansdown, Fidelity, etc.)
   Receives order, validates it, sends to exchange

          ▼
3. EXCHANGE (LSE, NYSE, NASDAQ)
   Receives order, matches with other orders

          ▼
4. CLEARING HOUSE (LCH, DTCC)
   Confirms trade details

          ▼
5. SETTLEMENT (CREST, DTC)
   Shares and money change hands

          ▼
6. YOU
   Shares appear in your account
```

Each of these steps involves different mechanisms. Let's focus on the exchange matching process.

---

## 🔄 Types of Trading Mechanisms

### 1. Order Book (Continuous Auction)

**How it works:**
- All buy and sell orders are collected in an "order book"
- Orders are matched continuously throughout the day
- Highest buy meets lowest sell = trade executes
- Price and time priority (first in at best price gets filled first)

**Used by:** NASDAQ, LSE (SETS), Euronext, most modern exchanges

```
ORDER BOOK EXAMPLE: BP SHARES

BUY ORDERS (Bids)              SELL ORDERS (Asks)
Price      Qty      Time        Price      Qty      Time
──────     ────     ─────       ─────      ────     ─────
£15.05     500      09:31:22    £15.10     300      09:30:45
£15.04     1,000    09:30:15    £15.11     500      09:31:55
£15.03     750      09:32:01    £15.12     1,000    09:29:30
£15.02     2,000    09:28:44    £15.15     750      09:32:12

Best bid: £15.05     Best ask: £15.10
Spread: £0.05

→ New buy order at £15.10 would immediately match with sell at £15.10
```

### 2. Dealer Market (Quote-Driven)

**How it works:**
- Market makers stand ready to buy and sell
- You trade with the dealer, not directly with other investors
- You see their quotes (bid/ask) and decide to trade

**Used by:** Some bond markets, some OTC markets, parts of FX market

### 3. Auction (Batch Trading)

**How it works:**
- Orders are collected but NOT executed immediately
- At specific times, all orders are matched at a single price
- This price clears the market (maximizes volume)

**Used by:** NYSE open/close auctions, some European exchanges, some commodities

```
AUCTION EXAMPLE: Opening Auction for Apple

All buy and sell orders come in:

BUY ORDERS                     SELL ORDERS
£158.50 × 10,000              £158.00 × 5,000
£158.30 × 25,000              £158.30 × 20,000
£158.00 × 50,000              £158.50 × 30,000

The auction algorithm finds the price where most volume matches:
→ Clearing price: £158.30
→ 20,000 + 25,000 = 45,000 shares trade at £158.30
```

### 4. Dark Pools (Alternative Trading Venues)

**How it works:**
- No public order book — orders are hidden
- Prices are often better (no market impact)
- Institutional investors use these to hide large trades

**Used by:** Large institutional traders, some hedge funds

> ⚖️ **Debate:** Dark pools are controversial — critics say they reduce transparency, defenders say they improve execution quality for large orders.

---

## 🌍 Trading Mechanisms Around the World

### United States

| Mechanism | Details |
|-----------|---------|
| **NASDAQ** | Pure order book, electronic from start |
| **NYSE** | Hybrid: order book + floor auctions for open/close |
| **Dark Pools** | Dozens of alternative venues (IEX, BATS, etc.) |

**IEX (Investors Exchange):**
- Featured in "Flash Boys" (Michael Lewis book)
- Added speed bumps to slow down HFT
- Now a regulated exchange

### United Kingdom

| Mechanism | Details |
|-----------|---------|
| **SETS** | Order book for FTSE 100/250 stocks |
| **SETSqx** | Hybrid: order book + market makers for smaller stocks |
| **SEAQ** | Quotes from market makers (older system) |
| **AIM** | Less formal, more flexible |

### Europe

| Exchange | Mechanism |
|----------|-----------|
| **Euronext (Paris/Amsterdam)** | Pure order book |
| **Xetra (Frankfurt)** | Order book, very liquid |
| **Euronext Milan** | Order book |

> 🇪🇺 **MiFID II:** EU regulations require more transparency and best execution across all venues — you must get the best price for your trade, regardless of venue.

---

## 📊 Order Types and How They Work

### Market Orders

- Execute immediately at best available price
- Guaranteed execution, not guaranteed price
- Use when: You need to get in/out fast

### Limit Orders

- Execute only at your specified price or better
- May not execute at all
- Use when: You want price control

### Stop Orders

| Type | Trigger | Purpose |
|------|---------|---------|
| **Stop-loss** | Price drops to trigger | Limit losses |
| **Stop-limit** | Price drops to trigger, then limit | Better price control |

### Hidden/Iceberg Orders

- Show only small portion to market
- Hide large orders from market impact
- Common with institutional traders

```
ICEBOOK ORDER EXAMPLE

You want to sell 50,000 BP shares

Instead of showing "SELL 50,000 @ £15.10"

You show: "SELL 1,000 @ £15.10" (iceberg)
Market sees only 1,000 — they don't know more behind

As each 1,000 is filled, another 1,000 appears
```

---

## ⏱️ The Rise of Electronic Trading

### Timeline

| Year | Development |
|------|-------------|
| 1971 | NASDAQ — first electronic exchange |
| 1990s | ECNs (Electronic Communication Networks) emerge |
| 2000s | Most floor trading moves electronic |
| 2010s | High-frequency trading dominates |
| 2020s | AI/algorithm trading grows |

### What This Means for You

**Benefits:**
- Faster execution (milliseconds)
- Lower costs (no floor brokers)
- Better prices (more competition)
- 24/7 trading in some markets

**Concerns:**
- Flash crashes (rapid sell-offs)
- HFT advantages over retail
- Less human oversight

### The Flash Crash (May 6, 2010)

Within minutes, US markets lost ~1 trillion dollars in value, then recovered:

- Sell orders triggered by algorithms
- HFT firms withdrew temporarily
- Market mechanism broke down briefly
- Circuit breakers stopped the bleeding

> 💡 **Lesson:** Electronic trading is fast and efficient, but mechanisms need safeguards (circuit breakers, speed bumps) to prevent crashes.

---

## 🎯 Best Execution

When you place a trade, your broker has a legal duty to get you the **best available price** considering:

1. **Price** — best bid/ask
2. **Cost** — commissions, fees
3. **Speed** — how fast
4. **Likelihood of execution** — will it actually fill?
5. **Size** — can you trade your full quantity?

> 📜 **Regulation:** MiFID II (EU) and SEC best execution rules require brokers to check multiple venues and route orders where they'll get best execution.

---

## 💡 Key Takeaways

1. **Order book** is the most common mechanism — orders matched continuously by price/time priority

2. **Auctions** happen at specific times — NYSE open/close, used for price discovery

3. **Dealer markets** rely on market makers — you trade with a dealer, not other investors

4. **Dark pools** hide order flow — used by institutions to avoid market impact

5. **Order types matter:** market orders guarantee execution, limit orders guarantee price

6. **Electronic trading** now dominates — milliseconds matter, but so do safeguards

7. **Best execution** is your right — brokers must get you the best price overall

---

## 🧪 Quick Check (Answer in your head)

1. What's the difference between a market order and a limit order?  
   *(Answer: Market order executes immediately at current price; limit order executes only at your specified price or better)*

2. How does an order book work?  
   *(Answer: Buy and sell orders are listed; highest buy matches lowest sell = trade executes)*

3. What is a dark pool?  
   *(Answer: Alternative trading venue where orders are hidden — no public order book)*

4. Why did the 2010 Flash Crash happen?  
   *(Answer: Automated selling triggered, HFT firms withdrew, market mechanisms temporarily broke down — circuit breakers stopped the fall)*

---

## 📚 Next Up

**Module 20: Market Regulation** — How governments and regulators keep markets fair and protect investors.

---

## 🤔 Questions?

Ask away! Common questions:
- "Why do dark pools exist if they're less transparent?"
- "Can my broker refuse to execute my trade?"
- "What's the difference between NYSE and NASDAQ's mechanisms?"
- "Are HFT firms unfair to regular investors?"

**When you're ready, reply: "Done with Module 19" or ask your questions!**