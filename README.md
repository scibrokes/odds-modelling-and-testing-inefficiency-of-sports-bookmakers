# 赔率计数|机数造物（打造尤物）建模与试探体育彩券商的昏庸、无能、腐败与破绽（英）

## 科研项目总结

*二零零八年四月 至 二零一零年四月*

**Odds Modelling and Testing Inefficiency of Sports-Bookmakers**

- 学习并使用电子表格的RExcel、CrystalBall、ModelRisk等附属计数/机数软件，然后选择并开始自修R鄀计数/机数编程开源软件和科研项目。
- 手动从伍佰万（500WAN）、博彩零零七（BET007）、进球网（Nowgoal）采撷天下权威的廿九家博彩公司即时比分、欧赔（赢和输/赢平输/胜和负/胜平负）、亚赔、大小数据，采撷从二零零六年到二零一一年的赔率数据，将赔率转化为净占卜值，再通过好几种比率（尚未着手去筹算，当赔率越来越小的时候，误差会越来越大，有空才学习数值论去筹算加权指数）去添加价差/抽佣加以转化为一般上市场上博彩公司所开出的赔率。
- 借鉴**棣逊与克尔斯（一九九六∙英）**，通过泊松计数/机数尤物筹算出概率占卜值后转化为净赔率，再通过价差来评估天下权威的廿九家博彩公司的误差比率与误差值，回测出比博彩庄还精准的计数/机数尤物来挣取利润。也就是所谓的量化对冲基金的基本计数/机数尤物。此科研作品算是挺完善和成功的科学研究，也是我第一个科研作品与文献/论文，从客世博离职回国后开始着手科研，阅读几乎上百至千篇科研论文中千篇一律的论文中筛选出最可行的计数/机数尤物，从简单的数据管理和极大似然估计筹算出赔率。

