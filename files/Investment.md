# Investment Brief Note

*经12-计18  张诗颖  2021011056*



## 1 金融市场 Common Sense

+ **金融机构**：Investment Banking, Commercial Banking, Pension Fund, Mutual Fund, Hedge Fund, **P**rivate **E**quity（股权 / 证券）, **V**enture **C**apital

+ **2008金融危机**：**M**ortgage-**B**acked **S**ecurities, **C**ollateralized **D**ebt **O**bligations, **C**redit **D**efault **S**wap

+ **Asset Classes**：Fixed Income (Money / Capital Market) + Equity + Derivatives

  - **T**reasury bills, **C**ertificates of **D**eposits (**L**ondon **I**nter**B**ank **O**ffered **R**ate), Commercial Paper, Bankers' Acceptances, Eurodollars, Repo and Reverse Repo, Federal Funds, **E**xchange-**T**raded **F**unds (Asset Management + **A**uthorized **P**articipants)
  - (**I**nflation-**P**rotected) **T**reasury Notes and Bonds (par=1000, semi-annual compounding), Federal Agency Debt, International Bonds, Municipal Bonds, Corporate Bonds, **M**ortgage-**B**acked **S**ecurities
  - Equity, Options (Call/Put), Futures

+ **Market**：Primary Market + Secondary Market

  - Private Placement, **I**nitial **P**ublic **O**ffering (underwriters + **S**ecurities and **E**xchange **C**ommission + **C**hina **S**ecurities **R**egulatory **C**ommission / 中国证监会, prospectus + road shows + bookbuilding), **S**easoned **E**quity **O**ffering

  - Limit Order Book: Limit-Buy, Limit-Sell, Stop-Buy, Stop-Loss
    **E**lectronic **C**ommunication **N**etworks, NASDAQ, **N**ew **Y**ork **S**tock **E**xchange (+ Arca), Sarbanes-Oxley Act
    Broker / Dealer - Specialist (market maker)

  - **Margin** $= \frac{Equity}{Value}$, Margin Account, Maintenance Margin, Margin Call
    $$
    \begin{aligned}
    \qquad \quad Assets\quad \qquad &|\qquad Liabilities\  \&\ Equity \\
    -------------&-------------- \\
    Shares \quad  \ \$4,000\ \downarrow \quad &|\quad  \mathbf{Margin\ Loan}  \qquad \$2,000\\
    \mathbf{Margin\ Deposit}\quad \qquad \$0\qquad&| \quad Account\ Equity \quad\ \  \$2,000\ \downarrow \quad
    \end{aligned}
    $$

    $$
    \begin{aligned}
    \qquad \quad Assets\quad \qquad &|\qquad Liabilities\  \&\ Equity \\
    -------------&-------------- \\
    Sale \quad \ \$3,000\quad  &|\quad  Short\ Position \qquad \$3,000\ \uparrow \quad\\
    \mathbf{Margin\ Deposit}\quad\ \$1,500\quad&| \quad Account\ Equity \quad\ \ \ \$1,500\ \downarrow \quad
    \end{aligned}
    $$





## 2 Capital Allocation

It is about speculation, not gamble...

> 1. **Fisher Effect**: $i = r + E(\pi)$，actually: $1 + r = \frac{1 + i}{1 + \pi}$
>
> 2. $Expected\ Return\ E(r)\ =\ \sum_ip_ir_i$ , **or**: $\hat{E(r)}\ =\ \frac{1}{n}\sum_{i=1}^nr_i$
>
>    $Variance\ \sigma^2\ =\ \sum_ip_i[r_i-E(r)]^2$, **or**: $\hat\sigma^2\ =\ \frac{1}{n-1}\sum_{i=1}^n(r_i-\overline{r})$
>    $Estimated\ Skewness\ =\ [\hat{(\frac{r - \overline{r}}{\hat\sigma})}]^3$，正/左偏 = 高估risk，负/右偏 = 低估risk 
>    $Estimated\ Kurtosis\ =\ [\hat{(\frac{r - \overline{r}}{\hat\sigma})}]^4 - 3$，正峰度 = 低估risk
>
> 3. **V**alue **a**t **R**isk：最差的情况损失多少，$VaR(1\%, normal)\ =\ Mean-2.33SD$
>
>    **E**xpected **S**hortfall / CVaR：最差的情况**平均**损失多少
>
>    <img src="https://cdn.jsdelivr.net/gh/Catherine0120/ics_image/image-20230526210206671.png" alt="image-20230526210206671" style="zoom:20%;" />
>
> 4. Normal Distribution: $E(Geometric\ Avergage)\ =\ E(Arithmetic\ Average)\ -\ \frac{1}{2}\sigma^2$

