# Odds Modelling and Testing Inefficiency of Sports Bookmakers

## Summary during Conducting the Project

*Apr-2008 to Apr-2010*
**Odds Modelling and Testing Inefficiency of Sports-Bookmakers**

- Learn RExcel, CrystalBall, ModelRisk etc. and choose R open source software to start my research.
- Collect the livescore and also 1x2, Asian Handicap, Over Under odds price data of 29 sportsbookmakers manually from 500WAN, BET007 and NowGoal website and filter the odds price data from 2006 to 2011.
- Apply Poisson model in R to test the return of the investment. This research job is the most completed, success and the first research which write the whole odds compilation EM model and data management by refer to thousands of research papers in sportsbook odds modelling after resigned from Caspo Inc.

  You are feel free to browse over source code via [`Rmodel`](https://github.com/englianhu/Rmodel) package.

```
if(!require('devtools') install.packages('devtools'))
devtools::install_github('englianhu/Rmodel')
```

## 1. Abstract

  In this paper I am applied a diagonal inflated biviriate poisson as well as a simple staking model whereby evaluate the efficiency of odds price of Asian Handicap and Goal Line offered by 40 sports bookmakers. Finally I get a breakdown profit & lose table. While I used **Kelly model**^[Refer to [Testing Inefficiency of Sports-Bookmakers by Kelly Model](https://github.com/Scibrokes/Kelly-Criterion)] next to this research which generated profit (positive return of investment) more than 30% every year.

## 2. Full Version Thesis

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

## 3. Odds Modelling Version II

  In my previous [Betting-Strategy-and-Model-Validation](https://github.com/scibrokes/betting-strategy-and-model-validation), I enhanced my *Rmodel* and test the return of investment. Here I collect the odds price trends of bookmakers and directly fit into calculation as refer to *Niko (2006)*.

### 3.1 Mixed Model

  ...

### 3.2 Betting Strategy

  ...


### 3.3 Reference

  1. [**Creating a Profitable Betting Strategy for Football by Using Statistical Modelling**](https://github.com/scibrokes/betting-strategy-and-model-validation/blob/master/references/Creating%20a%20Profitable%20Betting%20Strategy%20for%20Football%20by%20Using%20Statistical%20Modelling.pdf) *by* [*Niko Marttinen*](https://www.linkedin.com/in/niko-marttinen-7ab18539) *(2006)*
