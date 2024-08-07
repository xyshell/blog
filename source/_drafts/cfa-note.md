---
title: cfa-note
tags: cfa
mathjax: true
---

# CFA Level 3

## Chapter: Capital Market Expectations (5-10%)

### Trend Rate of Growth

$$
\%\text{Growth}= \%\text{labor input} + \%\text{capital per worker} + \%\text{total factor productivity}
$$

where:
- Labor input: labor force (population, demographics) + labor participation (real wages, work/leisure decision, social factors)
- capital per worker: increases labor productivity
- total factor productivity: technological progress + changes in government policies

### Business Cycle Phases

The business cycle can be subdivided into five phases: 

#### 1. Initial Recovery

- Duration of a few months.
- Business confidence rising.
- Government stimulus provided by low interest rates and/or budget deficits.
- Decelerating inflation.
- Large output gap.
- Low or falling short-term interest rates.
- Bond yields bottoming out.
- Rising stock prices.
- Cyclical, riskier assets such as small-cap stocks and high yield bonds doing well.

#### 2. Early Expansion

- Duration of a year to several years.
- Increasing growth with low inflation.
- Increasing confidence.
- Rising short-term interest rates.
- Output gap is narrowing.
- Stable or rising bond yields.
- Rising stock prices.
  
#### 3. Late Expansion

- High confidence and employment.
- Output gap eliminated and economy at risk of overheating.
- Increasing inflation.
- Central bank limits the growth of the money supply.
- Rising short-term interest rates.
- Rising bond yields.
- Rising/peaking stock prices with increased risk and volatility.

#### 4. Slowdown

- Duration of a few months to a year or longer.
- Declining confidence.
- Inflation still rising.
- Short-term interest rates at a peak.
- Bond yields peaking and possibly falling, resulting in rising bond prices.
- Possible inverting yield curve.
- Falling stock prices.

#### 5. Contraction. 

- Duration of 12 to 18 months.
- Declining confidence and profits.
- Increase in unemployment and bankruptcies.
- Inflation topping out.
- Falling short-term interest rates.
- Falling bond yields, rising prices.
- Stock prices increasing during the latter stages, anticipating the end of the recession.

### Taylor rule

central bank uses taylor rule to make monetary policy decisions, determined by the target interest rate using the neutral rate, expected GDP relative to its long-term trend, and expected inflation relative to its targeted amount. It can be formalized as follows:

$$
n_{target} = r_{neutral} + i_{expected} + \underbrace{[0.5(\text{GDP}_{expected} - \text{GDP}_{trend}) + 0.5(i_{expected} - i_{target})]}_{\text{adjustment}}  
$$

where:
- $n_{target}$ = target nominal short-term interest rate
- $r_{neutral}$ = neutral real short-term interest rate
- $\text{GDP}_{expected}$ = expected GDP growth rate
- $\text{GDP}_{trend}$ = long-term trend in the GDP growth rate
- $i_{expected}$ = expected inflation rate
- $i_{target}$ = target inflation rate

### Macroeconomic linkage

A country's current account and capital account are measures of macroeconomic linkages

$$
\begin{aligned}
\text{net exports} &= \text{net private saving} + \text{government surplus} \\
X - M &= (S - I) + (T - G)
\end{aligned}
$$

where:
- X = exports
- M = imports
- S = private savings
- I = investment spending
- T = tax
- G = government spending

### GK Model

GK Model, i.e. Grinold-Kroner model, states that the expected return of a stock is its dividend yield, plus the inflation rate, plus the real earnings growth rate, minus the change in stock outstanding, plus changes in the P/E ratio:

$$
\begin{aligned}
E(R_e) & \approx \frac{D}{P} + \underbrace{(\%\Delta{E} - \%\Delta{S})}_{\text{growth rate of eps}} + \%\Delta{\frac{P}{E}} \\
    & \approx \underbrace{\frac{D}{P} - \%\Delta{S}}_{\text{income (cash flow) return}} + \underbrace{\%\Delta{E}}_{\text{nominal earnings growth}} + \underbrace{\%\Delta{\frac{P}{E}}}_{\text{repricing return}} \\
    & \approx \underbrace{\frac{D}{P} + g}_{\text{constant growth model}} + i - \%\Delta{S} - \%\Delta{\frac{P}{E}} \\
    & \approx \frac{D}{P} + \underbrace{g + i}_{\text{Nominal GDP Growth}} && \text{(in the long run)}
