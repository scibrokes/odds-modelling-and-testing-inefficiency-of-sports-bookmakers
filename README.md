# 赔率建模与测试低效率的体育博彩庄家（英）

## 科研项目总结

*二零零八年四月 至 二零一零年四月*

**Odds Modelling and Testing Inefficiency of Sports-Bookmakers**

- 学习并使用电子表格的RExcel、CrystalBall、ModelRisk等附属计数/机数软件，然后选择并开始自修R鄀计数/机数编程开源软件和科研项目。
- 手动从伍佰万（500WAN）、博彩零零七（BET007）、进球网（Nowgoal）采撷天下权威的廿九家博彩公司即时比分、欧赔（赢和输/赢平输/胜和负/胜平负）、亚赔、大小数据，采撷从二零零六年到二零一一年的赔率数据，将赔率转化为净占卜值，再通过好几种比率（尚未着手去筹算，当赔率越来越小的时候，误差会越来越大，有空才学习数值论去筹算加权指数）去添加价差/抽佣加以转化为一般上市场上博彩公司所开出的赔率。
- 借鉴**棣逊与克尔斯（一九九六∙英）**，通过泊松计数/机数尤物筹算出概率占卜值后转化为净赔率，再通过价差来评估天下权威的廿九家博彩公司的误差比率与误差值，回测出比博彩庄还精准的计数/机数尤物来挣取利润。也就是所谓的量化对冲基金的基本计数/机数尤物。此科研作品算是挺完善和成功的科学研究，也是我第一个科研作品与文献/论文，从客世博离职回国后开始着手科研，阅读几乎上百至千篇科研论文中千篇一律的论文中筛选出最可行的计数/机数尤物，从简单的数据管理和极大似然估计筹算出赔率。

