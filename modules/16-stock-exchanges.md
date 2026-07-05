# Module 16: Stock Exchanges

**Learning time:** 20-25 minutes  
**Prerequisites:** Modules 1-6 (especially Module 6 on Equity Markets)

---

## 🤔 The Big Question

When you buy a share of Apple or BP, where does that transaction actually happen? How does your buy order reach a seller you've never met?

The answer: **stock exchanges** — the digital marketplaces where buyers and sellers find each other.

---

## 📖 What Is a Stock Exchange?

A **stock exchange** is a marketplace where people trade shares of companies. It's not a physical building anymore — it's a sophisticated electronic network that matches buyers with sellers.

Think of it like eBay for company ownership:
- **Sellers** list shares they want to sell
- **Buyers** place orders for shares they want to buy
- The exchange matches them instantly

### Why Exchanges Matter

1. **Liquidity** — You can buy or sell shares quickly without finding a specific buyer/seller
2. **Price discovery** — The exchange aggregates all orders to find the "fair" price
3. **Trust** — The exchange guarantees trades, so you don't worry about the other party defaulting
4. **Transparency** — Everyone sees the same prices and trading data

---

## 🌍 The World's Major Stock Exchanges

### United States — The World's Largest Market

| Exchange | Founded | Notable Companies |
|----------|---------|-------------------|
| **NYSE** (New York Stock Exchange) | 1792 | Berkshire Hathaway, Disney, Coca-Cola |
| **NASDAQ** | 1971 | Apple, Microsoft, Amazon, Tesla, NVIDIA |

**Key difference:**
- **NYSE** — Historic, floor-based trading (though now mostly electronic), tends to list larger, established companies
- **NASDAQ** — All-electronic from day one, heavy tech focus, shorter history

> 📊 **By the numbers:** The NYSE and NASDAQ together account for roughly 60% of global stock market capitalization.

**Examples:**
- Apple trades on NASDAQ as **AAPL**
- Tesla trades on NASDAQ as **TSLA**
- JPMorgan Chase trades on NYSE as **JPM**

### United Kingdom — The City of London

| Exchange | Notes |
|----------|-------|
| **LSE** (London Stock Exchange) | One of the oldest exchanges in the world, dating back to 1698 |

**FTSE Indices:**
- **FTSE 100** — 100 largest UK companies (called "Footsie")
- **FTSE 250** — Next 250 largest companies
- **FTSE All-Share** — Combined FTSE 100, 250, and smaller companies

**Examples of LSE-listed companies:**
- BP (ticker: BP.)
- HSBC (ticker: HSBA)
- Unilever (ticker: ULVR)
- AstraZeneca (ticker: AZN)

> 🏛️ **Fun fact:** The LSE's building on Paternoster Square is one of London's most iconic financial landmarks — but most trading happens electronically.

### Europe — Multiple Markets, One Currency Zone

| Exchange | Location | Notable Companies |
|----------|----------|-------------------|
| **Euronext Paris** | Paris | LVMH, Carrefour, Orange |
| **Euronext Amsterdam** | Amsterdam | ASML, Philips, Shell |
| **Euronext Brussels** | Brussels | Anheuser-Busch, Umicore |
| **Frankfurt Stock Exchange** (Xetra) | Frankfurt | SAP, Deutsche Telekom, Siemens |
| **Borsa Italiana** | Milan | Eni, Intesa Sanpaolo, Ferrari |

**Euronext** is notable — it's a merged exchange spanning Paris, Amsterdam, Brussels, and Lisbon. Companies listed on one can trade on all.

**Examples:**
- **ASML** (ASML.AS) — Dutch chip-making giant, one of Europe's most valuable companies
- **SAP** (SAP.DE) — German software company, Europe's largest tech firm
- **LVMH** (MC.FP) — Louis Vuitton owner, France's biggest company

### Asia — Rapid Growth

| Exchange | Location | Notable Companies |
|----------|----------|-------------------|
| **Tokyo Stock Exchange** (TSE) | Japan | Toyota, Sony, SoftBank |
| **Hong Kong Stock Exchange** (HKEX) | Hong Kong | Tencent, Alibaba, HSBC |
| **Singapore Exchange** (SGX) | Singapore | Singapore Airlines, DBS |
| **National Stock Exchange of India** (NSE) | India | Reliance, TCS, HDFC Bank |
| **BSE** (Bombay Stock Exchange) | India | Oldest Asian exchange, founded 1875 |

> 📈 **Growth story:** Asian markets now account for over 30% of global market cap, up from under 10% in 2000.

### Key Ticker Examples