\end{aligned}
$$

where:
- $E(R_e)$ = expected equity return
- $\frac{D}{P}$ = dividend yield
- $\%\Delta{E}$ = expected percentage change in total earnings
- $\%\Delta{S}$ = expected percentage change in shares outstanding, e.g. share repurchase means negative $\%\Delta{S}$, increasing $E(R_e)$
- $\%\Delta{P/E}$ = expected percentage change in the P/E ratio
- all the inputs should be forward-looking (i.e. forecast)

note:
- a share repurchase is a negative $\%\Delta{S}$ term, thus increasing $E(R_e)$
- a nominal earnings growth rate is used, thus incorporating effects of inflation explicitly
- limitation: assumption of infinite time horizon, ignoring investment horizon
- limitation: a $\%\Delta{E}$ larger than GDP growth is not plausible, because it implies a perpetually expanding economy

Real Estate Variation:

$$
E(R_{re}) = \text{cap rate} + \text{NOI growth rate} - \%\Delta{\text{cap rate}}
$$

### ST Model

ST Model, i.e. Singer-Terhaar model, international CAPM

$$
\begin{aligned}
  R_i &= R_f + \beta_{i, M} (R_M - R_f) && \text{(CAPM)} \\
  RP_i &= \beta_{i, M} \times RP_M && (\because RP = R - R_f) \\
       &= \rho_{i, M} \cdot \sigma_i \cdot \underbrace{(\frac{RP_M}{\sigma_M})}_{\text{Sharpe Ratio}} && (\because \beta_{i, M} = \rho_{i, M} \frac{\sigma_i}{\sigma_M})
\end{aligned}
$$

Step1. Full integrated market

$$
\begin{aligned}
  RP_i^G = \rho_{i, GM} \cdot \sigma_i \cdot (\frac{RP_{GM}}{\sigma_{GM}}) && (\text{+  e.g. liquidity premium})
\end{aligned}
$$

Step2. Full segmented market

$$
\begin{aligned}
  RP_i^S = \sigma_i \cdot (\frac{RP_{i}^S}{\sigma_{i}}) && (\text{+  e.g. liquidity premium})
\end{aligned}
$$

Step3. weighted average risk premium

$$
RP  = \phi \cdot RP^G + (1 - \phi) \cdot RP^S
$$

where:
- $\phi$ = degree of integration with the global markets

Step4. expected return

$$
R = RP + R_f
$$

## Chapter: Asset Allocation (5-10%) 
### MVO 

MVO, i.e. Mean-variance optimization

$$
max(\text{Utility}) = E(R) - 0.005 \times \lambda \times Var 
$$

where:
- $\lambda$ = risk aversion score

note:
- if using decimal, times 0.5 instead of 0.005

limitation:
- GIGO: results sensitive to inputs, e.g. expected return, standard deviation, and correlation
- Concentrated asset class allocations: often results in a highly concentrated subset of asset classes, with zero allocation to others, causing lack of diversification of asset classes
- Skewness and kurtosis: only looks at expected return and variance, while in realty, there is significant skewness and kurtosis in actual returns
- Liquidity constraint: does not automatically incorporate liquidity constraints, often resulting in over-allocation to illiquid assets.

## Chapter: Fixed Income

### LDI types

Four types of liability-driven investing (i.e. LDI) 

- Type I: Known future amount(s) and payout dates(s)
- Type II: Known future amount(s) but uncertain payout dates(s)
- Type III: Uncertain future amount(s) but known payout dates(s)
- Type IV: Uncertain future amount(s) and uncertain payout dates(s)

### Hedge Duration Gap between PVA and PVL

Consider an underfunded pension (i.e. DB plan) fund (i.e. PVA < PVL)

#### 1. using future contract

$$
N_f \text{ for 100\% hedge} = \frac{\overbrace{\text{BPV}_L - \text{BPV}_A}^{\text{BPV Gap} }}{\text{futures BPV}}
$$

where:
- $\text{futures BPV} \approx \frac{\text{BPV}_{\text{CTD}}}{\text{CF}_{\text{CTD}}}$


#### 2. using interest rate swaps