+ **E**ffective **A**nnualized **R**ates of Return, **A**nnual **P**ercentage **R**eturn
  **H**olding **P**eriod **R**eturn (= Capital Gain + Dividend Yield)

+ **Sharp Ratio** $=\ \frac{Risk\ Premium}{SD\ of\ excess\ return}$, where $Risk\ Premium\ =\ E(r)-r_f$

  **Sortino Ratio** $=\ \frac{Risk\ Premium}{LPSD}$, **L**ower **P**artial **S**tandard **D**eviation: count only negative deviations

  **Utility Function** $=\ E(r) - \frac{1}{2}A\sigma^2$, (Mean-Variance Utility), is also denoted as **C**ertainty **E**quivalent **R**ate, ==$r$ and $\sigma$ in decimal==



#### 2.1 Markowitz

##### 1. One Risky + Risk-Free

+ **C**apital **A**llocation **L**ine (Expected Return - SD) + Utility Function => Best Allocation
  $$
  \left\{
  \begin{aligned} 
  \quad E(\mathbf{r_p}) \quad & =\quad  r_f + y[E(r_1)-r_f] \\
  \ \mathbf{\sigma_p} \quad & =\quad  y\sigma_1 \\
  \end{aligned}
  \right.\\
  \rightarrow\ E(\mathbf{r_p}) = \frac{E(r_1)-r_f}{\sigma_1}·\mathbf{\sigma_p} + r_f\qquad (CAL) \\
  $$
  <img src="https://cdn.jsdelivr.net/gh/Catherine0120/ics_image/image-20230526220920382.png" alt="image-20230526220920382" style="zoom:50%;" />
  $$
  Max_{\mathbf{y}}\ U\ =\ E(\mathbf{r_p})\ -\ \frac{1}{2}A\mathbf{\sigma_p}^2 \\
  \rightarrow\qquad \mathbf{y^*}\ =\ \frac{E(r_1)-r_f}{A\sigma_1^2}\qquad (best\ allocation)
  $$

+ **C**apital **M**arket **L**ine: CAL for market index + Risk-Free asset (short-term T-bill / money market fund)



##### 2. Two Risky + Risk-Free

+ **Two Risky Assets**

  Efficient Frontier => Optimal Risky Portfolio => Capital Allocation
  $$
  \left\{
  \begin{aligned} 
  \quad E(\mathbf{r_risky}) \ & =\  w_1E(r_1) + w_2E(r_2) \\
  \ \mathbf{\sigma_risky^2} \ & =\ w_1^2\sigma_1^2 + w_2^2\sigma_2^2 + 2w_1w_2·Cov(r_1, r_2),\\
  & \qquad,\ where\ \ Cov(r_1, r_2)=\rho_{12}\sigma_1\sigma_2 \\
  \end{aligned}
  \right.\\
  (Efficient\ Frontier) \\
  perfect\ hedge:\ \rho_{12} = -1,\ \mathbf{w_1}=\frac{\sigma_2}{\sigma_1+\sigma_2},\ \mathbf{w_2}=\frac{\sigma_1}{\sigma_1+\sigma_2} \rightarrow\ \mathbf{\sigma_risky}=0 \\
  $$
  <img src="https://cdn.jsdelivr.net/gh/Catherine0120/ics_image/image-20230526220803536.png" alt="image-20230526220803536" style="zoom:50%;" />
  $$
  \mathbf{(FOC)}\qquad Max_{\mathbf{w_i}}\ S_{risky}\ =\ \frac{E(r_{risky})-r_f}{\sigma_{risky}}\quad s.t.\ w_1 + w_2 = 1\\
  \begin{aligned}
  solution: w_1\ &=\ \frac{E(R_1)\sigma_2^2-E(R_2)Cov(R_1, R_2)}{E(R_1)\sigma_2^2+E(R_2)\sigma_1^2-[E(R_1) + E(R_2)]Cov(R_1, R_2)} \\
  w_2\ &=\ 1\ -\ w_1 
  \end{aligned} \\
  \rightarrow\ E(\mathbf{r_p}) = \frac{E(r_{risky}^*)-r_f}{\sigma_{risky}^*}·\mathbf{\sigma_p} + r_f\qquad (CAL) \\
  $$
  <img src="https://cdn.jsdelivr.net/gh/Catherine0120/ics_image/image-20230526225022955.png" alt="image-20230526225022955" style="zoom:50%;" />

+ **N Risky Assets: Markowitz Portfolio Optimization** 
  $$
  \left\{
  \begin{aligned} 
  \quad E(\mathbf{r_{risky}}) \ & =\  \sum_{i=1}^nw_iE(r_i) \\
  \ \mathbf{\sigma_{risky}^2} \ & =\ \sum_{i=1}^n\sum_{j=1}^nw_iw_jCov(r_i, r_j)\ \\
  & =\ \mathbf{w}^T\Sigma\mathbf{w},\ \Sigma = Covariance\ Matrix \\
  \end{aligned}
  \right.\\
  \begin{aligned}
  & \mathbf{(FOC)}\qquad min_{\mathbf{w}}\ \sigma_{risky}^2\quad s.t.\ E(r_{risky}) = \sum_{i=1}^Nw_ir_i = R\quad \rightarrow Efficient\ Frontier \\
  & \mathbf{(FOC)}\qquad Max_{\mathbf{w}}\ S_{risky}\ =\ \frac{E(r_{risky})-r_f}{\sigma_{risky}}\quad s.t.\ \sum w_i = 1 \quad \rightarrow\ CAL\\
  \\
  & Another\ Apporach: \\
  \end{aligned} \\
  \begin{align}
  & Define:\quad \mathbf{R},\ \Sigma,\ \mathbf{w},\qquad U = r_p - \frac{1}{2}A\sigma_p ^2 \\
  & Then:\quad R_p = \mathbf{w}^T\mathbf{R},\qquad \mathbf{\sigma_p^2} = \mathbf{w}^T\Sigma\mathbf{w} \\
  & \mathbf{(FOC)}\qquad min_\mathbf{w}\ U\ =\ R_p\ -\ \frac{1}{2}A\sigma_p ^2
  \\
  & \rightarrow\qquad \mathbf{w}\ =\ \frac{1}{A}{\Sigma}^{-1}R \qquad (best\ allocation)
  \end{align}
  $$

+ **Detailed Analysis**

  Define:
  $$
  \begin{aligned}
  Average\ Variance\ \ \overline\sigma&=\ \frac{1}{n}\sum_{i=1}^n\sigma_i^2 \\
  Average\ Covariance\ \ Cov&=\ \frac{1}{n(n-1)}\sum_{j=1,j\ne i}^n\sum_{i=1}^nCov(r_i, r_j)
  \end{aligned}
  $$
  Then, we would have:
  $$
  \sigma_p^2\qquad =\qquad \frac{1}{n} \overline\sigma^2\qquad +\qquad \frac{n-1}{n}\ Cov \\
  \qquad \qquad (firm\ specific\ risk) \quad (systematic\ risk)
  $$
  Risk pooling (long-term investment): increase overall risk, increase Sharpe ratio
  Risk sharing: limit pool size, reduce overall risk, increase Sharpe ratio



#### 2.2 Index Model

##### 1. Single Index Model

+ **Single Factor Model**
  $$
  r_i = E(r_i) + \beta_im + e_i \\
  where\ E(m) = 0,\ E(e_i) = 0\\
  \begin{align}
  & Characteristics:\\
  & 1.\ \sigma_i^2 = \beta_i^2\sigma_m^2 + \sigma^2(e_i) \\
  & 2.\ Cov(r_i, r_j) = Cov(\beta_im + e_i, \beta_jm+e_j) = \beta_i\beta_j\sigma_m^2 \\
  & 3.\ Corr(r_i, r_j) = \frac{\beta_i\beta_j\sigma_m^2}{\sigma_i\sigma_j} = Corr(r_i, r_m) \cross Corr(r_j, r_m) \\
  & 4.\ Cov(r_i, r_m) = \beta_i\sigma_m^2,\quad Corr(r_i, r_m) = \beta_i\frac{\sigma_m}{\sigma_i}
  \end{align}
  $$

+ **Single-Index Model**
  $$
  \begin{aligned}
  E(R_i) \qquad =\qquad &\alpha_i\qquad +\qquad \beta_i\ E(R_M) \\
  (total\ Risk\ Premium) \quad (no&nmarket) \qquad\ \ (market)
  \end{aligned}
  $$
  Regression: $R_i = \alpha_i + \beta_i R_M + e_i$

  **S**ecurity **C**haracteristic **L**ine: $R_i = f(R_M)$
  **Ajusted Beta** $=\ \frac{2}{3}\hat\beta + \frac{1}{3} \cross 1$



##### 2. Treynor Black Process

> an active portfolio (A) comprised of the n analyzed securities
> \+ the market index portfolio / passive portfolio (M), the (n+1)-th assets
> $$
> \left\{
> \begin{aligned}
> \mathbf{E(R_p)}\ =\ &\alpha_p + \beta_p·E(R_M)\\
> =\ &(\sum_{i=1}^{n+1}w_i\alpha_i) + (\sum_{i=1}^{n+1}w_i\beta_i)·E(R_M)\\
> \mathbf{\sigma_p^2}\ =\ &\beta_p^2\sigma_M^2 + \sigma^2(e_p) \\
> =\ &(\sum_{i=1}^{n+1}w_i\beta_i)^2·\sigma_M^2 + \sum_{i=1}^{n+1}(w_i^2\sigma^2(e_i)) \\
> & \qquad \qquad  \rightarrow tracking\ error\ 积极组合的个股风险
> \end{aligned}\\
> \right.
> ,\quad max_{\mathbf{w}}\ S_p = \frac{E(R_p)}{\sigma_P} \\
> $$

+ **TB procedure**

  + initial position of each security in the active portfolio: $w_i^0 = \frac{\alpha_i}{\sigma^2(e_i)}$

  + scale to summation 1: $w_i = \frac{w_i^0}{\sum_{i=1}^nw_i^0}$

  + alpha of the active portfolio: $\alpha_A = \sum_{i=1}^nw_i\alpha_i$

    residual variance of the active portfolio: $\sigma^2(e_A) = \sum_{i=1}^nw_i^2\sigma^2(e_i)$

  + initial position of the active portfolio: $w_A^0 = \frac{\alpha_A/\sigma^2(e_A) }{E(R_M)/\sigma_M^2}$

    beta of the active portfolio: $\beta_A = \sum_{i=1}^nw_i\beta_i$

  + adjust the initial posistion in the active portfolio: $w_A^* = \frac{w_A^0}{1+(1-\beta_A)w_A^0}$

    the optimal risky portfolio: $w_M^* = 1 - w_A^*$, $w_i^* = w_A^*w_i$

  risk premium of the optimal risky portfolio: $E(R_p)=(w_M^*+w_A^*\beta_A)E(R_M)+w_A^*\alpha_A$

  variance of the optimal risky portfolio: $\sigma_P^2=(w_M^*+w_A^*\beta_A)^2\sigma_M^2+[w_A^*\sigma(e_A)]^2$

  Sharp Ratio on the optimal risk portfolio: $S_p^2 = S_M^2 + [\frac{\alpha_A}{\sigma(e_A)}]^2\ (\ ={IR}^2=\sum_{i=1}^n[\frac{\alpha_i}{\sigma(e_i)}]^2\ )$

+ **hedged security return** $=\ R_i - \beta_iR_M\ =\ \alpha_i+e_i$ 

+ **comparison: Index Model vs. Full-Covariance Matrix**

  <img src="https://cdn.jsdelivr.net/gh/Catherine0120/ics_image/image-20230527095713010.png" alt="image-20230527095713010" style="zoom:60%;" />





#### 2.3 CAPM

> Market Portfolio (M^*^): 包括投资者**所有**可交易的证券或资产
> $$
> E(R_M^*) = E(r_M^*) - r_f = \overline{A}\sigma_{M^*}^2
> $$

Correspondingly, we generate the concept **C**apital **M**arket **L**ine

+ **Expected Return - Beta relationship**: $E(R_i) = E(r_i) - r_f = \beta_i(E(r_m)-r_f)=\beta_iE(R_m)$
  $$
  \begin{align}
  & market\ return:\\
  & E(R_M) = \sum_{i=1}^Nw_iE(R_i) \\
  & market\ portfolio\ risk:\\
  & \mathbf{\sigma_M^2} = \mathbf{w}^T\Sigma\mathbf{w} = \sum_{i=1}^N\sum_{j=1}^Nw_iw_jCov(r_i, r_j) \\
  & \quad \ = \sum_{i=1}^Nw_iCov(r_i, \sum_{j=1}^Nw_jr_j) = \sum_{i=1}^Nw_i·Cov(r_i,r_M)\ \rightarrow\ risk\ contribution_i \\
  & \mathbf{(Equilibrium\ Condition):}\ E(R_M) = \overline{A}\sigma_{M}^2 \\
  & \qquad \qquad \qquad \qquad  \rightarrow\ E(R_i) = \overline{A}Cov(R_i, R_M) = \frac{E(R_M)}{\sigma_M^2}Cov(R_i, R_M) \\
  & Define:\qquad \qquad \qquad \beta_i \equiv \frac{Cov(R_i, R_M)}{\sigma_M^2}\\
  & Therefore: \qquad \qquad E(R_i) = \beta_iE(R_M)
  \end{align} \\
  $$

+ **S**ecurity **M**arket **L**ine: $E(r) = f(\beta)$

  <img src="https://cdn.jsdelivr.net/gh/Catherine0120/ics_image/image-20230527101406937.png" alt="image-20230527101406937" style="zoom:50%;" />





#### 2.4 APT and Factor Model

$$
Single\ Factor\ Model:\ R_i = E(R_i)+\beta_iF+e_i \\
Single\ Index\ Model:\ R_i = \alpha_i + \beta_iR_M +e_i \\
\rightarrow\ CAPM:\ E(R_i) = \beta_iE(R_M)\\
\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\\
$$

APT: arbitrage if $\alpha_i \gt 0$

> $$
> portfolio\ P:\ R_i = \alpha_p + \beta_pR_M,\quad e_p\ diversified\ away  \\
> \left\{
> \begin{align}
> w_p = \frac{1}{1 - \beta_p} \\
> w_M = \frac{-\beta_p}{1 - \beta_p}
> \end{align}
> \ \ \rightarrow\ \ \beta_z = w_p\beta_p + w_M \beta_M = 0 \\
> \right.\\
> \rightarrow\ \alpha_z = w_p\alpha_p = \frac{1}{1 - \beta_p}\alpha_p
> $$

$$
Multifactor\ Model: R_{it} = \alpha_{it} + \sum_{j=1}^k\beta_{ij}F_j + \epsilon_{it} \\
\rightarrow\ APT:\ E(R_i) = \sum_{j=1}^k\beta_{ij}E(R_j^F)
$$

Suppose $k=2$, arbitrage pricing portfolio Q (portfolio A: $E(R_A) = \beta_{A1}R_1^F + \beta_{A2}R_2^F$, if $E(R_A) \ne price(A)$, then we can arbitrage by construting Q)

> For \$1 investment, invest:
> 		$\beta_{A1}$ to **factor portfolio 1** (with return $r_1$)
> 		$\beta_{A2}$ to **factor portfolio 2** (with return $r_2$)
> 		$1 - \beta_{A1} - \beta_{A1}$ to risk free asset (with return $r_f$)

$$
\begin{aligned}
Portfolio\ Q:\ E(r_Q)& = \beta_{A1}E(r_1) + \beta_{A2}E(r_2) + (1-\beta_{A1}-\beta_{A2}r_f) \\
&= r_f + \beta_{A1}[E(r_1)-r_f] + \beta_{A2}E[(r_2)-r_f]
\end{aligned}
$$

+ **Fama-French Three-Factor Model**
  $$
  R_{it} = \alpha_i + \beta_{iM}R_{Mt} + \beta_{iSMB}SMB_t + \beta_{iHML}HML_t + e_t \\
  where\quad SMB\ \rightarrow\ firm\ size,\quad HML\ \rightarrow \ book\_to\_market
  $$
  



## 3 Frontier Topics

#### 3.1 EMH

**C**ummulative **A**bnormal **R**eturn

+ **Weak Form**: market trading data, technical analysis
  Momentum: positive serial correlation and negative long-term serial correlation
+ **Semi-Strong Form**: all publicly available information, fundamental analysis
  Dividend Ratio (D/P): mostly 1% ~ 10%, (+)
  Earning Yield (E/P): P/E mostly 12 ~ 25
  Bond Spread（高低信用评级债的利差）: (+) with market risk premium
  Fama-French Three Factor Model
+ **Strong Form**: including private details, insider trading



#### 3.2 Behavioral Finance

+ **Cognitive Bias / Heuristics** 认知偏差 / 启发式认知
  Availability bias 可得性偏差：错误的概率预期（忽略样本偏差、先验为主）
  Representativeness 代表性偏差：强加因果/关联，回归效应
  Overconfidence 过度自信：交易frequency越高，平均回报越低
  Conservatism 保守主义：slow react to new information
+ **Behavioral Bias / Framing** 行为偏差 / 框架效应
  Convex utility function
  Prospect Theory (Loss Aversion)
  Frame effect (refrence point matters, regret avoidance, mental accounting )
+ **Limit to Arbitrage** 有限套利
  noise-trader risk, implementation cost, model risk, sentiment index





## Other Brief Notes

1. Bond pricing: Invoice Price = Flat Price + Accrued Interest (in % of par)

2. Callable Bond: (an example)
   Face value (par value): $1,000
   Coupon rate: 6%
   Coupon payment frequency: semi-annual
   Maturity: 10 years
   Call date: After 5 years
   Call price: 105% of face value

3. Determinants of bond saftey
   Coverage ratios: earnings to fixed cost
   Leverage ratios: debt-to-equity
   Liquidity ratios: current asset to current liability
   Profitability ratios
   Cash flow-to-debt ratio

4. Default Bond: recovery rate, default yield spread

5. Interest Rate Uncertainty and Forward Rates
   Forward Rate: future short rates implied from current yield curve
   Expectation Hypothesis: $f_2 = E(r_2)$ (expected future short rate)
   Liquidity premium: $f_n - E(r_n) > 0$, and shall increase over maturity length

6. Synthetic forward loan

   <img src="https://cdn.jsdelivr.net/gh/Catherine0120/ics_image/image-20230527152001551.png" alt="image-20230527152001551" style="zoom:40%;" />

7. Economic Indicators: leading / coincident / lagging indicators

   <img src="https://cdn.jsdelivr.net/gh/Catherine0120/ics_image/image-20230603140250261.png" alt="image-20230603140250261" style="zoom:50%;" />

   Industry Analysis: cyclical / defensive industries（防御性行业）
   Sensitivity to the Business Cycle: 
           sensitivity to sales (necessities vs discretionary goods)
           operating leverage: the split between fixed and variable costs (higher leverage, more sensitive), **D**egree of **O**perating **L**everage: $DOL=\frac{Percentage\ change\ in\ Profits}{Percentage\ change\ in\ Sales} = 1+\frac{Fixed\ costs}{profits}$
           financial leverage: the use of borrowing (higher interest rate, higher sensitivity)
   财务杠杆的比例和CAPM中的β等比例放缩
   Sector Rotation: 预计好的行业based on business cycle 的 investment strategy
   inflation rate $\uparrow$ $\Rightarrow$ P/E Ratio $\downarrow$ (lowers P and boost nomial E)