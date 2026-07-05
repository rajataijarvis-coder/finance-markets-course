# Module 13: Derivatives — Swaps

**Learning time:** 20-25 minutes  
**Prerequisites:** Modules 11-12 (Futures & Forwards, Options) — we build on derivatives concepts

---

## 🤔 The Big Picture

**Swaps** are customized OTC contracts where two parties exchange cash flows over time. Unlike futures (standardized) or options (rights), swaps are bespoke agreements to swap payments.

The most common: **interest rate swaps** — exchanging fixed for floating payments. This is how trillions of dollars of interest rate exposure are managed.

---

## 📖 What Are Swaps?

### Basic Swap Structure

```
INTEREST RATE SWAP EXAMPLE
──────────────────────────────────────────────────────
You (Company A) vs Bank (Company B):

Agreement:
• You pay: Fixed 5% per year on £10M
• You receive: Floating (SONIA + 1%) on £10M
• Tenor: 3 years

Why do this?
• You have floating-rate debt (pay SONIA + 1%)
• Swap gives you fixed payments → now you're hedged
• Net: You pay 5%, bank pays SONIA + 1%
```

### Cash Flow Timeline

```
SWAP CASH FLOWS (Semi-Annual)
──────────────────────────────────────────────────────
        Your payment      Bank's payment
        (Fixed 5%)       (Floating)
─────────────────────────────────────────
Month 6:  £250,000        £255,000 (SONIA was 5.1%)
Month 12: £250,000        £262,000 (SONIA was 5.4%)
Month 18: £250,000        £248,000 (SONIA was 4.8%)
Month 24: £250,000        £260,000 (SONIA was 5.2%)
→ Net = Your fixed - bank's floating
```

---

## 🌍 Types of Swaps

### 1. Interest Rate Swaps

The most common swap type:

```
INTEREST RATE SWAP VARIANTS
──────────────────────────────────────────────────────
• Standard (Vanilla): Fixed ↔ Floating
• Basis: Floating ↔ Floating (different rates)
• Cross-currency: GBP fixed ↔ USD floating
• Amortizing: Notional decreases over time
• Step-up: Notional increases over time
```

### 2. Currency Swaps

```
CURRENCY SWAP EXAMPLE
──────────────────────────────────────────────────────
UK company needs euros, US company needs pounds:

UK Co → US Co: £10M at 5% GBP
US Co → UK Co: €12M at 6% EUR
(Assuming 1.20 GBP/EUR)

At maturity: Exchange principal back

Used for:
• Getting foreign currency
• Exploiting rate differentials
• Hedging currency exposure
```

### 3. Commodity Swaps

```
COMMODITY SWAP
──────────────────────────────────────────────────────
Airline ↔ Oil Company:

Airline pays: Fixed $80/barrel × 100,000 barrels
Oil Co pays: Floating (Brent monthly average)

Result: Airline locks in fuel cost at $80
→ No delivery; just net cash settlement
```

### 4. Credit Default Swaps (CDS)

```
CDS: INSURANCE AGAINST DEFAULT
──────────────────────────────────────────────────────
You buy protection (insurance) on BP bonds:
• Pay: 1.5% per year (£15,000 on £1M)
• Receive: If BP defaults, get £1M

2020: After oil crash, BP CDS spiked to 5%+
→ Market feared default risk
→ Now back to ~1.5% (stable)

This is "insurance" on debt — controversial!
```

---

## 📊 Swap Market Size

### Global Volumes

```
DERIVATIVES BY TYPE (Notional Outstanding)
──────────────────────────────────────────────────────
• Interest rate swaps: ~$400 trillion
• Currency swaps: ~$100 trillion
• Credit derivatives: ~$10 trillion
• Commodity swaps: ~$3 trillion

For comparison:
• Global GDP: ~$100 trillion
• Total world stock markets: ~$100 trillion

→ Swaps are ENORMOUS
```

### Key Participants

| Participant | Role |
|-------------|------|
| **Banks** | Market makers, arrange swaps |
| **Corporations** | Hedge interest rate/exchange exposure |
| **Hedge funds** | Speculate on rate movements |
| **Insurance companies** | Match assets/liabilities |
| **Central banks** | Policy operations |

---

## 💵 Pricing Swaps

### The Swap Rate

```
SWAP PRICING
──────────────────────────────────────────────────────
The "fixed" rate in an interest rate swap is set so that
the present value of fixed payments = present value of
floating payments (at inception).

This "fair rate" is determined by:
• Current yield curve (LIBOR, SONIA, SOFR)
• Credit spreads
• Market expectations of future rates

Traders use bootstrapping and curve fitting
to determine the "correct" swap rate
```

### Mark-to-Market

```
SWAP VALUE OVER TIME
──────────────────────────────────────────────────────
At inception: Value = 0 (fair rate set)

If rates FALL:
• Your fixed payments become MORE valuable
• Mark-to-market: You have an ASSET

If rates RISE:
• Your fixed payments become LESS valuable
• Mark-to-market: You have a LABILITY

→ Swaps can be huge gains/losses on balance sheets
```

---

## ⚠️ Key Risks

### 1. Counterparty Risk (MAJOR)