receive-fixed swap has positive (+) duration; pay-fixed swap has negative (-) duration

e.g. receive-fixed swap:

$$
\text{net swap BPV} = \text{fixed-side BPV} - \text{floating-side BPV} \\[0.5em]
\text{NP} = \frac{\text{BPV Gap}}{\text{net swap BPV}}
$$

#### 3. using swaption

- to increase asset duration (i.e. $\text{BPV}_A$, closing duration gap), buy receiver swaption
- to decrease asset duration (i.e. $\text{BPV}_A$, widening duration gap), buy payer swaption

#### 3*. using swaption collar

- buy a receiver swaption at lower strike (i.e. SFR: swap fixed rate)
- sell a payer swaption at higher strike (to reduce the initial premium cost outlay)

note:
- the payoff looks like a short risk reversal, with interest rate as X-axis

### Fixed-income return decomposition

- 1. rolling yield:
  - a. coupon income = annual coupon amount / current bond price
  - b. rolldown return = (projected bond price (BP) assuming not yield curve change - beginning BP) / beginning BP
- 2. expected price change due to change in benchmark yield = $(-MD \times \Delta{Y}) + (1/2 \times C \times \Delta{Y}^2)$
- 3. expected price change due to change in credit spreads = $(-MD \times \Delta{S}) + (1/2 \times C \times \Delta{S}^2)$
- 4. expected currency G/L

### CIRP

covered interest rate parity (i.e. CIRP) states that high interest rate currencies should trade at a forward discount

$$
\text{forward rate}_{D/F} = \text{spot rate}_{D/F} \times \frac{(1 + r_D)^T}{(1+r_F)^T}
$$

where:
- $\text{spot rate}_{D/F}$, $\text{forward rate}_{D/F}$: spot and forward rates denoted in direct quotes

### Hedge Foreign Coupon-Paying Bonds

Consider an Australian investor who wishes to hedge their exposure to a coupon-paying U.S. Treasury bond. Assume current USD/AUD = 0.8

| Position                         | At Initiation                                            | Periodic Semiannual Payments for Next 10 Years | At the End                                                |
|----------------------------------|----------------------------------------------------------|------------------------------------------------|-----------------------------------------------------------|
| **U.S. Treasury Bond**           | Pay out USD 100 million to purchase the U.S. bond        | Receive-fixed USD bond coupon                   | Receive USD 100 million par at maturity of bond           |
| **Fixed-Fixed Cross-Currency Swap** | Receive USD 100 million and pay AUD 125 million in exchange of principal amounts | Pay-fixed USD leg                             | Pay USD 100 million and receive AUD 125 million in exchange of principal amounts |
| **Net Flow**                     | Pay AUD 125 million principal outflow                    | Receive-fixed AUD payment                       | Receive AUD 125 million principal inflow                  |


the fixed-fixed cross-currency swap can be synthesized by:

| Swap                          | Description             | Interest Paid | Interest Received | Principal Exchange at Outset                       | Principal Exchange at End                       |
|-------------------------------|-------------------------|---------------|-------------------|---------------------------------------------------|------------------------------------------------|
| **A**                         | USD interest rate swap  | USD Fixed     | USD Floating      | None                                              | None                                           |
| **B**                         | AUD interest rate swap  | AUD Floating  | AUD Fixed         | None                                              | None                                           |
| **C**                         | Cross-currency basis swap | USD Floating  | AUD Floating      | Receive in USD principal, pay out AUD principal   | Pay out USD principal, receive in AUD principal |

### Unhedged Cross-Currency Carry Trade

the carry trade involves borrowing in a low interest rate currency and depositing in a high interest rate currency, facing risk that high interest rate currency weakens.

total pnl = foreign returns - cost of funds + FX rate (D/F) return

## Chapter: Equity

### HHI

Herfindahl-Hirschman index (i.e. HHI):

$$
\text{HHI} = \sum\limits_{i=1}^n{w_i^2} \\
\text{effective number of stocks} = \frac{1}{\text{HHI}}
$$

where:
- n = the number of stocks in the portfolio
- ${w_i}$ = the weight of stock i

note:
- HHI ranges from 1/n (an equally-weighted portfolio) to 1 (a single stock portfolio)
- mcap-weighted portfolio has number of holdings larger than the number predicted by HHI, due to disproportionate effect of the largest capitalization stocks on the index