| Company | Exchange | Ticker |
|---------|----------|--------|
| Apple | NASDAQ | AAPL |
| Microsoft | NASDAQ | MSFT |
| BP | LSE | BP. |
| Shell | Euronext Amsterdam | SHEL |
| Unilever | LSE | ULVR |
| SAP | Xetra (Frankfurt) | SAP.DE |
| Toyota | TSE | 7203.T |
| Tencent | HKEX | 0700.HK |

---

## 🏗️ How Exchanges Work

### 1. Order Matching

```
BUY ORDERS                    SELL ORDERS
(People wanting to buy)       (People wanting to sell)

Price    Shares               Price    Shares
-----    ------               -----    ------
£15.10   500                 £15.05   300      ← Match! Trade executes at £15.05
£15.05   200                 £15.10   1,000
£15.00   1,000               £15.15   500
```

The exchange matches the highest buy price with the lowest sell price. That becomes the current market price.

### 2. Market Orders vs. Limit Orders

- **Market order:** "Buy at whatever the current price is" — executes immediately
- **Limit order:** "Buy only if price drops to £15.00" — waits for your price

### 3. Continuous vs. Auction Trading

- **Continuous trading:** Orders match instantly throughout the day (NASDAQ, LSE)
- **Auction trading:** Prices set at specific times (NYSE open/close auctions)

---

## 🏷️ Listing — How Companies Join an Exchange

For a company to trade on an exchange, it must be **listed**. This involves:

### Requirements Vary by Exchange

| Exchange | Minimum Market Cap | Minimum Free Float | Other Requirements |
|----------|-------------------|-------------------|-------------------|
| NYSE | $40 million | 10% of shares | Audited financials, corporate governance |
| NASDAQ | $4.5-110 million (tier-dependent) | 10% of shares | Minimum 300-500 shareholders |
| LSE Standard | £700,000 | 25% of shares | 3-year trading record |
| LSE AIM | No minimum | No minimum | Less regulation, more flexible |

### What Companies Get

1. **Access to capital** — Issue new shares to raise money
2. **Liquidity** — Existing shareholders can sell
3. **Prestige** — Listed companies are "publicly traded"
4. **Valuation** — Market sets the company's value daily

### What Companies Give Up

1. **Disclosure** — Must publish financial reports
2. **Governance** — Must follow exchange rules
3. **Costs** — Listing fees, legal costs, ongoing compliance
4. **Control** — Shareholders have a voice

---

## 🔄 Types of Markets

### Main Market vs. Alternative Investment Market (UK)

- **Main Market:** Full listing, strict requirements, big companies
- **AIM (Alternative Investment Market):** Smaller companies, lighter regulation, more risk

### Primary vs. Secondary Markets

- **Primary market:** New shares are issued (IPO, secondary offerings)
- **Secondary market:** Existing shares are traded (this is what "stock exchange" usually means)

---

## 📊 Types of Orders You Can Place

| Order Type | What It Does |
|------------|--------------|
| **Market order** | Buy/sell immediately at current price |
| **Limit order** | Buy/sell only at your specified price or better |
| **Stop-loss order** | Sell automatically if price falls below threshold |
| **Stop-limit order** | Similar to stop-loss, but with a floor price |
| **Fill-or-kill** | Execute immediately or cancel entirely |

---

## 💡 Key Takeaways

1. **Stock exchanges are marketplaces** — electronic networks that match buyers and sellers

2. **Major global exchanges:** NYSE, NASDAQ (US), LSE (UK), Euronext (Europe), TSE/HKEX (Asia)

3. **Exchanges provide liquidity** — you can convert shares to cash quickly

4. **Listing requires meeting standards** — financial records, governance, minimum size

5. **FTSE 100** contains the UK's 100 largest companies; **S&P 500** tracks America's 500 largest

6. **Ticker symbols vary by exchange:** AAPL (US), BP. (LSE), SHEL (Euronext)

---

## 🧪 Quick Check (Answer in your head)

1. What's the difference between NYSE and NASDAQ?  
   *(Answer: NYSE is older, historically floor-based, tends to list larger companies; NASDAQ is all-electronic with a tech focus)*

2. What does "FTSE 100" represent?  
   *(Answer: The 100 largest companies listed on the London Stock Exchange)*

3. Why do companies become "listed"?  
   *(Answer: To raise capital from investors and provide liquidity for existing shareholders)*

4. What happens when you place a market order?  
   *(Answer: It executes immediately at the current market price)*

---

## 📚 Next Up

**Module 17: Clearing & Settlement** — What happens after you click "buy" to actually own the shares.

---

## 🤔 Questions?

Ask away! Common questions:
- "What's the difference between listing and trading?"
- "Why do some companies choose LSE over NYSE?"
- "What is an IPO and how does it work?"

**When you're ready, reply: "Done with Module 16" or ask your questions!**