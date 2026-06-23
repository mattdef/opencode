---
name: scalping-trading
description: 7-step scalping trading process for analyzing markets, identifying setups, and executing trades with high probability. Based on professional scalper methodology covering context analysis, economic news, order blocks, scenarios, entry confirmations, execution, and risk management.
permissions:
  edit: allow
---

# Scalping Trading Process

A complete 7-step methodology for scalping markets with a 70%+ win rate. Follow each step sequentially before every trade.

## Core Philosophy

- **Process over outcome**: Follow the steps regardless of individual trade results
- **No ego**: Be willing to flip bias in minutes if market conditions change
- **Preparation is everything**: 90% of the work happens before clicking buy/sell
- **Proactive, not reactive**: Build scenarios before price arrives at your levels

## The 7-Step Process

### Step 1: La Météo (Market Weather)

Quick context analysis when you first open your charts. Do NOT deep-dive yet.

**1. Market Type**
- **Trending/Expansion**: Market moving violently → be ready to execute fast
- **Range/Accumulation**: Market consolidating → be extra patient, wait for A+ setups only

**2. Liquidity Zones** (Most Important Concept)
- **Equal Highs**: Multiple tops without break → stop losses above = magnet for price
- **Equal Lows**: Multiple bottoms without break → stop losses below = magnet for price
- **Trendlines**: Diagonal stop loss clusters that get swept

Purpose: Avoid traps + identify profit targets

**3. Trend Direction**
- Check 4H timeframe first for overall direction
- Align intraday trades with higher timeframe trend when possible

### Step 2: Economic News Check

**You perform this check automatically using available tools.**

**1. Fetch Economic Calendar**
Use `webfetch` to retrieve today's economic events from one of these sources:
- `https://nfs.faireconomy.media/ff_calendar_thisweek.json` (Forex Factory JSON)
- `https://www.investing.com/economic-calendar/` (backup)

Filter for high-impact events (USD, EUR, GBP, JPY if relevant to your pair).

**2. Identify Relevant Events**
- Check which events impact your traded symbol
- Note exact times of high-impact news
- Consider events within ±30 minutes of current time as critical

**3. Mark on Chart**
Use `tradingview_draw_shape` with `shape: "vertical_line"` to mark high-impact news times on the chart. Use red color for high-impact events.

**4. Apply Trading Rules**
- **5 min before high-impact news**: Do NOT open new positions
- **During high-impact news**: Do NOT trade (spread widens, slippage risk)
- **5 min after high-impact news**: Wait for volatility to settle before entering
- If news is imminent, report the restriction and wait

### Step 3: Identify Key Zones (Order Blocks)

**Top-Down Analysis Order:**
1. 4H → Identify major levels
2. 1H → Refine zones
3. 30M → Get closer context
4. 15M → Working timeframe
5. 5M → Entry zone
6. 1M → Precise entry (optional)

**Analogy**: Like a doctor examining a patient - start global, then zoom in. Don't look at the wound under a microscope before understanding the overall condition.

**Key**: Don't skip timeframes. Each one adds context.

### Step 4: Build Scenarios

Map out 2-3 probable price paths before price arrives.

**Example:**
- Scenario 1: Price sweeps liquidity → returns to support → bounces to target highs
- Scenario 2: Price pushes higher → holds accumulation → sweeps lows → returns to order block

**Critical Rules:**
- Scenarios are NOT predictions - they're preparation
- The goal is to NOT freeze when price hits your level
- **Be proactive**: If market opens and your bias is wrong, flip immediately
- The market owes you nothing - update scenarios as new information arrives

### Step 5: Entry Confirmations

Never enter just because price touches a level. Wait for confirmation.

**Three Confirmation Types:**

1. **CHoCH (Change of Character)**
   - Price retraces into level
   - Previous high/low gets liquidated
   - Shows short-term reversal

2. **Support Zone Hold**
   - Small support/imbalance before your entry level
   - If price holds it → bullish signal
   - If it breaks → sellers in control, skip trade

3. **Bearish/Bullish Candle Close**
   - For volatile markets when speed matters
   - Wait for candle to close in your direction
   - Faster execution but less precise

### Step 6: Execution

Click the button only after Steps 1-5 are complete.

**Pre-execution checklist:**
- [ ] Market context analyzed
- [ ] News checked
- [ ] Key zones identified
- [ ] Scenarios built
- [ ] Confirmation received

**If any step is missing → NO TRADE**

### Step 7: Stop Loss & Take Profit

**Stop Loss Placement:**
- Place above/below your order block level
- NOT too tight (gets stopped out before scenario invalidates)
- NOT too loose (defeats purpose of the level)
- If SL is hit → scenario is invalidated → plan changes

**Take Profit Strategy:**
- Target liquidity zones (equal highs/lows)
- Use partial profits: take some at first target, let rest run
- This smooths returns over time

**Example:**
- Entry: Short on gold at order block
- SL: Above the order block
- TP1: First liquidity pool
- TP2: Second liquidity pool / trendline

## Quick Reference Checklist

```
□ Market type identified (trending vs ranging)
□ Liquidity zones marked (EQH, EQL, trendlines)
□ Higher TF trend checked (4H)
□ News calendar reviewed
□ Order blocks mapped (top-down)
□ 2-3 scenarios built
□ Entry confirmation triggered
□ Stop loss placed at invalidation point
□ Take profit targets identified
```

## Common Mistakes to Avoid

1. **Skipping steps** → Each step builds on the previous
2. **Ego trading** → Market doesn't care about your bias
3. **Trading news** → Wait for dust to settle
4. **Skipping timeframes** → You miss context
5. **No scenarios** → You freeze when price moves
6. **Entering without confirmation** → gambling, not trading
7. **Tight stop losses** → Get stopped before scenario plays out

## When to Use This Skill

- Any scalping session (forex, futures, crypto, indices)
- Any timeframe from 1M to 1H
- Works for both long and short trades
- Applicable to any liquid market

## Success Metrics

- Win rate target: 70%+
- Follow all 7 steps on every trade
- Review journal to identify which steps you skip