```
OTC RISK IN SWAPS
──────────────────────────────────────────────────────
Swaps are not cleared by exchanges
→ If your counterparty fails, you lose

2008 Crisis:
• AIG sold CDS protection
• When defaults loomed, AIG nearly collapsed
• Government bailed out — "too big to fail"

→ Now: More clearing, margin requirements
```

### 2. Interest Rate Risk

```
RATE RISK EXAMPLE
──────────────────────────────────────────────────────
You entered swap paying fixed 4%
Now rates are 6% → Your swap is an asset!
But if you unwind (exit early), you pay penalty

If rates DROP to 2%:
• Your fixed payments are expensive
• Mark-to-market shows huge loss
• Unwinding costs a fortune
```

### 3. Basis Risk

```
BASIS RISK
──────────────────────────────────────────────────────
You have floating-rate debt: SONIA + 1%
You enter swap: Pay fixed 5%, receive SONIA

But your debt is at SONIA + 1%, swap is at SONIA:
• When SONIA is 5%, you pay net: 5% - 5% + 1% = 1%
• When SONIA is 3%, you pay net: 5% - 3% + 1% = 3%
→ You still have exposure to your spread!
```

### 4. Liquidity Risk

```
UNWINDING SWAPS
──────────────────────────────────────────────────────
Swaps are not standardized:
• Can't just "sell" like futures
• Must find counterparty to take opposite position
• Or pay high termination fees

This makes exiting swaps expensive and slow
→ Not as liquid as futures/options
```

---

## 💡 Uses of Swaps

### 1. Hedging Interest Rate Risk

```
CORPORATE EXAMPLE
──────────────────────────────────────────────────────
Company has £100M debt at floating SONIA + 2%
 Concern: Rates might rise

Solution: Enter interest rate swap
• Pay fixed 5%, receive SONIA

Net result:
• Debt: SONIA + 2%
• Swap: 5% - SONIA
• Total: 5% + 2% = 7% fixed!

→ No more rate risk
```

### 2. Speculation

```
SPECULATOR USE
──────────────────────────────────────────────────────
Trader thinks rates will FALL:
• Enter swap: Pay fixed 4.5%, receive floating
• If rates fall to 3%:
  → Receives 3%, pays 4.5%
  → Net gain: 1.5% × notional

→ Massive bet on rates with minimal upfront
→ Just like being long/short futures, but custom terms
```

### 3. Asset-Liability Matching

```
INSURANCE COMPANY EXAMPLE
──────────────────────────────────────────────────────
Assets: £1B in 5-year bonds yielding 4%
Liabilities: £1B in 5-year policies paying floating

Problem: If rates fall, assets underperform
Solution: Pay fixed, receive floating on swap

Now both assets and liabilities are fixed:
→ Matched!
→ No interest rate risk
```

---

## 📈 Swaps vs Other Derivatives

```
COMPARISON
──────────────────────────────────────────────────────
┌──────────────┬────────────┬─────────────┬────────────┐
│ Feature      │  Swaps     │  Futures    │  Options   │
├──────────────┼────────────┼─────────────┼────────────┤
│ Trading      │    OTC     │  Exchange   │  Exchange  │
│ Standardized │    No      │    Yes      │    Yes     │
│ Obligation   │    Yes     │    Yes      │     No     │
│ Customizable │   Heavy    │    None     │    Some    │
│ Counterparty │    Risk    │    None     │    None    │
│ Regulation   │   Light    │   Heavy     │   Heavy    │
│ Typical use  │   Hedging  │  Speculation│   Insurance│
└──────────────┴────────────┴─────────────┴────────────┘
```

---

## 💡 Key Takeaways

1. **Swaps = Cash flow exchanges** — Custom OTC contracts between two parties

2. **Interest rate swaps most common** — Exchange fixed for floating payments

3. **Huge market** — ~$500 trillion notional; much larger than stock markets

4. **Counterparty risk** — Unlike futures, no clearing house; if counterparty fails...

5. **Not liquid** — Can't easily unwind; custom terms, harder to exit

6. **Used by banks, corporations** — For hedging interest rate and currency exposure

7. **CDS = Credit default swap** — Insurance against bond default; controversial

---

## 🧪 Quick Check

1. In a standard interest rate swap, what do you typically exchange?  
   *(Answer: Fixed interest payments for floating interest payments)*

2. What's the main advantage of swaps over futures?  
   *(Answer: Customizable terms — notional, maturity, payment dates)*

3. What's a key risk with swaps that doesn't exist with exchange-traded derivatives?  
   *(Answer: Counterparty risk — if the other party defaults, you lose)*

4. What is a CDS?  
   *(Answer: Credit Default Swap — insurance against a bond or loan defaulting)*

---

## 📚 Next Up

**Module 14: Credit Markets** — The world of private debt, syndicated loans, and credit analysis.

---

## 🤔 Questions?

Common ones:
- "Why do swaps exist?" (Custom hedging when futures don't fit)
- "Are CDS gambling?" (Controversial — used for both hedging and speculation)
- "How do I value a swap?" (Need yield curve + credit spreads)

**Reply: "Done with Module 13" when ready!**