此外，[`fbRanks`](https://cran.r-project.org/web/packages/fbRanks/index.html)鄀计数|机数编程包与蔽包`RModel`的科研路线相似，回测足球彩券的比分、赔率与占卜精准度[**迪逊与克尔斯（一九九六∙英）** *赢家黄氏江夏堂联富，雷欧（二零一四）著*](https://rpubs.com/englianhu/Dixon-Coles1996)，欲知更多详情可查阅[LastPlanet Soccer Ranking](http://lastplanetranking.blogspot.com/p/frontpage_5.html)，同时.敝包`RModel`不仅包含欧赔（赢和输、胜平负）还包含其它产品，请查阅以下列表：

- 欧赔（赢和输、胜平负）
- 亚赔（包含上半场与全场）
- 大小（包含上半场与全场）
- 正确比分（包含上半场与全场）
- 单双（包含上半场与全场）
- 半全场（包含上半场与全场）

数据管理、概率与赔率计数|机数建模、占卜计数|机数建模与投注等量化对冲相关编程代码函数，欲知更多详情请查阅[`Rmodel`](https://github.com/englianhu/Rmodel)鄀计数|机数编程程序包。它日得参考[`QuantTools`](https://cran.r-project.org/web/packages/QuantTools/index.html)鄀计数|机数编程程序包编写个采撷并储存实时外汇价格的网站与应用，可供科研、回测、占卜的高频量化对冲金融交易。

```r
if(!require('devtools') install.packages('devtools'))
devtools::install_github('englianhu/Rmodel')
```

> ## 1. 采撷实时日内汇价
> 
> - **FXCM每周委托挂单数据**：点击[FXCMTickData](https://github.com/FXCMAPI/FXCMTickData) 获取历史委托挂单汇价（汇价数据默认时间为🇬🇧`GMT+0`）。为了方便科研作业，这儿忽略时差问题，将时间添加个时区但不修改时间差距。
> - **Historical Data Downloader Basic** : 点击[Historical Spreads](https://www.fxcm.com/uk/why-fxcm/execution/historical-spreads)获取历史汇价数据。
> 
> 此外，也可点击[**DataCollection**](https://beta.rstudioconnect.com/content/3153)获取历史汇价数据，回测并筛选最优统计模型，再进行交易。
> 
> <img src='诸子百家考工记/ice_video_20171113-013636.gif' width='240'>

*出处[「猫城」FXCM高频量化对冲实时数据](https://github.com/scibrokes/real-time-fxcm)*

## 一、简介

In this paper I am applied a diagonal inflated biviriate poisson as well as a simple staking model whereby evaluate the efficiency of odds price of Asian Handicap and Goal Line offered by 40 sports bookmakers. Finally I get a breakdown profit & lose table. While I used **Kelly model**^[Refer to [Testing Inefficiency of Sports-Bookmakers by Kelly Model](https://github.com/Scibrokes/Kelly-Criterion)] next to this research which generated profit (positive return of investment) more than 30% every year.

## 二、科研论文全局

### 2.1 Odds Modelling

The research on the soccer odds modelling, result prediction, staking as well as the return of investment is applicable to real life. Kindly refer to [Odds Modelling and Testing Inefficiency of Sports-Bookmakers.pdf](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/Odds%20Modelling%20and%20Testing%20Inefficiency%20of%20Sports-Bookmakers/Odds_Modelling_and_Testing_Inefficiency_of_Sports-Bookmakers.pdf) to view the paper.

<iframe src="https://raw.githubusercontent.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/master/Odds%20Modelling%20and%20Testing%20Inefficiency%20of%20Sports-Bookmakers.pdf" width="700px" height="500px" frameborder="0" scrolling="no"> </iframe>

Kindly refer to [*Odds Modelling and Testing Inefficiency of Sports-Bookmakers*](http://issuu.com/englianhu/docs/odds_modelling_and_testing_ineffici?e=24685247/38057010) to read the embed online read mode pdf version.

- Publised version at [ResearchGate.net](https://www.researchgate.net/publication/303135550_Journal_of_Statistical_Software_Odds_Modelling_and_Testing_Inefficiency_of_Sports_Bookmakers_Rmodel)
- Embed Read mode version at [Issuu.com](http://issuu.com/englianhu/docs/odds_modelling_and_testing_ineffici?e=24685247/38057010)

### 2.2 Betting Strategy

Due to my previous research applied \$1 as long as the edge of EM^[Expectation Maximization] odds is over BK^[Odds price offer by Bookmakers] odds and concludes that the staking methods need to be improved.
  
Here I tried to scrap the odds price from [7M](http://www.7msport.com/) and [NowGoal.com](http://www.nowgoal.com/) website^[You are feel free to read from [WebDriver-DynamicWebpage-Scrapping.](https://github.com/scibrokes/webdriver-dynamicwebpage-scrapping)], and apply Kelly-Criterion Model, from the simulatioin we can know that the EM model is profitable.
  
- [Application of Kelly Criterion model in Sportsbook Investment](https://github.com/scibrokes/kelly-criterion)
  + [Application of Kelly model in English Soccer session 2011/12](http://rpubs.com/englianhu/kelly_eng1112)
  + [Application of Kelly model in English Soccer session 2012/13](http://rpubs.com/englianhu/kelly_eng1213)
- [Betting-Strategy-and-Model-Validation](https://github.com/scibrokes/betting-strategy-and-model-validation)

### 2.3 Reference

1. [**Modelling association football scores** *1982 by M.J Maher*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/Maher1982.pdf)
2. [**Modelling Association Football Scores and Inefficiencies in the Football Betting Market.** *1996 by Mark Dixon and Stuart Coles*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/DixonColes1996.pdf)
3. [**A Birth Process Model for Association Football Matches.** *1997 by Mark Dixon and Michael Robinson*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/DixonRobinson1997.pdf)
4. [**Dynamic Modelling and Prediction of English Football League Matches for Betting.** *2002 by Martin Crowder, Mark Dixon, Anthony Ledford and Mike Robinson*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/DixonLedfordRobinson2001.pdf)
5. [**The value of statistical forecasts in the UK association football betting market.** *2004 by Mark Dixon and Peter Pope*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/DixonPope2004.pdf)
6. [**Statistical Modelling for Soccer Games: The Greek League.** *1998 by Dimitris Karlis and Ioannis Ntzoufras*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/KarlisNtzoufras1998.pdf)
7. [**Bayesian modelling of football outcomes (using Skellam’s Distribution).** *2007 by Dimitris Karlis and Ioannis Ntzoufras*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/KarlisNtzoufras2007.pdf)
8. [**Bivariate Poisson and Diagonal Inflated Bivariate Poisson Regression Models in R.** *2005 by Dimitris Karlis and Ioannis Ntzoufras*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/KarlisNtzoufras2005.pdf)
9. [**John Goddard and Ioannis Asimakopoulos** *2004 by John Goddard and Ioannis Asimakopoulos*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/GoddardAsimakopoulos2004.pdf)
10. [**Statistical Methodology for Profitable Sports Gambling** *2012 by Fabián Enrique Moya*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/Moya2012.pdf)

---

By the way, you are feel free to surf over [Bookdown contest submission: Odds Modelling and Testing Inefficiency of Sports Bookmakers](https://community.rstudio.com/t/bookdown-contest-submission-odds-modelling-and-testing-inefficiency-of-sports-bookmakers/13889) or [pdf version](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/bookdown-contest-submission-odds-modelling-and-testing-inefficiency-of-sports-bookmakers.pdf) to know the description of the paper.

---

## 3. Odds Modelling Version II

In my previous [Betting-Strategy-and-Model-Validation](https://github.com/scibrokes/betting-strategy-and-model-validation), I enhanced my *Rmodel* and test the return of investment. Here I collect the odds price trends of bookmakers and directly fit into calculation as refer to *Niko (2006)*.

*Gianluca Baio & Marta Blangiardo (2010)* introduced a model which is not inferior to the one used by *Karlis & Ntzoufras (2003)*. *Ioannis Ntzoufras (2009)* also using WinBugs for modelling where it (and OpenBugs) are not user friedly.

### 3.1 Mixed Model

...

### 3.2 Betting Strategy

...


### 3.3 Reference

1. [**Creating a Profitable Betting Strategy for Football by Using Statistical Modelling**](https://github.com/scibrokes/betting-strategy-and-model-validation/blob/master/references/Creating%20a%20Profitable%20Betting%20Strategy%20for%20Football%20by%20Using%20Statistical%20Modelling.pdf) *by* [*Niko Marttinen*](https://www.linkedin.com/in/niko-marttinen-7ab18539) *(2006)*
2. [**Bayesian Hierachical Model for the Prediction of Football Results**](https://github.com/scibrokes/betting-strategy-and-model-validation/blob/master/references/Bayesian%20Hierachical%20Model%20for%20the%20Prediction%20of%20Football%20Results.pdf) *by* [*Gianluca Baio & Marta Blangiardo (2010)*](https://www.statslife.org.uk/news/84-significance/authors/1458-gianluca-baio-marta-blangiardo)
3. [**Bayesian Modeling using WinBUGS**](https://github.com/scibrokes/betting-strategy-and-model-validation/blob/master/references/Bayesian%20Modeling%20using%20WinBUGS.pdf) *by* [*Ioannis Ntzoufras (2009)*](http://www2.stat-athens.aueb.gr/~jbn/ntzoufras.html)
4. [**Beating the bookmakers**](https://github.com/scibrokes/betting-strategy-and-model-validation/blob/master/references/Beating%20the%20bookmakers.pdf) *by* *Simon Borøy-Johnsen (2017)*

---

<span style='color:RoyalBlue'>**Powered by - Copyright® Intellectual Property Rights of [<img src="figure/Scibrokes.png" width="14"/> Sςιβrοκεrs Trαdιηg®](http://www.scibrokes.com) 個人の経営企業**</span>