### Decomposition of realized active return

realized (i.e. ex post) active return can be decomposed into:

$$
R_A = \sum{(\beta_{pk} - \beta_{bk})} \times F_k + (\alpha + \epsilon)
$$

where:
- $\beta_{pk}$ = the sensitivity of the portfolio to each rewarded factor (k)
- $\beta_{bk}$ = the sensitivity of the benchmark to each rewarded factor
- $F_k$ = the return of each rewarded factor
- ($\alpha + \epsilon$) = the return not explained by exposure to rewarded factors—alpha (α) is the active return attributable to manager skill, and ε is the idiosyncratic return—noise or luck (good or bad) (In practice it is very difficult to distinguish between α and ε)

### Active Share

$$
\text{Active Share} = \frac{1}{2}\sum\limits_{i=1}^n{|w_{p,i} - w_{b,i}|}
$$

where:
- n = total number of securities in the benchmark or the portfolio
- $w_{p,i}$ = weight of security i in the portfolio
- $w_{b,i}$ = weight of security i in the benchmark

### Risk Contribution

The contribution of Asset i to portfolio variance ($CV_i$):

$$
CV_i = \sum\limits_{j=1}^n{w_i w_j C_{ij}} = w_i C_{ip}
$$

where:
- $w_j$ = Asset j's weight in the portfolio
- $C_{ij}$	= the covariance of returns between Asset i and Asset j
- $C_{ip}$	= the covariance of returns between Asset i and the portfolio (= $\sum\limits_{j=1}^n{w_j C_{ij}}$)

note:
- The portfolio variance is the sum of each asset's contribution to portfolio variance plus any unexplained variance

The contribution of Asset i to portfolio active variance ($CAV_i$):

$$
CAV_i = (w_{pi} - w_{bi}) RC_{ip}
$$

where:
- $w_{pi}$ = weight of Asset i in the portfolio
- $w_{bi}$ = weight of Asset i in the benchmark
- $RC_{ip}$	= the covariance between the active returns of Asset i and the active returns of the portfolio, which reflects the covariances between the active returns for Asset i and the active returns for each of the n assets in the portfolio (= $\sum\limits_{j=1}^n{(w_{pj} - w_{bj}) RC_{ij}}$)

note:
- Adding up the CAVs for all the assets in the portfolio will give the variance of the portfolio's active return ($AV_p$).

The contribution of Factor i to portfolio variance:

$$
CV_i = \sum\limits_{j=1}^n{\beta_{i} \beta_{j} C_{ij}} = \beta_i C_{ip}
$$

where:
- $\beta_i$ = sensitivity of portfolio to Factor i (regression coefficient)
- $C_{ij}$	= the covariance of Factor i and Factor j
- $C_{ip}$	= the covariance of Factor i and the portfolio (= $\sum\limits_{j=1}^n{\beta_{j} C_{ij}}$)

note:
- The portfolio variance is the sum of each factor's contribution to portfolio variance.

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


### Expected Compounded Return

$$
R_g = R_a - \sigma^2 / 2
$$

where:
- $R_g$ = geometric compounded returns
- $R_a$ = arithmetic non-compounded returns
- $\sigma$ = portfolio volatility

note:
- increasing leverage will lower expected geometric compounded returns over time, due to multiplication to $\sigma$ is squared, while it's not to $R_a$.

example:
- a portfolio falls 2% and then rises by 2%, yielding a compounded return of 0.98 x 1.02 = 0.9996; vs the x10 leveraged portfolio (i.e. falls 20% and then rises by 20%), yielding 0.8 x 1.2 = 0.96

### Style-based Active Management Strategy


Value-based approaches: attempt to identify securities that are trading below their estimated intrinsic value, including:
- Relative value: Comparing price multiples such as P/E and P/B to peers. An undervalued company has an inexplicably low multiple relative to the industry average.
- Contrarian investing: Purchasing or selling securities against prevailing market sentiment. For instance, buying the securities of depressed cyclical stocks with low or negative earnings.
- High-quality value: Equal emphasis is placed on both intrinsic value and evidence of financial strength, high quality management, and demonstrated profitability (the "Warren Buffet" approach).
- Income investing: Focus is on high dividend yields and positive dividend growth rates.
- Deep-value investing: Focus is on extremely low valuations relative to assets (e.g., low P/B), often due to financial distress.
- Restructuring and distressed debt investing: Investing prior to or during an expected bankruptcy filing. The goal is to release value through restructuring the distressed company or through the company having sufficient assets in liquidation to generate appropriate returns.
- Special situations: Identifies mispricings due to corporate events such as divestitures, spin-offs, or mergers.

