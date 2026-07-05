# Module 49: International Investing & Tax Considerations

**Learning time:** 20-25 minutes  
**Prerequisites:** Modules 46-48 (Tax foundations)

---

## 🤔 The Big Question

You've mastered domestic investing. You know your ISA from your SIPP, your 401k from your IRA.

But what about investing **abroad**?

Buying Apple (AAPL), Shell (SHEL), or SAP shares isn't just about picking global companies — it's about understanding how different countries tax your gains, dividends, and foreign investments.

In this module, we'll cover:
- How different countries tax international investments
- Foreign tax credits and treaties
- Currency considerations
- Reporting requirements
- Strategies for global portfolios

---

## 📖 The Basics of International Taxation

### Why It Gets Complicated

When you invest internationally, **two or more tax systems** can claim a piece of your returns:

```
Your Investment
        │
        ▼
┌───────────────────┐
│   Home Country   │  ← Tax on worldwide income/gains
└───────────────────┘
        ▲
        │
        ▼ (sometimes)
┌───────────────────┐
│  Source Country  │  ← Tax on income from their country
└───────────────────┘
        │
        ▼
        YOU ← What you actually keep
```

### Types of International Income

| Income Type | Example | Taxed Where? |
|-------------|---------|---------------|
| Capital gains | Sell LVMH shares (France) | Usually home country |
| Dividends | Apple (US) dividend | US (withholding) + home |
| Interest | European bonds | Usually source country |
| Rental income | UK property | UK only |

---

## 🏴󠁧󠁢󠁥󠁮󠁧󠁿 UK: International Investing

### UK Rules for Foreign Investments

**Good news:** The UK is relatively simple.

