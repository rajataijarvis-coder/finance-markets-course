# Module 7: Fixed Income (Bonds)

**Learning time:** 20-25 minutes  
**Prerequisites:** Module 6 (Equity Markets) — we build on market concepts

---

## 🤔 The Big Picture

While stocks represent **ownership**, bonds represent **debt**. When you buy a bond, you're lending money to a government or company in exchange for regular interest payments.

Bonds are the backbone of global finance — the bond market is actually **larger** than the stock market.

---

## 🏷️ What is a Bond?

A bond is a loan agreement between two parties:

```
BOND STRUCTURE
┌─────────────────────────────────────────────────────────┐
│  Issuer (borrower)    ──────►   Investor (lender)        │
│  Government/Company              You buy the bond       │
│                                                         │
│  You receive:          Issuer promises:                 │
│  • Regular interest    • Fixed coupon payments          │
│  • Principal back      • Your principal back at end    │
└─────────────────────────────────────────────────────────┘
```

### Key Bond Terms

| Term | Meaning |
|------|---------|
| **Face value (Par)** | Amount you get back at maturity (usually £100/$100/€100) |
| **Coupon** | Annual interest payment (as % of face value) |
| **Maturity date** | When issuer pays back principal |
| **Yield** | Your actual return (coupon ÷ price) |
| **Issuer** | Who owes the money |

### Example: UK Government Bond (Gilts)

```
Gilt: UK 5% Treasury 2030
┌────────────────────────────────────────────┐
│  Face value:     £100                      │
│  Coupon:         5% per year              │
│  Coupon paid:    £5 annually (or 2x £2.5) │
│  Maturity:       2030                      │
│  Current price:  £98                       │
│  Current yield:  5.1%                     │
└────────────────────────────────────────────┘
→ You pay £98, get £5/year + £100 in 2030
```

---

## 🌍 Global Bond Markets

### Government Bonds (Sovereign Debt)

| Country | Name | Index | Yield (2024) |
|---------|------|-------|--------------|
| **UK** | Gilts | FTSE Gilts | ~4-5% |
| **US** | Treasuries | Bloomberg US Treasury | ~4-5% |
| **Germany** | Bunds | REX Performance Index | ~2-3% |
| **France** | OAT | French Treasury | ~3% |
| **Japan** | JGBs | JGB Market | ~0.8% |

### US Treasury Quotes

```
US TREASURY 10-YEAR NOTE
┌────────────────────────────────────────────┐
│  CUSIP:    912828YM7                      │
│  Coupon:   4.25%                          │
│  Maturity: May 2034                       │
│  Price:    98-16 (98.5%)                  │
│  Yield:    4.38%                          │
│  Auction:  Monthly                        │
└────────────────────────────────────────────┘
```

### Corporate Bonds

Companies issue bonds too — usually with higher yields than government bonds:

```
CORPORATE BOND EXAMPLES
┌─────────────────────────────────────────────────────────┐
│  Company     │ Coupon  │ Maturity │ Yield  │ Rating  │
│──────────────│─────────│──────────│────────│─────────│
│  Apple       │ 3.25%   │ 2029     │ 3.4%   │ AAA     │
│  Shell       │ 4.875%  │ 2031     │ 4.9%   │ A+      │
│  BP          │ 5.5%    │ 2030     │ 5.2%   │ A       │
│  Vodafone    │ 6.0%    │ 2028     │ 6.8%   │ BB+     │
│  Tesco       │ 5.5%    │ 2032     │ 5.6%   │ BBB     │
└─────────────────────────────────────────────────────────┘
Higher yield = Higher risk (investors demand more interest)
```

---

## 📊 Bond Pricing & Yields

### The Price-Yield Relationship

Bonds have an interesting property: when prices fall, yields rise (and vice versa).

```
                 Yield
                   ↑
    High yields    │          \  (prices low)
    (prices low)  │           \_
                   │            \_
    Low yields     │             \___________
    (prices high) │              \__________ → Price
                   └─────────────────────────→
                   Par        Premium      Premium
                                (above par)
```

### Why This Matters

```
Example: You buy a bond
┌────────────────────────────────────────────────────────┐
│  Scenario A:                     Scenario B:          │
│  • Buy at £100 (par)             • Buy at £90 (discount)│
│  • Coupon 5% = £5                • Coupon 5% = £5       │
│  • Yield = 5%                    • Yield = 5.6%        │
│                                    (£5 ÷ £90 = 5.6%)     │
└────────────────────────────────────────────────────────┘
→ Cheaper price = Higher yield = Better return
```

### Current Yields Vary by Maturity

This creates the **yield curve**:

```
YIELD CURVE SHAPES

Normal (upward sloping):        Inverted (downward):
    ↑                              ↑
    │    /                          │\
    │   /                           │ \
    │  /                            │  \
    │ /                             │   \
    ├────────────────→              ├────\──→  ← Often signals recession
    Short    Long                   Short    Long
```

---

## ⚖️ Bond Ratings (Credit Risk)

Rating agencies judge issuer solvency:

| Rating | Meaning | Examples |
|--------|---------|----------|
| **AAA** | Highest quality, lowest risk | Apple, Microsoft, UK Gov |
| **AA** | Very high quality | Shell, BP, Unilever |
| **A** | High quality | Vodafone, Siemens |
| **BBB** | Medium quality (investment grade) | Tesco, Marks & Spencer |
| **BB** | Speculative (high yield) | Ford, Hertz |
| **B** | Highly speculative | Emerging market debt |
| **CCC/CC/C** | Near/default | Distressed debt |

> ⚠️ **Warning:** Once a bond drops below BBB-, it's "junk" — and yields skyrocket.

---

## 📈 Types of Bonds

### By Issuer