Growth-based approaches attempt to identify companies with revenues, earnings, or cash flows that are expected to grow faster than their industry or the overall market. Analysts will be less concerned about high valuation multiples and more concerned about the source and persistence of the growth rates of the company, including:

- Consistent long-term growth.
- Shorter-term earnings momentum.
- GARP (growth at a reasonable price); looking for growth at a reasonable valuation. Often this strategy will use the P/E-to-growth (PEG) ratio, which is calculated as the stock's P/E ratio divided by expected earnings growth in percentage terms.

## Chapter: Derivative and Currency Management

### BPVHR

BPVHR, i.e. Basis Point Value Hedge Ratio

$$
\begin{aligned}
\text{BPVHR} & = \frac{\text{BPV}_{\text{target}} - \text{BPV}_{\text{port}}}{\text{BPV}_{\text{futures}}} \\
& = \frac{\text{BPV}_{\text{target}} - \text{BPV}_{\text{port}}}{\text{BPV}_{\text{CTD}}} \times \text{CF}
\end{aligned}

$$

where:
- $\text{BPV}_{\text{CTD}}$ = $\text{MD}_{\text{CTD}} \times 0.0001 \times [\text{price} / 100 \times \text{contract size}]$
- $\text{BPV}_{\text{futures}} \approx \frac{\text{BPV}_{\text{CTD}}}{\text{CF}_{\text{CTD}}}$
- CF: conversion factor

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

excess spread: spread in excess of the fair spread for suffering credit losses.

$$
\text{Excess Spread} := \text{Spread} - \text{EffSpreadDur} \times \Delta \text{Spread} - \underbrace{\text{POD} \times \text{LGD}}_{\text{credit loss}}
$$

Where:
- EffSpreadDur: Effective Spread Duration
- POD: Probability of Default
- LGD: Loss Given Default
- `Spread` and `POD` should be de-annualized to match holding period, if given as annualized

### CDS Price

$$
\text{CDS Price} := 1 + (\text{Fixed Coupon} - \text{CDS Spread}) \times \text{EffSpreadDur}
$$

## Chapter: Alternative Investment

### Hedge Fund Strategy

six strategy categories:

- 1. Equity related: 
- 2. Event driven
- 3. Relative value
- 4. Opportunistic
- 5. Specialist
- 6. Multi-manager

#### Equity-related
Ranked by overall long exposure to market

#### L/S Equity: 

L/S Equity, i.e. Long/Short Equity. The fund manager longs stocks that they think will rise, and shorts stocks that they believe will fall.

- typically have 40% - 60% net long exposure, benefitting from market's long term upward trend
- more concentrated on particular sector or industry
- aspire to provide returns comparable to long-only fund, but with half of volatility
- may use leverage to achieve worthwhile returns

Example:

- Long extension: net exposure of 100%. e.g. 130/30 fund (gross exposure 160%)

#### EMN:

EMN, i.e. Equity Market Neutral

- near-zero market risk exposure; (immune to overall market movements)
- systematic approach to take long and short positions in diversified stocks
- alpha seeking, low volatility
- leverage is generally applied to achieve acceptable level of return

#### Dedicated Short Selling and Short-Biased

dedicated short-selling: pure shorts overpriced stocks (e.g. poorly managed, in declining market segment, or with deceitful accounting); typically 60% - 120% short (by holding the rest in cash).

short-biased, similar except somewhat offset by a long exposure

- negative corr with market, lower returns, greater volatility, little leverage
- activist short selling: not only shorts, but also presents research that contends overprice

### Investment Opportunity Set

- traditional approach:

![Liquidity-Based-Investment-Opportunity-Set](../photos/cfa-note\Liquidity-Based-Investment-Opportunity-Set.png)

![Economic-Environment-Based-Investment-Opportunity-Set](../photos/cfa-note\Economic-Environment-Based-Investment-Opportunity-Set.png)