- **No tax on foreign capital gains** (if you're UK-domiciled)
- **No withholding tax** on most foreign dividends (but check treaty)
- **Reporting required:** If you have >£50,000 in foreign assets, report on SA1

### UK Dividend Tax on Foreign Stocks

```
Example: UK investor with US stocks
- Apple pays $0.96/share dividend
- US withholds: 0% (under US-UK treaty)
- UK taxes: 0% within ISA, 20% in taxable account
- With £40,000 in dividend income from US:
  Tax-free in ISA
  Taxable at 20% outside ISA
```

### Foreign Tax Credit (UK)

If you **do** pay foreign tax, you can claim credit:

```
Formula: Foreign tax paid × (UK tax rate / Source country rate)
         But cannot exceed UK tax on that income
```

**Example:**
```
German dividend: €1,000
German tax (25%): €250
UK tax (20% on same income): £200
Credit allowed: £200 (not £250)

You still owe: UK £200 - Credit £200 = £0
```

### UK Reporting Requirements

| Threshold | Requirement |
|-----------|-------------|
| >£50,000 foreign assets | Register for Self Assessment |
| >£10,000 foreign income | Register for Self Assessment |
| Foreign bank account | Report to HMRC (COP) |

---

## 🇺🇸 US: International Investing

### US Rules for Foreign Investments

**More complex:** US citizens are taxed on **worldwide income**.

- Must report all foreign financial accounts (FBAR)
- Foreign investments taxed similarly to US ones
- Foreign tax credits available

### Foreign Tax Credit (US)

```
Formula: (Foreign tax paid / Total foreign income) × US tax on that income
         Cannot exceed US tax on foreign income
```

**Example:**
```
UK dividend: £1,000 (~$1,250)
UK tax: £0 (under treaty)
US tax: $1,250 × 15% = $187.50

Since UK tax = $0, no FTC needed.
```

### Withholding Tax on Foreign Dividends

Many countries **withhold tax** on dividends paid to US persons:

| Country | Standard Rate | US Treaty Rate |
|---------|--------------|----------------|
| UK | 0% | 0% |
| Germany | 25% | 15% |
| France | 25% | 15% |
| Switzerland | 35% | 15% |
| Japan | 20.42% | 10% |

### Reporting Requirements (US)

```
┌─────────────────────────────────────────────────────┐
│            US FOREIGN REPORTING                    │
├─────────────────────────────────────────────────────┤
│                                                     │
│  • FBAR (FinCEN 114):                              │
│    Foreign accounts >$10,000 → due April 15        │
│                                                     │
│  • Form 5471:                                      │
│    Own >10% of foreign corporation                 │
│                                                     │
│  • Form 8865:                                      │
│    Foreign partnership interests                   │
│                                                     │
│  • Form 8938:                                      │
│    Foreign assets >$50,000 (single)                │
│    Foreign assets >$100,000 (married)              │
│                                                     │
└─────────────────────────────────────────────────────┘
```

### US Tax Example

```
Scenario: US investor, 24% bracket
Holds: 100 shares of Shell (UK-listed)

Shell dividend: £0.70/share × 100 = £70/year
UK withholding: 0%
US tax: 24% × $90 (converted) = ~$21.60

If held in taxable account, you owe US tax.
If held in IRA/401k, tax deferred or tax-free.
```

---

## 🇪🇺 Europe: International Investing

### EU Freedom of Capital

Good news: Within the EU, there's **free movement of capital**.

- No withholding tax on dividends between EU countries
- Parent-Subsidiary Directive: 0% withholding on EU dividends
- Savings Directive: Some automatic information exchange

### Cross-Border Tax in Europe

| From → To | Withholding | Notes |
|-----------|------------|-------|
| Germany → France | 0% (EU) | Under parent-subsidiary directive |
| France → Germany | 0% (EU) | Same |
| UK → Germany | 15% | Treaty rate |
| US → Any EU | Varies | Check treaty |

### European Tax Example

```
Scenario: German resident with French stocks (LVMH)

Dividend: €1,000
French withholding: 0% (EU directive)
German tax: 25% (if outside PEA)

Net: €1,000 × (1 - 0.25) = €750

If in PEA (Plan d'Épargne en Actions):
Held >5 years: 100% tax-free
```

---

## 💡 Key Strategies

### Strategy 1: Use Tax-Advantaged Accounts First

```
For international investments:
1. Max out ISA/401k/IRA first
2. Foreign stocks in these accounts = no foreign tax complications
3. Tax-free (or tax-deferred) growth

Example:
- UK investor: Put US stocks in ISA
- US investor: Put foreign stocks in 401k/IRA
```

### Strategy 2: Check Tax Treaties

Before investing in a foreign stock, check:
- Withholding tax rate (with/without treaty)
- Capital gains treatment (taxed where?)

**Resource:** Tax treaties are online. Find your home country's treaty network.

### Strategy 3: Consider ETFs Over Individual Stocks

**ETFs often have better tax treatment:**

| Structure | Tax Efficiency |
|-----------|----------------|
| ETF (accumulation) | No distribution = no tax |
| ETF (distributing) | Dividends taxed |
| Individual stock | Dividends + potential wash sales |

**Example:**
```
US-domiciled ETF (VTI):
- No UK stamp duty on purchase
- No UK CGT while held in ISA
- Cleanest for UK investors

UK-domiciled ETF (VWRL):
- US dividend withholding may apply
- But easier for UK tax reporting
```

### Strategy 4: Currency Hedging

**Consider whether you want currency exposure:**

```
Example: UK investor buys US stocks
- Dollar strengthens → More £ when selling
- Dollar weakens → Less £ when selling

If you want to reduce currency risk:
- Buy currency-hged ETFs (e.g., GBP-hedged S&P 500)
- Accept lower returns in exchange for stability
```

### Strategy 5: Keep Track of Cost Basis

**For foreign stocks, track in two currencies:**

```
Example: Bought Apple at $150, sold at $200
- USD gain: $50/share
- If GBP strengthened from $1.30→$1.50:
  - GBP cost: $150/1.30 = £115
  - GBP proceeds: $200/1.50 = £133
  - GBP gain: £18 (not £38!)

Currency moved against you.
This matters for CGT calculations.
```

---

## 📊 Real-World Examples

### Example 1: UK Investor with US Portfolio

```
Scenario: Sarah, UK resident
Portfolio:
├── Apple (NASDAQ: AAPL): +£3,000 gain
├── Microsoft (NASDAQ: MSFT): +£2,000 gain
└── Amazon (NASDAQ: AMZN): -£500 loss

Total gains: £5,000 - £500 = £4,500

In ISA: All tax-free!
In taxable:
- Annual exemption: £3,000
- Taxable: £1,500
- Tax at 20%: £300

Sarah's UK tax is simple - no US withholding issues in ISA.
```

### Example 2: US Investor with UK Dividend Stocks

```
Scenario: John, US citizen, 24% bracket
Holds: 200 shares of Shell (LSE: SHEL)

Shell dividend: £0.70 × 200 = £140/year
UK withholding: 0% (US-UK treaty)
US tax: $180 × 24% = $43.20

In taxable account: Owe $43.20
In IRA/401k: Tax deferred or tax-free
```

### Example 3: German Investor with US Tech

```
Scenario: Hans, German resident
Portfolio:
├── NVDA: +€8,000 gain (held 8 months)
├── Meta: +€3,000 gain (held 14 months)
└── Amazon: -€2,000 loss

Gains: €11,000 - €2,000 = €9,000

Tax treatment:
- NVDA (8 months): taxed as income at 25%
- Meta (14 months): tax-free (held >1 year)
- Amazon: loss carries forward

Net tax: €8,000 × 25% = €2,000
```

---

## ⚠️ Common Mistakes

### ❌ Mistake 1: Ignoring Foreign Withholding

Some countries withhold tax automatically. If you don't claim credit, you lose money.

### ❌ Mistake 2: Not Reporting Foreign Accounts

US: FBAR is strict. Failure to report can be $100,000+ penalties.

### ❌ Mistake 3: Double Taxation

Getting taxed twice (once in source country, once at home) without claiming credit.

### ❌ Mistake 4: Currency Confusion

Calculating gains in wrong currency. Track in both currencies.

### ❌ Mistake 5: Not Using Tax-Advantaged Accounts for Foreign Stocks

ISAs/401ks/IRAs simplify international investing enormously.

---

## 🔑 Key Takeaways

1. **International investing** adds complexity but also diversification
2. **UK:** Simple — no foreign CGT, minimal withholding, foreign tax credits available
3. **US:** Complex — worldwide income, FBAR reporting, wash sale rules apply
4. **Europe:** EU has free capital movement; check treaty rates
5. **Strategy:** Use ISA/401k/IRA for foreign stocks first
6. **Check treaties:** Can reduce withholding from 25%+ to 0-15%
7. **Track currencies:** Gains in one currency can be losses in another

---

## ✅ Quick Check

Test your understanding:

1. **UK Question:** Anna, a UK resident, holds Apple shares in her ISA. Apple pays a dividend. Does she pay UK tax? US tax?

2. **US Question:** Mike is a US citizen with a UK bank account containing £100,000. What reporting might he need to do?

3. **Strategy Question:** You want to invest in German stocks (SAP, Siemens). You're a UK resident. What's the tax-efficient way to do this?

---

## Answers

1. **UK Answer:** 
   - UK tax: **No** — ISAs are completely tax-free
   - US tax: **No** — ISA is a foreign account, but the account itself is tax-advantaged in the UK. US doesn't tax foreign accounts in UK tax-advantaged wrappers.

2. **US Answer:** 
   - **FBAR** (FinCEN 114) — must report if foreign accounts exceed $10,000 at any point during the year
   - Could also need **Form 8938** if total foreign assets exceed $50,000 (single)

3. **Strategy Answer:** 
   - Hold German stocks in a **Stocks & Shares ISA** or **SIPP** — both are UK tax-advantaged
   - No UK CGT, no UK income tax on dividends within these wrappers
   - Check US withholding if buying US-listed versions — UK-domiciled ETFs may be cleaner

---

*Next up: Module 50 — Estate Planning & Wealth Transfer Basics*