# Module 45: Execution, Order Flow & Broker Setup

**Learning time:** 20-25 minutes  
**Prerequisites:** Modules 36-44 (All prior trading modules)

---

## 🤔 Why Execution Matters

You have a strategy. You've backtested it. You know exactly when to enter and exit.

But if your broker is slow, your orders slip, or you use the wrong order type, you'll lose money anyway.

**Execution is the final link between your plan and the market.**

In this module, we'll cover:
- Order types and when to use them
- Reading order flow
- Broker selection
- Optimizing execution

---

## 📖 Order Types

### Market Orders

**What it is:** Buy or sell immediately at the best available price

```
Pros:  Guaranteed execution
Cons:  No price guarantee, slippage in volatile markets
Use:   When speed matters more than price
```

**Example:**
```
Stock: $100 bid / $101 ask
Market buy → You pay ~$101
Market sell → You receive ~$100
```

### Limit Orders

**What it is:** Buy or sell only at your specified price or better

```
Pros:  Price control, no slippage
Cons:  May not execute
Use:   When price matters more than execution
```

**Example:**
```
Limit buy at $99
→ Executes only if price drops to $99 or lower
→ Won't execute at $100
```

### Stop Orders

**What it is:** Triggers a market order when price reaches your stop level

```
Stop-Loss Stop:
Entry: $100
Stop: $95
→ If price drops to $95, market sell triggers

Stop-Limit:
Entry: $100
Stop: $95, Limit: $93
→ If price drops to $95, limit order to sell at $93+
→ May not execute if no buyers at $93+
```

### Trailing Stops

**What it is:** Stop that follows price as it moves in your favor

```
Buy at $100, trailing stop 10%
Stock rises to $120 → stop moves to $108
Stock drops to $108 → stop triggers
Stock continues to $130 → stop moves to $117
```

---

## 📊 Order Flow Basics

### What is Order Flow?

Order flow = seeing the actual buy and sell orders entering the market.

**The concept:**
- Price moves because of executed trades
- Large orders move price
- Understanding order flow helps anticipate moves

### Level 2 / DOM (Depth of Market)

**What it is:** Shows pending orders at each price level

```
DOM:
$105   500 shares to sell
$104   200 shares to sell
$103   100 shares to sell
─────────────────────────
$102   Current price
$101   300 shares to buy
$100   800 shares to buy
```

**How to read:**
- More buyers than sellers at a level = support
- More sellers than buyers at a level = resistance
- Large orders can "absorb" opposite side

### Volume at Price

**What it is:** How much volume traded at each price

**Why it matters:**
- High volume at a level = strong interest
- Price often reverses from high-volume zones
- Shows "fair value" areas

### Order Flow Indicators

| Indicator | What it shows |
|-----------|---------------|
| Cumulative Delta | Net buying/selling pressure |
| Volume Profile | Volume at each price |
| Order Book Imbalance | Buys vs. sells at levels |
| Delta Divergence | Price makes new high but delta doesn't |

---

## 🏦 Broker Selection

### What to Look For

| Factor | Why it matters |
|--------|----------------|
| Execution quality | Slippage = lost money |
| Commissions | Affects profitability |
| Real-time data | Required for active trading |
| Platform | Must be reliable |
| Regulation | Protects your funds |

### Broker Types

**Full-Service Brokers:**
- Human advice, research
- Higher fees
- Example: Morgan Stanley, Goldman Sachs

**Discount Brokers:**
- Self-directed, low fees
- Good for beginners
- Example: Interactive Investor, Hargreaves Lansdown (UK)

**Active Trading Platforms:**
- Low fees, good execution
- Advanced tools
- Example: Lightspeed, tastyworks, IBKR

### UK Brokers Comparison

| Broker | Fees | Best For |
|--------|------|----------|
| Interactive Investor | £0-£12/trade | Beginners |
| Hargreaves Lansdown | £0-£12/trade | Long-term investors |
| Freetrade | Free | Casual traders |
| IBKR | Low, tiered | Active traders |
| Saxo | Low, tiered | Professionals |

### US Brokers Comparison