- risk factor based approach:

defining asset classes by statistically estimating their sensitivities to risk factors, e.g. economic growth and inflation, interest rates and credit spreads, or currency values, liquidity, capitalization, and value-versus-growth.

advantage:
- Identifying sources of risk that are common across asset classes, mitigating a limitation of the traditional approaches, which may classify investments into different classes even when they face largely the same risk factors, leading a manager to believe the portfolio is more diversified than it actually is.
- by allowing a manager to analyze multiple dimensions of portfolio risk, this approach is useful for developing an integrated risk management framework. In this sense, it can be more useful than the traditional approaches for highlighting the primary drivers of portfolio risk.

disadvantage:
-  risk factor estimates can be sensitive to the period used for analysis
-  The results may also be more difficult to communicate to decision makers and to implement compared to traditional approaches.

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

### Portfolio Reporting

Portfolio reporting enables private clients to understand how their investment portfolio is performing and whether their financial goals are likely to be achieved. It provides a basis for a private wealth manager to review a client's IPS and investment strategy with the client to determine if changes are required to achieve the client's goals.

- Performance summary for the current period.
- Market commentary for the current period to provide context for the portfolio's performance.
- Portfolio asset allocation at the end of the current period, including strategic asset allocation - weights or tactical asset class target ranges.
- Detailed performance of asset classes and individual securities.
- Benchmark report comparing asset class and overall portfolio performance to appropriate benchmarks.
- Historical performance of client's investment portfolio since inception.
- Transaction details for the current period (e.g., contributions, withdrawals, interest, dividends, and capital appreciation).
- Purchase and sale report for the current period.
- Impact of currency exposure and exchange-rate fluctuations.
- Progress toward meeting goal portfolios when using a goals-based investing approach.

### Portfolio Review

A portfolio review enables the private wealth manager to reassess a client's IPS and investment strategy in light of recent performance to determine if changes are required. A portfolio review typically addresses the following areas:

- Appropriateness of client's existing goals and investment parameters and if any changes are  required.
- Rebalancing of portfolio asset allocation to target allocation or ranges.
- Any changes to the wealth manager's ongoing management of the portfolio (e.g., degree of - discretionary authority).
- Any changes or updates in the wealth manager's duties and responsibilities.
- Any changes to IPS and portfolio review frequency.

### Balance Sheet Management of Banks and Insurers

how changes in the market value of assets, liabilities, and leverage levels affect the change in the market value of equity is:

$$
\%\Delta E = \%\Delta A \cdot M - \%\Delta L \cdot (M - 1)
$$

where:
- $\%\Delta E$ = percentage change in the value of equity
- $\%\Delta A$ = percentage change in the value of assets
- $\%\Delta L$ = percentage change in the value of liabilities
- M = leverage multiplier, A / E

The sensitivity of the institution's equity capital to a unit change in the reference yield, y, of the assets (i.e., the modified duration of the equity capital) is:

$$
D_E = D_A \cdot M - D_L \cdot (M - 1) \cdot \frac{\Delta i}{\Delta y}
$$

where:
- $D_E$ = modified duration of the institution's equity capital
- $D_A$ = modified duration of the institution's assets
- $D_L$ = modified duration of the institution's liabilities
- M = leverage multiplier, A / E
- $\frac{\Delta i}{\Delta y}$ = estimated change in yield of liabilities, i, relative to a unit change in yield of assets, y

Expected volatility of the percentage changes in the market value of equity capital:

$$
\sigma_E^2 = M^2 \sigma_A^2 + (M - 1)^2 \sigma_L^2 - 2 M (M - 1) \sigma_A \sigma_L \rho_{AL}
$$

where:
- $\sigma_E$ = standard deviation of percentage change in the market value of equity
- $\sigma_A$ = standard deviation of percentage change in the value of assets
- $\sigma_L$ = standard deviation of percentage change in the value of liabilities
- M = leverage multiplier, A / E
- $\rho_{AL}$ = correlation of percentage value changes in assets and liabilities

### Lifetime Gifts vs Testamentary Bequests

