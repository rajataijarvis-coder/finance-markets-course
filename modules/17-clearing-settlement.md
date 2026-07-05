# Module 17: Clearing & Settlement

**Learning time:** 20-25 minutes  
**Prerequisites:** Module 16 (Stock Exchanges) — understanding how trades execute helps you appreciate what happens next

---

## 🤔 The Big Question

You click "Buy" on 10 shares of Apple. The trade executes instantly. You're happy. But what actually happened behind the scenes to make those shares yours? Who made sure the seller actually had shares to sell? Who made sure you actually paid?

The answer: **clearing and settlement** — the invisible plumbing that makes trading possible.

---

## 📖 The Two-Step Process

Every trade goes through two distinct phases:

### 1. Clearing — "The Deal Is Done"

**Clearing** is the process after a trade is executed where the exchange confirms:
- Who bought what
- Who sold what
- At what price
- Who owes what to whom

Think of it like a receipt at a shop — the transaction is recorded, but you haven't physically handed over money yet.

### 2. Settlement — "The Exchange Happens"

**Settlement** is when the actual exchange of shares and money happens. This is when:
- Shares move from seller to buyer
- Money moves from buyer to seller

> ⏱️ **Timing:** In most developed markets, settlement happens **T+1** (trade date plus 1 business day). In the US and UK, T+1 is now becoming the standard, replacing the older T+2.

---

## 🏗️ Who's Involved?

```
┌─────────────────────────────────────────────────────────────────────┐
│                     THE CLEARING ECOSYSTEM                         │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│   BUYER                           SELLER                            │
│      │                                │                             │
│      ▼                                ▼                             │
│   ┌──────┐                      ┌──────┐                           │
│   │Broker│                      │Broker│                           │
│   └──────┘                      └──────┘                           │
│      │                                │                             │
│      └────────┬─────────────────────┘                             │
│               ▼                                                    │
│        ┌──────────────┐                                            │
│        │  CLEARING   │  ← Confirms obligations                     │
│        │    HOUSE    │    (who owes what)                          │
│        └──────────────┘                                            │
│               │                                                    │
│               ▼                                                    │
│        ┌──────────────┐                                            │
│        │  CENTRAL     │  ← Holds securities                        │
│        │  DEPOSITORY  │    (shares, bonds)                         │
│        └──────────────┘                                            │
│                                                                     │
│   Money Flow: Buyer → Seller                                        │
│   Share Flow: Seller → Buyer                                        │
└─────────────────────────────────────────────────────────────────────┘
```

### The Key Players

1. **Brokers** — The firms you trade through (Fidelity, Charles Schwab, Hargreaves Lansdown)
2. **Clearing Houses** — The middlemen who guarantee trades (DTCC in the US, LCH in Europe/UK)
3. **Central Securities Depositories (CSDs)** — Where securities are held (DTC in US, CREST in UK, Euroclear in Europe)

---

## 🔒 Why Does This Matter?

### The Guarantee

Here's the key insight: **when you trade, you don't know the other person.**

You might buy 100 shares of BP from a stranger in Singapore. You have no idea if they actually own BP shares. You don't know if they'll disappear.

**That's where clearing houses come in.**

Clearing houses act as the **counterparty to both sides of every trade**:

- If you're the buyer, the clearing house guarantees you'll get your shares
- If you're the seller, the clearing house guarantees you'll get your money

> 💎 **This guarantee is crucial** — it's why markets can function at all. Without it, you'd have to vet every counterparty before trading, which would be impossible.

### How It Works in Practice

Let's say you buy £1,000 of BP shares through Hargreaves Lansdown:

```
Step 1: Trade Executes
   You click "Buy" → Trade happens on LSE at £15.00

Step 2: Trade Cleared (T+0 to T+1)
   LSE sends trade details to LCH (London Clearing House)
   LCH calculates: "Buyer owes £1,000, Seller owes 66.67 shares"

Step 3: Settlement (T+1)
   Your broker Hargreaves Lansdown sends £1,000 to LCH
   Seller's broker sends 66.67 BP shares to CREST (UK CSD)
   LCH verifies both sides → confirms the exchange
   Shares appear in your account
```

---

## 🌍 How Major Markets Handle This

### United States — DTCC

| Entity | Role |
|--------|------|
| **DTCC** (Depository Trust & Clearing Corporation) | Main clearing house |
| **DTC** (Depository Trust Company) | Holds securities |
| **NSCC** (National Securities Clearing Corporation) | Clears trades |

**Example:** When you buy Apple (AAPL) through a US broker:
1. Trade executes on NASDAQ
2. NSCC calculates obligations
3. DTC transfers shares from seller's account to buyer's account
4. Money moves through bank settlement

