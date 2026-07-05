# Module 8: Money Markets

**Learning time:** 15-20 minutes  
**Prerequisites:** Module 7 (Fixed Income) — we build on bond concepts

---

## 🤔 The Big Picture

**Money markets** are where institutions borrow and lend for very short periods — from one day to one year. Unlike bonds (which have years-long maturities), money markets are about instant, low-risk transactions.

This is the plumbing of the financial system — banks, companies, and governments manage their short-term cash needs here.

---

## 🏧 What Are Money Markets?

### Definition

Money markets trade **short-term debt** — typically with maturities of:
- Overnight (1 day)
- 1 week to 1 month
- 3 months to 12 months

### Key Characteristics

| Feature | Money Markets | Bond Markets |
|---------|--------------|--------------|
| **Maturity** | < 1 year | 1-30+ years |
| **Credit risk** | Very low (high quality) | Varies |
| **Liquidity** | Extremely high | Medium to high |
| **Price volatility** | Minimal | Higher |
| **Typical investors** | Banks, institutions | Everyone |

---

## 🏦 Key Money Market Instruments

### 1. Treasury Bills (T-Bills)

**Government short-term borrowing:**

```
UK TREASURY BILLS (Gilts)
┌────────────────────────────────────────────────────┐
│  Maturity:  1, 3, or 6 months                     │
│  Issued by: UK Government (HM Treasury)           │
│  Denomination: £100,000+                           │
│  Yield:      ~5% (Apr 2024)                        │
│  Auction:    Weekly                                │
└────────────────────────────────────────────────────┘

Example: 3-month T-Bill
• You pay:    £98.50
• You get:    £100 (in 3 months)
• Return:     1.5% in 3 months ≈ 6% annualized
```

### 2. Commercial Paper

**Corporate short-term borrowing:**

```
COMMERCIAL PAPER EXAMPLE: APPLE
┌────────────────────────────────────────────────────┐
│  Issuer:     Apple Inc.                            │
│  Maturity:  90 days                                │
│  Amount:    $1 billion                            │
│  Coupon:    Discount (sold below face)            │
│  Rating:    A1+ (highest quality)                 │
│  Yield:     ~5.1%                                 │
└────────────────────────────────────────────────────┘
```

### 3. Banker's Acceptances

```
HOW A BANKER'S ACCEPTANCE WORKS
────────────────────────────────────────────────────────
1. Company (Importer) accepts a bill of exchange
2. Bank "accepts" it (guarantees payment)
3. Seller can sell it on secondary market
4. Buyer gets face value at maturity
→ It's like a post-dated cheque, bank-guaranteed
```

### 4. Repurchase Agreements (Repos)

**The most important money market instrument:**

```
REPO TRANSACTION
┌─────────────────────────────────────────────────────┐
│  Day 1:                                              │
│  ─────────                                           │
│  You sell:   Government bonds                       │
│  To:         Bank                                   │
│  Price:      £95                                   │
│  Agreement:  Buy back tomorrow at £95.01           │
│                                                       │
│  Day 2:                                              │
│  ─────────                                           │
│  You buy:    Same bonds at £95.01                  │
│  Cost:       £0.01 (overnight rate ≈ 4%)          │
└─────────────────────────────────────────────────────┘
→ It's collateralized overnight lending
```

> 💡 **Why repos matter:** Most short-term funding flows through repos. They're the overnight "heartbeat" of banking.

---

## 🌎 Global Money Markets

### Key Markets

| Country | Instrument | Key Rate |
|---------|------------|----------|
| **UK** | Overnight Indexed Swaps (SONIA) | ~5.2% |
| **US** | Secured Overnight Financing Rate (SOFR) | ~5.3% |
| **Europe** | Euro Short-Term Rate (ESTR) | ~3.9% |
| **Japan** | Tokyo Overnight Average (TONAR) | ~0.1% |

### UK Money Market Rates

```
UK OVERNIGHT RATES (2024)
┌─────────────────────────────────────────────────────┐
│  SONIA (Sterling Overnight Index Average)          │
│  ─────────────────────────────────────────────────│
│  Rate:         5.20%                               │
│  Used by:     Banks for overnight lending         │
│  Replaces:    LIBOR (phased out since 2021)       │
│  Administered: Bank of England                     │
└────────────────────────────────────────────────────┘
```

### US Money Market Rates

```
US OVERNIGHT RATES (2024)
┌─────────────────────────────────────────────────────┐
│  SOFR (Secured Overnight Financing Rate)          │
│  ─────────────────────────────────────────────────│
│  Rate:         5.31%                               │
│  Used by:     Treasury repos                      │
│  Volume:      ~$2 trillion daily                   │
│  Replaces:    LIBOR (targeted 2023)              │
└────────────────────────────────────────────────────┘
```

