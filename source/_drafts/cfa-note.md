---
title: cfa-note
tags: cfa
---

# CFA Level 3

## Chapter: Equity

### Fundamental Law of Active Management

$$
E(R_A) = IC \cdot \sqrt{BR} \cdot \sigma_{R_A} \cdot T C
$$

where:
- $E(R_A)$ = expected active return of the portfolio
- IC = expected information coefficient of the manager, calculated as the correlation between manager forecasts and realized active returns
- BR = breadth, i.e. the number of truly independent decisions made by the manager each year
- TC = transfer coefficient, a number between 0 and 1 that measures the level to which the manager is constrained—TC will take a value of 1 if the manager has no constraints, and 0 if the manager is fully constrained
- $\sigma_{R_A}$ = the manager's active risk (the volatility of active returns)



## Chapter: Derivative and Currency Management

### FOMC % probability of rate change

FOMC, i.e. The Federal Open Market Committee

$$
\frac{
    \text{effective rate implied by future} - \text{current fed target rate}
}{
    \text{fed fund rate assuming change} - \text{current fed target rate}
}
$$

### Excess Spread

$$
\text{Excess Spread} := \text{Spread} - \text{EffSpreadDur} \times \Delta \text{Spread} - \text{POD} \times \text{LGD} 
$$

Where:
- EffSpreadDur: Effective Spread Duration
- POD: Probability of Default
- LGD: Loss Given Default
- `Spread` and `POD` should be de-annualized

### CDS Price

$$
\text{CDS Price} := 1 + (\text{Fixed Coupon} - \text{CDS Spread}) \times \text{EffSpreadDur}
$$

## Chapter: Alternative Investment

### Hedge Fund Strategy

Ranked by overall long exposure to market

### L/S Equity: 

L/S Equity, i.e. Long/Short Equity. The fund manager longs stocks that they think will rise, and shorts stocks that they believe will fall.

- typically have 40% - 60% net long exposure, benefitting from market's long term upward trend
- more concentrated on particular sector or industry
- aspire to provide returns comparable to long-only fund, but with half of volatility
- may use leverage to achieve worthwhile returns

### EMN:

EMN, i.e. Equity Market Neutral

- near-zero market risk exposure; (immune to overall market movements)
- systematic approach to take long and short positions in diversified stocks
- alpha seeking, low volatility
- leverage is generally applied to achieve acceptable level of return

### Dedicated Short Selling and Short-Biased

dedicated short-selling: pure shorts overpriced stocks (e.g. poorly managed, in declining market segment, or with deceiful accounting); typically 60% - 120% short (by holding the rest in cash).

short-biased, similar except somewhat offset by a long exposure

- negative corr with market, lower returns, greater volatility, little leverage
- activist short selling: not only shorts, but also presents research that contends overprice

## Chapter: Private Wealth Management

### TTLLU-RR

set of consideration for private wealth management 

- T: Time horizon;
- T: Taxes;
- L: Liquidity
- L: Legal issues
- U: Unique Constraints
- R: Returns
- R: Risk
  - ATBR: ability to bear risk
  - WTBR: willingness to bear risk
  
### SAMURAI

criteria for a good benchmark

- S: Specified in advance
- A: Appropriate with style
- M: Measurable
- U: Unambiguous
- R: Reflection of investment opinions
- A: Accountable
- I: investible

## Chapter: Performance Evaluation

### Return Attribution

$$
R_A = \sum\limits_{i=1}^N{\Delta W_i}{R_i}
$$

where:
- $R_i$: return from security i
- $\Delta W_i$: active weight of security i, i.e. diff between portfolio and benchmark weight

#### BHB Method, i.e. Brinson-Hood-Beebower

$$
\begin{aligned}
\text{Portfolio Return}, R = \sum\limits_{i=1}^n{w_i}{R_i} \\
\text{Benchmark Return}, B = \sum\limits_{i=1}^n{W_i}{B_i}
\end{aligned}
$$

where:
- $w_i$: portfolio weight of the ith segment (e.g. style, sector, geography, etc.)
- $R_i$: portfolio return in the ith segment
- $W_i$: benchmark weight of the ith segment
- $B_i$: benchmark return in the ith segment
- n: number of segments

$$
\begin{aligned} 
R_A & = R - B \\ 
    & = \sum\limits_{i=1}^n{w_i}{R_i} - \sum\limits_{i=1}^n{W_i}{B_i} \\
    & = \sum\limits_{i=1}^n(w_i R_i - W_i B_i) \\
    & = \sum\limits_{i=1}^n[\underbrace{(w_i - W_i)\cdot B_i}_{\text{Allocation Effect}} + \underbrace{Wi \cdot (R_i - B_i)}_{\text{Selection Effect}} + \underbrace{(w_i - W_i) \cdot (R_i - B_i)}_{\text{Interaction Effect }}]
\end{aligned} 
$$

#### BF Method, i.e. Brinson-Fachler

to solve BHB Method's issue of misleading allocation effect, due to the sign of the resulting allocation effect does not automatically indicate whether the decision to overweight/underweight a particular segment of the portfolio was correct.

$$
\text{Allocation Effect} = (w_i - W_i)\cdot (B_i - \bm{B})
$$

where:
- B: overall benchmark return

note:
- the additional term: $\sum\limits_{i=1}^n(w_i - W_i) \cdot (-B) = (\sum\limits_{i=1}^n{w_i} - \sum\limits_{i=1}^n{W_i}) \cdot (-B) = (1 - 1) \cdot (-B) = 0$