### United Kingdom — LCH & CREST

| Entity | Role |
|--------|------|
| **LCH** | Clearing house (part of LSE Group) |
| **CREST** | Central securities depository (now part of Euroclear) |

**UK settlement:** Uses CREST system — all UK-listed securities (FTSE 100, 250, etc.) are held electronically.

### Europe — European Central Securities Depository (ESMA)

The EU has been standardizing settlement across member states:

- **Euroclear** — Major CSD in Belgium, France, Netherlands, Sweden
- **Clearstream** — German CSD
- **Target2-Securities (T2S)** — EU-wide settlement platform

> 🌐 **Cross-border:** If you buy German SAP shares from a UK account, the trade might clear through LCH but settle through Clearstream. These systems talk to each other.

---

## ⚠️ What Happens When Things Go Wrong?

### Settlement Failures

Sometimes, on settlement day, one side can't deliver:

- **Buy-side failure:** Buyer can't pay → shares not delivered
- **Sell-side failure:** Seller doesn't have shares → money not received

**Consequences:**
- The clearing house steps in to fulfill the obligation
- Failed trades are "closed out" or resettled later
- Brokers may face penalties or margin calls

### The Case of GameStop (January 2021)

When retail traders piled into GameStop (GME), the trading volumes were so huge that settlement systems were strained:

- Brokers saw delays
- Some customers couldn't sell
- Clearing houses needed massive liquidity to guarantee trades

This event highlighted how critical — and fragile — clearing infrastructure can be during extreme market stress.

### Lehman Brothers (2008)

When Lehman Brothers collapsed, their clearing obligations were massive. The DTCC had to step in to ensure trades were settled, preventing a cascade of failures.

> 📊 **Lesson:** Clearing houses are "too big to fail" in practice — governments and central banks will backstop them because the alternative (no trading) is worse.

---

## 🔄 T+1: The Shift to Faster Settlement

### What's Changing?

Historically, most markets settled in **T+2** (trade date + 2 days). The US and UK are now moving to **T+1**:

- **US:** T+1 implementation began 2024, full rollout expected 2025
- **UK:** Also moving to T+1
- **EU:** Already implemented T+2, considering T+1

### Why Faster?

| Benefit | Explanation |
|---------|-------------|
| **Less risk** | Shorter window = less time for counterparty to fail |
| **Less capital** | Brokers need less capital sitting idle waiting to settle |
| **More efficiency** | Faster use of money and shares |
| **Better for trading** | More flexibility for day traders |

---

## 📊 Key Terminology

| Term | Meaning |
|------|---------|
| **Clearing** | Process of confirming trade details and calculating obligations |
| **Settlement** | Actual exchange of securities and money |
| **T+1 / T+2** | Trade date plus settlement days (T+1 = next business day) |
| **CSD** | Central Securities Depository — where securities are held |
| **Clearing House** | Entity that guarantees trades |
| **Delivery vs. Payment (DvP)** | Mechanism ensuring simultaneous exchange |
| **Fail** | When settlement doesn't happen on time |

---

## 💡 Key Takeaways

1. **Clearing and settlement are two separate steps** — clearing confirms obligations; settlement is the actual exchange

2. **Clearing houses guarantee trades** — this is why you can trade with strangers without worrying about counterparty risk

3. **Major clearing houses:** DTCC (US), LCH (UK), Euroclear (Europe)

4. **Settlement is moving to T+1** — faster than the old T+2 standard

5. **Central Securities Depositories (CSDs)** hold securities electronically — CREST (UK), DTC (US)

6. **Settlement failures are rare but serious** — clearing houses have mechanisms to handle them

---

## 🧪 Quick Check (Answer in your head)

1. What's the difference between clearing and settlement?  
   *(Answer: Clearing confirms who owes what; settlement is the actual transfer of shares and money)*

2. Who guarantees that you'll get the shares you bought?  
   *(Answer: The clearing house — DTCC in the US, LCH in the UK)*

3. What does "T+1" settlement mean?  
   *(Answer: Settlement happens the business day after the trade)*

4. What is CREST in the UK?  
   *(Answer: The central securities depository where UK shares are held electronically)*

---

## 📚 Next Up

**Module 18: Market Makers & Liquidity** — How these firms ensure there's always someone to buy when you want to sell, and vice versa.

---

## 🤔 Questions?

Ask away! Common questions:
- "Why does settlement take any time at all?"
- "What happens if my broker fails?"
- "Why is T+1 better than T+2?"
- "Can I lose money because of settlement problems?"

**When you're ready, reply: "Done with Module 17" or ask your questions!**