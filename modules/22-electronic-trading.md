# Module 22: Electronic Trading

**Learning time:** 20-25 minutes  
**Prerequisites:** Module 21 (Market Data & Indices) — understanding market measurement helps explain electronic trading's impact

---

## 🤔 The Big Question

In 1971, buying a stock meant calling a broker, who called another broker on the floor of the NYSE, who found a seller, and called back. Today, you click a button and the trade executes in milliseconds. What changed?

The answer: **electronic trading** — the technological revolution that transformed markets from floor-based pits to lightning-fast computer networks.

---

## 📖 The Evolution of Trading

### Before Electronics — The Old Way

```
1970s TRADING FLOW
─────────────────────────────────────────────────

1. YOU
   Call your broker: "I want to buy 100 BP"

2. YOUR BROKER
   Phone order to trading desk

3. BROKERAGE PHONE ROOM
   Phone to exchange floor broker

4. FLOOR BROKER (NY Floor of NYSE / LSE)
   Walk to trading pit, find seller
   Shout/hand signal to execute
   
5. FLOOR CLERK
   Record trade, notify both brokers

6. BACK OFFICE
   Process paperwork, settle in 5 days

TIME: Hours to days
COST: High (many humans involved)
```

### The Electronic Revolution

```
TODAY'S TRADING FLOW
─────────────────────────────────────────────────

1. YOU
   Click "Buy" on app

2. YOUR BROKER
   Electronic order sent to exchange

3. EXCHANGE COMPUTER
   Matches with sell order instantly

4. CLEARING HOUSE
   Confirms trade (T+1 settlement)

5. YOUR ACCOUNT
   Shares appear instantly

TIME: Milliseconds to seconds
COST: Low (computers, not people)
```

---

## 🌍 Key Milestones in Electronic Trading

| Year | Development | Impact |
|------|-------------|--------|
| **1971** | NASDAQ launches | First electronic stock market |
| **1980s** | ECNs emerge (Instinet, POSIT) | Alternative trading venues |
| **1990s** | Internet trading for retail | Anyone can trade from home |
| **1998** | SEC allows fully electronic exchanges | Physical floors start declining |
| **2000s** | High-frequency trading (HFT) emerges | Speed becomes everything |
| **2005** | Regulation NMS (US) | Best price protection |
| **2010s** | Mobile trading apps | Trading in your pocket |
| **2020s** | AI and algorithmic trading | Automated decision-making |

---

## 💻 How Electronic Trading Works

### The Technology Stack

```
YOUR TRADING APP
        │
        ▼
    BROKER SERVER
        │
        ▼
    ORDER ROUTING
        │
        ▼
    EXCHANGE NETWORK (FINRA, SIP, etc.)
        │
        ▼
    EXCHANGE MATCHING ENGINE
        │
        ▼
    ORDER BOOK UPDATED
        │
        ▼
    CONFIRMATION BACK TO YOU

Total time: Milliseconds
```

### What Is a Matching Engine?

The **matching engine** is the heart of an electronic exchange:

- Receives all orders
- Matches buyers and sellers
- Updates the order book
- Sends confirmations

**Speed:** Modern engines can process millions of orders per second.

### What Makes It Fast?

| Technology | What It Does |
|------------|--------------|
| **Fiber optics** | Light-speed data transfer |
| **Microwave towers** | Even faster than fiber for short distances |
| **Colocation** | Servers in exchange data centers (eliminates latency) |
| **FPGA chips** | Custom hardware for speed |
| **Cooling** | Prevents overheating at high speeds |

> ⚡ **Latency matters:** A difference of 1 millisecond can be worth millions in HFT. Firms literally race to be closer to exchange servers.

---

## 🎯 High-Frequency Trading (HFT)

### What Is HFT?

**High-frequency trading** uses computers to:
- Trade very fast (microseconds)
- Use massive data inputs
- Hold positions for very short periods
- Trade in enormous volumes

### How HFT Works

```
HFT STRATEGY EXAMPLE: Market Making

1. HFT computer sees 1,000 share buy order for Apple at £158.50
2. Instantly calculates: "I can sell from inventory at £158.51"
3. Fills the buy order, now long 1,000 shares
4. Simultaneously places sell order to offset position
5. Earns £0.01 × 1,000 = £10 profit
6. Entire sequence: < 1 millisecond
```

### Types of HFT Strategies

| Strategy | Description |
|----------|-------------|
| **Market making** | Provide liquidity, earn spread |
| **Statistical arbitrage** | Find price inefficiencies across markets |
| **Event-driven** | Trade news, earnings, economic data |
| **Liquidity detection** | Find hidden large orders |

### The Debate About HFT

**Arguments FOR:**
- Provides liquidity (more buyers and sellers)
- Tightens spreads (lower costs for everyone)
- Improves price discovery
- Increases market efficiency

**Arguments AGAINST:**
- Unfair advantage over regular investors
- Can cause flash crashes
- Benefits big firms, not small investors
- Too much complexity, systemic risk

> 📊 **Reality check:** HFT accounts for ~50-60% of US equity trading volume. Love it or hate it, it's a major part of modern markets.

---

## 📱 The Rise of Retail Trading Apps

### Democratization

The 2010s saw trading become accessible to everyone:

| Platform | Launch | Impact |
|----------|--------|--------|
| **Robinhood** | 2013 | Commission-free trading, mobile-first |
| **Fidelity** | Updated apps | Zero commissions |
| **Charles Schwab** | 2019 | Eliminated commissions |
| **eToro** | 2007 | Social/copy trading |

### What This Meant

**Before:** Trading was for professionals. High commissions ($10+ per trade), complex interfaces.

**After:** Anyone with a phone can trade. Zero commissions, simple apps, fractional shares.

> ⚠️ **Concern:** Easy access led to一些问题:
> - Robinhood GME mania (2021)
> - Memestocks (GameStop, AMC)
> - "Gamification" concerns (SEC investigated Robinhood)
> - Young traders taking on too much risk

---

## ⚡ The Infrastructure Behind Electronic Trading

### Data Feeds

| Feed | What It Provides |
|------|-------------------|
| **SIP (Securities Information Processor)** | Consolidated US market data |
| ** proprietary feeds** | Direct exchange feeds (faster) |
| **Depth of Book (DOO)** | Full order book (not just trades) |

### Co-location

**What it is:** Renting server space in the exchange's data center

**Why it matters:** Eliminates network latency

```
WITHOUT COLOCATION
Your order: London → New York data center → exchange
Latency: 70ms

WITH COLOCATION
Your server: Inside New York data center → exchange
Latency: 0.1ms

Difference: 700x faster
```

**Cost:** Millions per year. Only HFT firms and large institutions can afford it.

### The "Ping" Problem

When you trade through a retail app:

```
RETAIL TRADE PATH
You (London) → Broker server (US) → Exchange
                  │
                  ▼
            Routing delay (few ms)
                  │
                  ▼
            You see price after latency
```

**This is why retail traders sometimes get worse prices than HFT firms** — they see slightly stale prices.

---

## 🔒 Technology Risks and Safeguards

### Flash Crashes

Electronic trading can cause rapid crashes:

| Date | Event | Impact |
|------|-------|--------|
| **May 6, 2010** | Flash Crash (US) | ~$1 trillion lost in minutes |
| **Aug 24, 2015** | Flash Crash (US) | 1,000 point Dow drop in minutes |
| **Oct 7, 2016** | Sterling Flash Crash | 6% drop in minutes |

### Safeguards

| Protection | How It Works |
|------------|--------------|
| **Circuit breakers** | Trading halts if market drops too fast |
| **Limit Up/Limit Down** | Stock can't trade above/below price bands |
| **Speed bumps** | Exchange intentionally slows some trades (IEX) |
| **Kill switches** | Brokers can instantly halt all trading |

### The Role of Market Surveillance

Electronic trading generates massive data:

- **SEC/FCA** monitor for manipulation
- **FINRA** processes billions of daily transactions
- **AI/ML** used to detect patterns
- **Pattern recognition** spots spoofing, layering

---

## 🌐 Electronic Trading Around the World

### United States — Most Advanced

- All-electronic exchanges (NASDAQ)
- Hybrid models (NYSE — electronic + limited floor)
- Massive HFT presence
- Multiple alternative trading venues (dark pools)
- Best-in-class regulation

### United Kingdom — Mature and Liquid

- LSE fully electronic (SETS, SETSqx)
- Strong market maker presence
- European MiFID II rules apply
- Post-Brexit, competing with EU for business

### Europe — Fragmented but Harmonized

- MiFID II created single rules
- Multiple exchanges (Euronext, Xetra, Bolsa Madrid)
- Moving toward more competition
- T2S settlement platform

### Asia — Rapid Growth

- Japan: Fully electronic TSE
- Hong Kong: HKEX competitive globally
- Singapore: SGX electronic
- China: Rapid modernization

---

## 💡 Key Takeaways

1. **Electronic trading replaced floor trading** — milliseconds instead of days

2. **HFT dominates volume** — 50%+ of US trading, controversial but influential

3. **Co-location gives advantages** — being closer to exchange servers matters

4. **Retail apps democratized access** — zero commissions, mobile trading

5. **Flash crashes are a risk** — circuit breakers and safeguards exist

6. **The trading stack:** Your app → broker → exchange → clearing → settlement

7. **Technology creates advantages** — faster firms can profit from speed

---

## 🧪 Quick Check (Answer in your head)

1. What is high-frequency trading (HFT)?  
   *(Answer: Using computers to trade very fast, holding positions for extremely short periods)*

2. What is co-location?  
   *(Answer: Renting server space in the exchange's data center to reduce latency)*

3. What caused the 2010 Flash Crash?  
   *(Answer: Automated selling triggered, HFT withdrew, market mechanisms temporarily broke down)*

4. How have retail trading apps changed markets?  
   *(Answer: Made trading accessible to everyone, zero commissions, but raised concerns about gamification)*

---

## 📚 Next Up: Phase 4 — Central Banking & Policy

**Module 23: What Central Banks Do** — The institutions that control the money supply and set interest rates.

---

## 🤔 Questions?

Ask away! Common questions:
- "Is HFT unfair to regular investors?"
- "Why do flash crashes happen?"
- "Can I compete with HFT firms?"
- "What's the difference between NYSE and NASDAQ electronically?"

**When you're ready, reply: "Done with Module 22" or ask your questions!**

---

*🎉 Congratulations! You've completed Phase 3: Market Infrastructure!*

*Phase 4 covers central banking — the institutions that control the money supply and interest rates. These modules will help you understand how policy affects your investments.*