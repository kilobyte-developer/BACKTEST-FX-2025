# 2025 BACKTEST REPORT (EU + GU + XAU)

### Final Strategy Validation — 2025

## 🎯 Objective

To analyze all **A+ setups** from **January–December 2025** across:

- **EURUSD (EU)**
- **GBPUSD (GU)**
- **XAUUSD (Gold)**

and extract:

✅ data-backed SL requirements  
✅ DD (MAE) behavior + noise patterns  
✅ reversal / continuation nature per pair  
✅ best execution filters (sessions + conditions)  
✅ exit rules + trade management logic  
✅ no-trade conditions (where A+ setups fail anyway)

> This report converts raw backtest trades into **2026 execution rules**.

---

## 📌 Dataset Overview

- **Pairs Covered:** EU, GU, XAU
- **Timeframe:** H1 (core), HTF alignment applied (H4/D1 bias)
- **Period Tested:** Jan 2025 → Dec 2025
- **Trade Type:** Only A+ setups (filtered, not random entries)
- **Session Focus:** London / NY / Overlap
- **RR Baseline:** 1:2 model + exit extensions reviewed
- **Total Trades:** _(fill from Excel)_
  - EU trades: \_\_\_
  - GU trades: \_\_\_
  - XAU trades: \_\_\_

---

## 📚 Definitions & Terminology (VERY IMPORTANT)

### ✅ Played

Market respected the level and created a clean directional reaction.

### ✅ Tradable

Entry was realistic and executable:

- no insane spread
- no news spike
- no one-tap candle
- no dead hours / illiquid time
- no stupid chase entry

### ✅ DD after Entry (MAE)

Maximum adverse movement in pips after entry (before TP/SL).

### ✅ SL Needed

Minimum SL required to survive noise when setup later still worked.

### ✅ Reversed After

How many pips price moved in favor before reversal began.

### ✅ Consolidation Zone

A compression phase where multiple A+ setups fail regardless of bias accuracy.

### ✅ Extreme Levels

When two nearby HTF zones exist without invalidation → stronger combined zone.

- Used as: `Ex.T2`, `Ex.QML`

### ✅ Opposite Levels

Old-trend levels still pending/unmitigated that often react strongly.

- Used as: `Opp.T2`

---

# 🌍 Pair Behavior Summary (BIG PICTURE)

## ✅ EURUSD (EU)

- Generally cleaner structure + less manipulation
- Often respects levels well
- Rotation behavior common (not always runner)
- Best in: **London + early NY**

## ✅ GBPUSD (GU)

- More aggressive volatility + deeper wicks
- Needs extra SL tolerance vs EU
- Fake breaks common around liquidity

## ✅ XAUUSD (Gold)

- Highest volatility + manipulation spikes
- SL needs biggest tolerance
- Best reacts during **London + NY overlap**
- Horrible in dead/illiquid hours

---

# 📊 Backtest Insights (What the data proved)

## 1) Session Performance

### ✅ Best Sessions

- London session → highest clean follow-through
- NY session → strongest continuation potential
- Overlap → best for XAU explosions

### ❌ Worst Session / No Trade Window

Avoid trading during:

- **00:00 IST – 05:30 IST** _(illiquid / fake moves / spreads)_
- holidays / thin liquidity
- pre-news build-up spikes

---

## 2) Stop Loss Requirements (SL Model)

### 2.1 SL Tolerance Rule

SL must be based on:

- structure **AND**
- statistical noise tolerance

✅ Most losses were not “wrong bias”
❌ They were “tight SL got clipped”

### 2.2 Pair-Wise SL Behavior

_(fill these from Excel once finalized)_

- **EU:** needs tight-medium tolerance
- **GU:** needs medium-high tolerance
- **XAU:** needs high tolerance (noise + spikes)

✅ Rule:
If structural SL is too small compared to required tolerance → **skip trade**

---

## 3) DD (MAE) Insights — Noise vs Failure

### Typical DD types

- wick sweep then continuation
- body close beyond zone = true failure
- news-driven DD = invalid trade environment

✅ Rule:
Wick hit ≠ invalidation  
Body-close hit beyond tolerance = invalidation

---

## 4) Reversal / Exit Logic

### 4.1 Rotation vs Runner Behavior

- **EU** rotates often
- **GU** can run but with deep pullbacks
- **XAU** can run hard but reverses violently

### 4.2 Exit Zones

✅ price often reacts strongly first and then reverses after a certain move

#### Practical conclusion

- Default RR model should remain **1:2**
- Extensions only when **trend + momentum confirm**

---

## 5) Consolidation / Compression (No-Trade Condition)

Backtest shows:

- In compression, even perfect A+ setups fail
- 4–6 consecutive losses occur without bias failure

✅ Rule:
If multiple A+ setups fail back-to-back in same zone →
**identify as consolidation and STOP trading**

---

# ✅ Final Trading Rules for 2026 (EU + GU + XAU)

## 6.1 Entry Rules

Trade only A+ setups:

- `T2`
- `QML`
- `Extreme Levels`
- `Opposite Levels`

Entry quality rules:

- penetrative taps > wick taps
- wait for confirmation if first tap is sloppy
- don’t enter during news / pre-news spikes

✅ Preferred:
Extreme levels when price is within **5–10 pips** of zone.

---

## 6.2 Stop Loss Rules

- Use structural SL + noise tolerance
- avoid comfort SLs (too tight)
- if SL needed > allowed risk → **no trade**

---

## 6.3 Take Profit & Management

### Default:

✅ **1:2 RR**

### When to extend:

Only if:

- HTF trend aligns
- momentum candle structure supports continuation
- no major opposing HTF zone nearby

---

## 6.4 Re-Entry Rules

If wick-to-wick entry hits SL:

- do NOT revenge trade
- re-enter only after:
  - penetrative tap OR
  - liquidity sweep + confirmation

Treat re-entry as a **new trade**, not emotional continuation.

---

## 6.5 No-Trade Conditions (Hard Rules)

❌ Avoid trades when:

- consolidation/compression zones active
- illiquid hours (00:00 IST – 05:30 IST)
- major news spikes / CPI / FOMC volatility
- spread expanded
- one-tap candle nukes the zone instantly

---

# 🧠 Core Principle

**EU rewards patience and precision.**  
**GU rewards SL tolerance + discipline.**  
**XAU rewards timing + risk control.**

If SL is tight → you’re not “smart”, you’re just donating liquidity 💀

---

### ~~~ END OF REPORT ~~~