此外，[`fbRanks`](https://cran.r-project.org/web/packages/fbRanks/index.html)鄀计数|机数编程包与蔽包`RModel`的科研路线相似，回测足球彩券的比分、赔率与占卜精准度[**迪逊与克尔斯（一九九六∙英）** *赢家黄氏江夏堂联富，雷欧（二零一四）著*](https://rpubs.com/englianhu/Dixon-Coles1996)，欲知更多详情可查阅[LastPlanet Soccer Ranking](http://lastplanetranking.blogspot.com/p/frontpage_5.html)，同时敝包`RModel`不仅包含欧赔（赢和输、胜平负）还包含其它产品，请查阅以下列表：

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

> ## 一、採撷实时日内汇价
> 
> - **FXCM每周委托挂单数据**：点击[FXCMTickData](https://github.com/FXCMAPI/FXCMTickData) 获取历史委托挂单汇价（汇价数据默认时间为🇬🇧`GMT+0`）。为了方便科研作业，这儿忽略时差问题，将时间添加个时区但不修改时间差距。
> - **Historical Data Downloader Basic** : 点击[Historical Spreads](https://www.fxcm.com/uk/why-fxcm/execution/historical-spreads)获取历史汇价数据。
> 
> 此外，也可点击[**DataCollection**](https://beta.rstudioconnect.com/content/3153)获取历史汇价数据，回测并筛选最优统计模型，再进行交易。
> 
> <img src='诸子百家考工记/ice_video_20171113-013636.gif' width='240'>

*出处[「猫城」FXCM高频量化对冲实时数据](https://github.com/scibrokes/real-time-fxcm)*

## 一、简介

借鉴古代春秋战国史（公元前七七零年至公元前二二一年），游牧民族匈奴骑在马上得天下，姜太公的大数定律学术份子的赔率计数|机数建模与试探体育彩券商的昏庸、无能、腐败与破绽。

愚生此科研论文应用对角零通膨双变量泊松加权时间序列尤物和简单的投注计数|机数造物，评估天下诸侯卌霸主体育彩券商的欧赔、亚赔和大小磐上的失误率、低效率性、低学术造诣、昏庸、无能、腐败与破绽。结论上列出每场赛事上投注的注单明细和汇总盈亏表。接下来的科研论文中使用凯利计数|机数编程尤物，年收益超过三成（并且可以每年获得超过三成回酬），详情请查阅[Testing Inefficiency of Sports-Bookmakers by Kelly Model](https://github.com/Scibrokes/Kelly-Criterion)。

## 二、科研论文全局

### 第二章第一节、赔率建模/造物（打造尤物）

科研足彩计数|机数建模，包括赔率造物、占卜赔率、占卜赛果、投注和回酬率，在现实生活中可行的量化对冲投资计数|机数尤物。，详情请查阅[Odds Modelling and Testing Inefficiency of Sports-Bookmakers.pdf](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/Odds%20Modelling%20and%20Testing%20Inefficiency%20of%20Sports-Bookmakers/Odds_Modelling_and_Testing_Inefficiency_of_Sports-Bookmakers.pdf)。

<iframe src="https://raw.githubusercontent.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/master/Odds%20Modelling%20and%20Testing%20Inefficiency%20of%20Sports-Bookmakers.pdf" width="700px" height="500px" frameborder="0" scrolling="no"> </iframe>

至于为学者设计的在线阅读版电子书，请查阅[*Odds Modelling and Testing Inefficiency of Sports-Bookmakers*](http://issuu.com/englianhu/docs/odds_modelling_and_testing_ineffici?e=24685247/38057010)。

- 发布电子书版，请查阅[研究之门（ResearchGate.net）](https://www.researchgate.net/publication/303135550_Journal_of_Statistical_Software_Odds_Modelling_and_Testing_Inefficiency_of_Sports_Bookmakers_Rmodel)。
- 内嵌在线阅读版电子书，请查阅[Issuu.com](http://issuu.com/englianhu/docs/odds_modelling_and_testing_ineffici?e=24685247/38057010)。

### 第二章第二节、投注模式/投资战略

由于第一篇科研论文使用一元投注于任何拥有赔率优势的磐口`EM`值（极大似然估计 Expectation Maximization）的赔率超过`BK`值（足彩商家的赔率 Odds price offer by Bookmakers），该论文将投注门槛分别在于，当`EM`值高于`BK`值十点、廿点、卅点、卌点、一成、两成、三成、四成等，就投注一元再评估回酬。而科研论文的结论是投注模式或投资战略需要改进。

在此愚生从[7M](http://www.7msport.com)和[NowGoal.com](http://www.nowgoal.com)赔率资讯网上採撷赔率数据，欲知更多详情请查阅[WebDriver-DynamicWebpage-Scrapping.](https://github.com/scibrokes/webdriver-dynamicwebpage-scrapping)并且使用凯利标准计数|机数尤物，从模拟与回测中可以获利超过三成。

- [「猫城」在足彩投注模式|投资战略中，使用凯利标准计数|机数尤物（英）](https://github.com/scibrokes/kelly-criterion)
  + [在英超二零二一/二零二二年赛季中，使用凯利标准计数|机数尤物（英）](http://rpubs.com/englianhu/kelly_eng1112)
  + [在英超二零二二/二零二三年赛季中，使用凯利标准计数|机数尤物（英）](http://rpubs.com/englianhu/kelly_eng1213)
- [「猫城」Betting-Strategy-and-Model-Validation](https://github.com/scibrokes/betting-strategy-and-model-validation)

### 第二章第三节、参考文献

- 一、[**Modelling association football scores** *1982 by M.J Maher*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/Maher1982.pdf)
- 二、[**Modelling Association Football Scores and Inefficiencies in the Football Betting Market.** *1996 by Mark Dixon and Stuart Coles*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/DixonColes1996.pdf)
- 三、[**A Birth Process Model for Association Football Matches.** *1997 by Mark Dixon and Michael Robinson*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/DixonRobinson1997.pdf)
- 四、[**Dynamic Modelling and Prediction of English Football League Matches for Betting.** *2002 by Martin Crowder, Mark Dixon, Anthony Ledford and Mike Robinson*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/DixonLedfordRobinson2001.pdf)
- 五、[**The value of statistical forecasts in the UK association football betting market.** *2004 by Mark Dixon and Peter Pope*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/DixonPope2004.pdf)
- 六、[**Statistical Modelling for Soccer Games: The Greek League.** *1998 by Dimitris Karlis and Ioannis Ntzoufras*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/KarlisNtzoufras1998.pdf)
- 七、[**Bayesian modelling of football outcomes (using Skellam’s Distribution).** *2007 by Dimitris Karlis and Ioannis Ntzoufras*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/KarlisNtzoufras2007.pdf)
- 八、[**Bivariate Poisson and Diagonal Inflated Bivariate Poisson Regression Models in R.** *2005 by Dimitris Karlis and Ioannis Ntzoufras*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/KarlisNtzoufras2005.pdf)
- 九、[**John Goddard and Ioannis Asimakopoulos** *2004 by John Goddard and Ioannis Asimakopoulos*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/GoddardAsimakopoulos2004.pdf)
- 十、[**Statistical Methodology for Profitable Sports Gambling** *2012 by Fabián Enrique Moya*](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/reference/Moya2012.pdf)

---

于此之外，莘莘学子都可查阅[Bookdown contest submission: Odds Modelling and Testing Inefficiency of Sports Bookmakers](https://community.rstudio.com/t/bookdown-contest-submission-odds-modelling-and-testing-inefficiency-of-sports-bookmakers/13889)或[电子书版本](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/master/bookdown-contest-submission-odds-modelling-and-testing-inefficiency-of-sports-bookmakers.pdf)以了解科研论文内容。

---

## 三、赔率计数|机数造物（第二版）

根据愚生旧著[「猫城」Betting-Strategy-and-Model-Validation](https://github.com/scibrokes/betting-strategy-and-model-validation)使用凯利标准计数|机数尤物，回酬率比原本的*Rmodel*使用的最基本根据筹算出来的赔率优势，再以每十点一个单位来投注一元来得高，在此採撷足彩商赔率更变的时间序列数据并参照*逆寇（二零零六年∙英）*加以筹算。

**坚卢卡∙拜酉与马耳他∙布兰贾斗（二零一零年）** 介绍一个不逊色（inferior）于**卡尔里斯与猪肉法拉斯（二零零三年）**、**依酉安尼斯∙猪肉法拉斯（二零零九年）** 的计数|机数编程尤物，一样使用WinBugs（在西施康工作期间，自修并比较过，WinBugs软件比OpenBugs软件好使，当时也自修编汇语言、派森与逆向工程破解LeaguePad比分管理软件和一些加密文件和软件）。also using WinBugs for modelling where it (and OpenBugs) are not user friedly.

它日学习投资风险管理与夏普率，欲知更多详情，请查阅：

- [解密复兴科技 - 基于隐蔽马尔科夫模型的时序分析方法](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/世博量化研究院/图书馆/解密复兴科技%20-%20基于隐蔽马尔科夫模型的时序分析方法.pdf)。
- [解读量化投资 - 西蒙斯用公式打败市场的故事](https://github.com/scibrokes/odds-modelling-and-testing-inefficiency-of-sports-bookmakers/blob/世博量化研究院/图书馆/解读量化投资%20-%20西蒙斯用公式打败市场的故事.pdf)

### 第三章第一节、混合计数|机数尤物

...

### 第三章第二节、投注模式|投资战略

...


### 第三章第三节、参考文献

- 一、[**Creating a Profitable Betting Strategy for Football by Using Statistical Modelling**](https://github.com/scibrokes/betting-strategy-and-model-validation/blob/master/references/Creating%20a%20Profitable%20Betting%20Strategy%20for%20Football%20by%20Using%20Statistical%20Modelling.pdf) *by* [*Niko Marttinen*](https://www.linkedin.com/in/niko-marttinen-7ab18539) *(2006)*
- 二、[**Bayesian Hierachical Model for the Prediction of Football Results**](https://github.com/scibrokes/betting-strategy-and-model-validation/blob/master/references/Bayesian%20Hierachical%20Model%20for%20the%20Prediction%20of%20Football%20Results.pdf) *by* [*Gianluca Baio & Marta Blangiardo (2010)*](https://www.statslife.org.uk/news/84-significance/authors/1458-gianluca-baio-marta-blangiardo)
- 三、[**Bayesian Modeling using WinBUGS**](https://github.com/scibrokes/betting-strategy-and-model-validation/blob/master/references/Bayesian%20Modeling%20using%20WinBUGS.pdf) *by* [*Ioannis Ntzoufras (2009)*](http://www2.stat-athens.aueb.gr/~jbn/ntzoufras.html)
- 四、[**Beating the bookmakers**](https://github.com/scibrokes/betting-strategy-and-model-validation/blob/master/references/Beating%20the%20bookmakers.pdf) *by* *Simon Borøy-Johnsen (2017)*

<br><br>

---

[<img src='诸子百家考工记/世博量化.png' height='14'/> Sςιβrοκεrs Trαdιηg®](http://www.scibrokes.com)<br>
<span style='color:RoyalBlue'>**[<img src='诸子百家考工记/世博量化.png' height='14'/> 世博量化®](http://www.scibrokes.com)企业知识产权®及版权®所有，盗版必究。**</span>