| Type | Examples | Risk Level |
|------|----------|-------------|
| **Government** | US Treasuries, UK Gilts, German Bunds | Lowest |
| **Municipal** | NY State bonds, London boroughs | Low-medium |
| **Corporate** | Apple bonds, Shell bonds | Medium-high |
| **Emerging Market** | Brazil, India, Turkey | High |

### By Coupon Type

| Type | Description |
|------|-------------|
| **Fixed rate** | Same coupon every year |
| **Floating rate** | Coupon adjusts (e.g., SONIA + 1%) |
| **Zero coupon** | No interest; bought at deep discount |

### By Currency

| Currency | Market |
|----------|--------|
| **GBP** | UK, London Stock Exchange |
| **USD** | US, NYSE |
| **EUR** | Eurozone, Euronext |
| **Multi-currency** | Global bonds in multiple currencies |

---

## 🛡️ Why Bonds Matter in a Portfolio

### The Role of Fixed Income

```
DIVERSIFIED PORTFOLIO
┌─────────────────────────────────────────────────────┐
│  Stocks (60%)          │  Bonds (40%)              │
│  ─────────────────     │  ──────────────────        │
│  Growth potential      │  Stability & income       │
│  Higher volatility     │  Lower volatility         │
│  Dividends + gains    │  Coupon payments          │
└─────────────────────────────────────────────────────┘
→ Bonds smooth out stock market swings
```

### Historical Performance

```
STOCKS VS BONDS (10-year average returns)
┌────────────────────────────────────────────────────┐
│  Asset Class      │  UK (GBP)  │  US (USD)        │
│  ─────────────    │  ──────────│  ─────────────   │
│  UK Equities      │   7.2%     │   -              │
│  UK Gilts         │   4.1%     │   -              │
│  US Equities      │   -        │   10.5%          │
│  US Treasuries    │   -        │   2.8%           │
│  Global Bonds     │   3.5%     │   3.5%           │
└────────────────────────────────────────────────────┘
→ Stocks return more over time; bonds are steadier
```

---

## 💵 How to Make Money in Bonds

### 1. Coupon Income (The Main Game)

```
You own: £10,000 in UK Gilts at 5% coupon
Your annual income: £500/year
Paid: Twice yearly (£250 each)
```

### 2. Price Appreciation

```
You buy: Bond at £95
Later:   Selling at £102
Profit:  £7 per £100 face = 7.4% gain
```

### 3. Reinvestment

```
Interest received: £500/year
Reinvested at 5%: After 20 years, you have £13,386
                    (compounding works for you too!)
```

---

## ⚠️ Key Risks

### 1. Interest Rate Risk

When rates rise, bond prices fall:

```
UK INTEREST RATES (recent example)
───────────────────────────────────
2019: 0.75%    → Gilts at 1.5% yield
2022: 4.5%     → Gilts at 4% yield (price FELL)
2024: 5.25%    → Gilts at 4.5% yield (price fell more)
```

> 📉 **Rule:** Longer maturity = more rate sensitivity

### 2. Inflation Risk

Fixed coupons lose purchasing power:

```
Inflation eats your coupon:
──────────────────────────────────
£1,000 bond at 5% = £50/year
If inflation is 8% → you're losing 3% in real terms!
```

### 3. Credit Risk (Default)

Issuer might not pay:

```
Examples:
• 2020: Oil crash → some energy bonds defaulted
• 2008: Lehman Brothers → unsecured bondholders lost ~$130B
• 2011: Greece → sovereign debt crisis (haircuts >70%)
```

### 4. Liquidity Risk

Some bonds trade rarely:

```
Illiquid bonds:
• Small corporate issuances
• Emerging market debt
→ You might not find a buyer when you want
```

---

## 📊 Bond vs Stock Comparison

```
┌────────────────────┬──────────────────┬──────────────────┐
│                    │    BONDS        │    STOCKS        │
├────────────────────┼──────────────────┼──────────────────┤
│ What you own       │ Debt (lender)   │ Equity (owner)   │
│ Income             │ Fixed coupon    │ Variable dividend│
│ Capital gains      │ Price changes   │ Price changes    │
│ If company fails   │ Paid first      │ Paid last        │
│ Volatility         │ Lower           │ Higher           │
│ Typical return     │ 2-5%            │ 5-10%            │
└────────────────────┴──────────────────┴──────────────────┘
```

---

## 💡 Key Takeaways

1. **Bonds are loans** — You lend money, get interest, then principal back

2. **Global market is huge** — Bigger than stocks; US, UK, Germany are key

3. **Yield ≠ coupon** — Price changes affect your actual return

4. **Rating matters** — AAA to junk; lower ratings = higher yields

5. **Rate risk is real** — When rates rise, bond prices fall

6. **Portfolio role** — Bonds provide stability and income, stocks provide growth

---

## 🧪 Quick Check

1. If a £100 bond pays £5/year and currently trades at £90, what's the yield?  
   *(Answer: 5.6% — £5 ÷ £90)*

2. What's the difference between a gilt and a corporate bond?  
   *(Answer: Gilts are UK government debt; corporate bonds are company debt)*

3. Why do bond prices fall when interest rates rise?  
   *(Answer: Existing bonds with lower coupons become less valuable)*

4. What happens to bondholders if a company goes bankrupt?  
   *(Answer: They're paid before shareholders — but after secured creditors)*

---

## 📚 Next Up

**Module 8: Money Markets** — Short-term debt, interbank lending, and how banks manage cash.

---

## 🤔 Questions?

Some common ones:
- "How do I actually buy bonds?" (Module 45 covers this)
- "What happens if the UK defaults?" (Impossible — BoE can always print pounds!)
- "Why do some bonds have negative yields?" (Happened in Europe 2019-2022 — complex!)

**Reply: "Done with Module 7" when ready!**