| Broker | Fees | Best For |
|--------|------|----------|
| Fidelity | Free | Long-term |
| Schwab | Free | Long-term |
| Robinhood | Free | Beginners |
| Interactive Brokers | Low | Active traders |
| Lightspeed | Per-share | Day traders |

---

## ⚡ Execution Best Practices

### 1. Use Limit Orders

Limit orders give you price control:
- Always use for entries
- Always use for exits in normal markets
- Only use market orders in emergencies

### 2. Time Your Orders

**Best times to trade:**
- First 30 min (high volatility, liquidity)
- Last 30 min (price discovery)

**Worst times:**
- Pre-market / after-hours (low liquidity)
- Around major news (high slippage)

### 3. Avoid Trading Around News

News = high volatility + wide spreads = bad fills.

If you must trade:
- Use limit orders
- Expect slippage
- Give more room

### 4. Split Large Orders

If trading large size:
- Split into smaller chunks
- Use time-weighted execution
- Avoid moving the market against you

### 5. Monitor Your Fills

**Track execution quality:**
```
Good fill: Entry $100, filled at $100.10 (0.1% slippage)
Bad fill:  Entry $100, filled at $104   (4% slippage)
```

If slippage is high:
- Switch brokers
- Use different order type
- Trade different hours

---

## 🎯 Advanced Execution

### Order Routing

**Options:**
- SMART routing (broker finds best)
- Directed routing (specify exchange)

**Best practice:** Let broker handle unless you have reason not to.

### Fill Types

**Good til cancelled (GTC):**
- Stays active until executed or cancelled

**Day orders:**
- Invalid at market close

**Immediate or cancel (IOC):**
- Execute immediately or cancel

**Fill or kill (FOK):**
- Execute entirely now or cancel

### Algo Trading

**What it is:** Using algorithms to execute large orders

**Types:**
- TWAP (time-weighted average price)
- VWAP (volume-weighted average price)
- Implementation shortfall
- Adaptive algorithms

**Why use it:**
- Hide large orders
- Reduce market impact
- Get average price

---

## 🔑 Key Takeaways

1. **Order types:**
   - Market: Fast, no price guarantee
   - Limit: Price control, may not execute
   - Stop: Triggers execution at level
   - Trailing: Follows price movement

2. **Order flow:**
   - Level 2 shows pending orders
   - Volume at price shows interest
   - Delta shows net buying/selling

3. **Broker selection:**
   - Execution quality first
   - Consider fees for your style
   - Regulated = safe

4. **Execution best practices:**
   - Use limit orders
   - Time orders carefully
   - Monitor slippage
   - Avoid news

5. **The goal:** Get the price you expect with minimal slippage

---

## ✅ Quick Check

Test your understanding:

1. **What's the difference between a market order and a limit order?**  
   _Hint: One has price control, one doesn't_

2. **Why should you avoid market orders around news?**  
   _Hint: Slippage and volatility_

3. **What does "trailing stop" do?**  
   _Hint: It follows the price when it moves in your favor_

4. **What's the most important factor in broker selection for active trading?**  
   _Hint: Think about what happens when you press "buy"_

---

## 📚 Further Reading

- Broker reviews: Investopedia, The Motley Fool
- Broker comparison: Comparethebroker.com
- Order flow: www.orderflowtrading.com
- "Electronic Trading" guides from major brokers

---

*🎉 CONGRATULATIONS!*

*You've completed **Module 45** and finished **Phase 6: Active Trading & Strategy**!*

---

*What's Next?*

The course has **50 modules** total. Phases 1-6 (Modules 1-45) are now complete.

**Phase 7: Taxation & Wealth Preservation (Modules 46-50)** will cover:
- Capital Gains Tax (UK/US/Europe)
- Tax-efficient accounts (ISA, SIPP, 401k, IRA)
- Tax loss harvesting
- International investing & tax
- Estate planning

These modules will be added in future runs.

---

*You've completed the major practical trading modules. You now have:*
- Technical analysis skills
- Trading system knowledge
- Risk management discipline
- Psychology awareness
- Macro and sentiment awareness
- Execution knowledge

*Keep learning, keep trading, and good luck!*