$$
\begin{aligned}
& FV_{\text{gift}} &&= [1 + r_g(1-t_g)]^n(1-T_g) \\
& FV_{\text{bequest}} &&= [1 + r_e(1-t_e)]^n(1-T_e) \\
& RV &&= \frac{FV_{\text{gift}}}{FV_{\text{bequest}}}
\end{aligned}
$$

note:
- RV of tax-free gift, $T_g = 0$

### Life Insurance cost comparison

- Net payment cost index: assumes the individual dies at the end of the horizon and cash value is not considered
- Net surrender cost index: assumes the individual terminates the policy (insurance ceases) at the end of the horizon and the cash value is received

steps:
- 1. use annuity due (BGN mode) to compute FV of the premium
- 2. use ordinary annuity (END mode) to compute FV of the dividend
- 3. $FV_{\text{premium}} - FV_{\text{dividend}}$, further minus cash value if using new surrender cost index
- 4. use annuity due (BGN mode) to compute annuitized cost

## Chapter: Trading, Performance Evaluation

### Implementation Shortfall

IS (i.e. implementation shortfall) measures the total cost of trading, expressed as basis points of the total cost of the paper portfolio. e.g. buy order

$$
\text{IS} = \text{paper return} - \text{actual return}
$$

where:
- $\text{paper return} = \text{total order size} \times (\text{close price} - \text{decision price})$
- $\text{actual return} = \text{filled order size} \times (\text{close price} - \text{execution price}) - \text{commission}$

Decomposition of IS. e.g. buy order

- Execution cost = $\text{filled order size} \times (\text{execution price} - \text{decision price})$
  - Delay cost = $\text{filled order size} \times (\text{arrival price} - \text{decision price})$: 
  - trading cost (i.e. market impact cost) = $\text{filled order size} \times (\text{execution price} - \text{arrival price})$
- Opportunity cost = $\text{unfilled order size} \times (\text{close price} - \text{decision price})$
- Fixed cost = $\text{filled order size} \times \text{commission}$

note:
- for sell order, flip the sign
- execution risk: adverse price movement occurs over the trading horizon (in volatile market)
- market impact cost: trade at more adverse prices to execute a larger transaction (in illiquid market)

### Market-adjusted cost

market-adjusted cost removes the impact of market movements on trade cost.

$$
\text{market-adjusted cost} \text{(bps)} = \text{arrival cost} \text{(bps)} - \beta \times\text{index cost} \text{(bps)}
$$

where:
- arrival cost = $\text{side} \times (\text{execution price} / \text{arrival price} - 1)$
- index cost = $\text{side} \times (\text{index average price} / \text{index arrival price} - 1)$

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

### Arithmetic vs Geometric Attribution

|                  | Period 1 | Period 2 |
|------------------|----------|----------|
| Portfolio Return (R) | 5%       | 5%       |
| Benchmark Return (B) | 3%       | 3%       |

- arithmetic attribution: $R_A = R - B = 5\% - 3\% = 2\%$
- geometric attribution: $R_A = \frac{1 + R}{1 + B} - 1 = \frac{1.05}{1.03} - 1 = 1.94\%$

geometric attribution does compound across periods: $(1 + 1.94\%)^2 - 1 = (1.05/1.03)^2 - 1 = 3.92\%$

### Performance Metrics

#### Sharpe Ratio

calculated as excess return over the risk-free rate (numerator) divided by standard deviation (denominator)

$$
S_A = \frac{\bar{R}_A - \bar{r}_f}{\hat{\sigma}_A}
$$

note:
- denominator does not differentiate between volatility that is upside versus downside. Therefore, there is a penalty for all volatility, even if it is "good" volatility (addressed in Sortino Ratio below).

#### Treynor Ratio

similar to the Sharpe ratio, but the denominator is measured by beta, so only considering systematic risk rather than total risk

$$
T_A = \frac{\bar{R}_A - \bar{r}_f}{\hat{\beta}_A}
$$

note:
- assume efficient markets
- only useful in evaluating portfolios that have systematic risk and do not have unsystematic risk (i.e. well diversified)

#### Information Ratio

measures a portfolio's performance against the benchmark but accounts for differences in risk

$$
IR = \frac{E(r_p) - E(r_B)}{\sigma(r_p - r_B)}
$$

note:
- the denominator is known as the tracking risk, or the variability in the portfolio performance with that of its benchmark

#### Appraisal Ratio