---

## 📊 How Money Market Rates Work

### Annualized Returns

```
Example: 91-day T-Bill at 5% discount
─────────────────────────────────────────────
Price paid:    £97.50
Face value:    £100.00
Interest:      £2.50 (91 days)
Annualized:    £2.50 × (365/91) = £10.02 per £100
Return:        10.02% annualized
```

### The Interbank Market

Banks lend to each other overnight:

```
INTERBANK LENDING (UK)
────────────────────────────────────────────────
Bank A has £10M excess cash → lends overnight
Bank B needs £10M cash → borrows overnight

Rate: SONIA + small spread
Typical spread: 0-10 basis points

Daily volume: £50+ billion in UK alone
```

---

## 🏛️ Who Uses Money Markets?

### Primary Participants

| Participant | Activity |
|-------------|----------|
| **Commercial banks** | Overnight borrowing/lending |
| **Central banks** | Implement monetary policy |
| **Large corporations** | Short-term cash management |
| **Money market funds** | Invest excess cash |
| **Broker-dealers** | Trading and market making |
| **Government** | Manage Treasury cash flow |

### Money Market Funds

```
MONEY MARKET FUND (Retail Example)
┌─────────────────────────────────────────────────────┐
│  Fund:   Vanguard Sterling Money Market Fund       │
│  Goal:   Preserve capital + modest income          │
│  Yield:  ~5%                                       │
│  Assets: ~£500M+                                   │
│  Invests: UK T-bills, bank deposits, repos         │
│  Liquidity: Same-day withdrawal                    │
└────────────────────────────────────────────────────┘
→ These are what "high interest savings accounts" actually invest in
```

---

## ⚠️ Key Risks

### 1. Credit Risk (Very Low But Not Zero)

```
Notable failures:
• 2008: Lehman Brothers commercial paper → investors lost ~$130B
• 2023: Some regional US banks → stress in bank deposits

→ Always check credit ratings of issuers
```

### 2. Liquidity Risk

Most money markets are highly liquid — but in crises, even these can freeze:

```
2008 Crisis:
• Repo markets seized up
• Central banks had to intervene
• Money market funds "broke the buck" (valued below $1)
```

### 3. Interest Rate Risk

Short-term rates change daily — your yield fluctuates:

```
2022 Example (UK):
• January: SONIA 0.75%
• September: SONIA 5.0%
→ Your returns rose 5x, but so did borrowing costs
```

### 4. Inflation Risk

If inflation exceeds rates, you lose purchasing power:

```
2022 UK:
• Money market yield: ~3%
• Inflation: ~10%
→ Real return: -7%
```

---

## 📈 Why Money Markets Matter

### For the Financial System

```
MONEY MARKETS: THE PLUMBING
────────────────────────────────────────────────────
Banks need cash every day:
• To meet withdrawal demands
• To make new loans
• To satisfy regulations

Money markets provide:
• Places to borrow overnight
• Places to invest excess cash
• Price discovery for short-term rates
```

### For You (Indirectly)

```
HOW MONEY MARKETS AFFECT YOU
────────────────────────────────────────────────────
1. Savings rates: Your bank uses money market rates
2. Mortgage rates: Short-term rates influence longer rates
3. Cash returns: Money market funds = your "savings" returns
4. Economic health: Stressed money markets = crisis signal
```

---

## 💡 Key Takeaways

1. **Money markets = short-term debt** — Overnight to 12 months

2. **Key instruments:** T-bills, commercial paper, repos, banker's acceptances

3. **Central to banking:** Banks borrow/lend here daily; trillions flow through

4. **Very low risk:** High-quality issuers; but 2008 showed it's not zero

5. **Rates matter globally:** SONIA (UK), SOFR (US), ESTR (Europe)

6. **Your savings use this:** Money market funds = pooled short-term debt

---

## 🧪 Quick Check

1. What's the typical maturity of money market instruments?  
   *(Answer: Overnight to 12 months)*

2. What's a repo transaction?  
   *(Answer: Selling securities with agreement to buy back — collateralized loan)*

3. What rate replaced LIBOR in the UK?  
   *(Answer: SONIA — Sterling Overnight Index Average)*

4. Why are money markets important for banks?  
   *(Answer: Banks need short-term funding daily to meet withdrawals and lend)*

---

## 📚 Next Up

**Module 9: Foreign Exchange (Forex)** — Trading currencies, exchange rates, and the biggest market in the world.

---

## 🤔 Questions?

Common ones:
- "How do I trade currencies?" (Module 45 covers practical access)
- "Why do exchange rates matter?" (Module 9 explains!)
- "What happened to LIBOR?" (It was discontinued after 2021 due to manipulation scandals)

**Reply: "Done with Module 8" when ready!**