measures the ratio of active return, α, to the volatility of the residual term, $σ_ε$, both derived from a factor-based regression

$$
AR = \frac{α}{σ_ε}
$$

note:
- higher AR indicates generating more active return per unit of active risk (as represented by residual risk $σ_ε$ also referred to as the "standard error of the regression") and is therefore a superior active manager according to this measure.
- $σ_ε$, i.e. the standard error of the regression, is the volatility of the error term in a factor-based regression, representing the component of the volatility of returns not explained by the regression model factors. This component of volatility is generated by the manager taking active bets relative to the factors in the model, hence $σ_ε$ here is playing the role of active risk.
- The AR is analogous to the IR. It looks at active return per unit of active risk. The only difference is that the AR uses a factor-based regression to estimate active return and active risk.


#### Sortino Ratio

only considers the standard deviation of the downside risk, in contrast to the Sharpe ratio, which considers all risk (e.g., both upside and downside). Positive volatility associated with the upside can be considered "good" volatility. As a result, the Sortino ratio can provide a more meaningful view of a portfolio's risk-adjusted performance than the Sharpe ratio.

$$
SR_D = \frac{E(r_p) - r_T}{\sigma_D}
$$

where:
- $r_T$: target rate of return, or minimum acceptable return (MAR)
- $\sigma_D$: target semideviation, measuring the standard deviation of returns below the target return

note:
- determination of MAR is subjective and specific to each investor, causing comparability problems


#### Capture Ratio

Capture Ratio (CR) = UC ratio / DC ratio, a measure of return asymmetry, > 1 = positive asymmetry (convex shape), < 1 = negative asymmetry (concave shape)

$$
\text{Capture Ratio} = \frac{\text{Upside Capture Ratio}}{\text{Downside Capture Ratio}} 
$$

e.g.
- if portfolio return is 5%, and benchmark return is 4%, then upside capture ratio 5% / 4% = 125%, > 100% indicates outperformed
- if portfolio return is -3%, and benchmark return is -4%, then downside capture ratio -3% / -4% = 75% < 100% indicates outperformed
- then the capture ratio is 125% / 75% = 1.67, indicates a positively asymmetrical (convex) return profile

note:
- ideally, the manager would capture as much of the upside as possible and capture as little of the downside as possible to maximize the capture ratio
- when betas are increasing (decreasing), momentum-driven strategies should have higher (lower) UC than value-driven strategies. A low-beta (high-beta) strategy will have lower (higher) UC and DC. Therefore, CRs can be used to confirm the investment strategy.

#### Drawdown

| Month    | Monthly Return | Drawdown | Cumulative Drawdown | Comments                |
|----------|----------------|----------|---------------------|-------------------------|
| 01/2018  | 3.14%          |          | 0.00%               |                         |
| 02/2018  | –2.55%         | –2.55%   | –2.55%              | Drawdown phase begins   |
| 03/2018  | –2.71%         | –2.71%   | –5.26%              |                         |
| 04/2018  | –4.66%         | –4.66%   | –9.92%              |                         |
| 05/2018  | –4.91%         | –4.91%   | –14.83%             |                         |
| 06/2018  | –0.73%         | –0.73%   | –15.56%             | Maximum drawdown        |
| 07/2018  | 2.18%          |          | –13.38%             | Recovery phase begins   |
| 08/2018  | 3.11%          |          | –10.27%             |                         |
| 09/2018  | 2.45%          |          | –7.82%              |                         |
| 10/2018  | 3.65%          |          | –4.17%              |                         |
| 11/2018  | 4.03%          |          | –0.14%              |                         |
| 12/2018  | 4.14%          |          | 0.00%               | Drawdown recovered      |

### Time-to-Cash Table

liquidity classification schedule (time-to-cash table) is used to manage liquidity risk, including:

- 1. amount of time needed to convert assets to cash
- 2. liquidity classification level
- 3. liquidity budget

| Time to Cash | Liquidity Classification | Liquidity Budget (% of portfolio) |
|--------------|--------------------------|----------------------------------|
| < 1 week     | Highly liquid            | At least 5%                      |
| < 1 quarter  | Liquid                   | At least 25%                     |
| < 1 year     | Semi-liquid              | At least 40%                     |
| > 1 year     | Illiquid                 | Up to 40%                        |
