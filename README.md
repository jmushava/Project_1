# FinTech Project 1
## Performance Analysis & Recommendation

*First Notebook*
## Part 1- Performance Analysis
### Analyzing how the pandemic has had an impact on the airline industry vs the overall market. 

* Why was the airline industry so badly affected by the pandemic? 
  * Economic uncertainty:
    * GDP was down by 18% in April of 2020 from its previous year, by the second quarter it was down by 31.4%
    * The US economy lost 20.5 million jobs, causing the April unemployment rate to rise to 14.7%.
  * Fear of contagion:
    * 95,000 passengers were screened at the country's airports on April 16, 2020. This represents a 96% decline from 2.6 million on the same day       the year before.
  * Airline operating costs:
    * U.S. carriers’ 2020 net losses topped $35 billion as the pandemic forced carriers to quickly shrink, cut routes and park hundreds of jets. The planes that did fly were not at 100% capacity which contributed to the net losses
    * Even though airlines furloughed and/or laid off workers, total costs were still higher than revenues and airlines continued to burn through cash.
  * Travel restrictions:
    * Suspended entry, quarantine requirements and/or vaccine requirements for travel to and from certain countries including but not limited to Canada, China, United Kingdom, Iran, India, Brazil and the 26 countries included in the Schengen Area
  * Investor sentiments:
    * People were afraid to travel, people had no money to spend and demand for travel plummeted. This triggered a selloff of airline stocks which slashed the valuation of these carriers as seen below:
        * American Airlines’ share price lost 45%
        *	Delta Air Lines’ stock lost 31%,
        *	United Airlines fell 51% over the last 12 months, its biggest drop since 2008. 
        * Southwest shed 14%. 
  * US Stringency index:
    * This is a composite measure based on nine response indicators including school closures, workplace closures, and travel bans, rescaled to a value from 0 to 100 (100 = strictest). As the level of stringency decreased, the airline industry performed better.

## Analysis
* Stocks (ETFs) to analyze 
  * JETS (industry)
  * XLI (sector)
  * SPY (overall)
* Time period 3/1/20-3/1/21 (Different cycles of covid: pre-covid, covid, second wave, vaccine, post vaccine):
  * **Jan-March 2020- pre-covid**: WHO Announces Mysterious Coronavirus-Related Pneumonia in China then CDC Says COVID-19 Is Heading Toward Pandemic Status 
  * **March- April 2020- covid**: The world shuts down; borders close, sports teams cancel seasons, schools close and employees go home
  * **June- November 2020- second wave**: As states begin to reopen, cases begin to skyrocket again so states reverse reopening plans. Unemployment rises, mental health crisis escalates but vaccine research looks promising
  * **December 2020- vaccine**: The FDA authorizes two vaccines; Pfizer and Moderna
  * **Jan- March 2021- post-vaccine**: People are getting vaccinated; the number of new cases and deaths starts to decrease but new variants begin to emerge. CDC advises that the vaccines are effective against new variants, things start to reopen, and people return to a form of normalcy with a newfound hope
  
## Quantitative analysis

* Calculate returns and combine them in a data frame then plot the performance analysis charts 

## Risk analysis
* Calculate the std deviation
* Calculate and plot beta
* Calculate the correlation
* Calculate sharpe ratio

## Data visualization:
* Cumulative returns performance analysis
* Correlation mix
* Rolling std plot
* Rolling beta plot
* Sharpe ratio bar plot

## Analyze data
* **Standard Deviation**- Standard deviation is a measure of how far data points deviate from the mean. Volatile stocks have a higher standard deviation which indicates a stock has a higher risk. Looking at the standard deviation calculation plot, JETS has a higher standard deviation than SPY and XLI which, as shown below, results in it being more volatile.
* **Volatility**- Using the density plot, we can measure the volatility of the stock. The less volatile the stock, the smaller the standard deviation value. A smaller standard deviation means that the stock is less likely to have large (positive or negative) changes in value. Looking at the combined returns plot, we can see that JETS (industry) is the most volatile with SPY (overall market) being the least volatile making JETS a riskier stock than SPY. 
* **Correlation**- Correlation is the positive or negative relationship between two variables. From the correlation matrix, we can see that all three stocks have a positive correlation with each other and that makes sense because the overall market performance affects individual sectors, which in turn affects individual industries. However, since these stocks are not perfectly correlated, correlation does not imply causation. 
* **Beta**- Beta is a measure of the volatility—or systematic rick—of a security or portfolio compared to the overall market. Systematic risk is the risk that cannot be diversified away. Looking at the combined beta plot to compare XLI and JETS to SPY, we can see that JETS has a higher beta, and it is clearly more volatile than XLI. If we want a diversified portfolio, we would need to add stocks that have less correlation and less volatility with the overall market. 
* **Sharpe Ratio**- The Sharpe ratio shows the risk-return relationship and how much return to expect per unit of risk. SPY gives a higher return for every unit of risk assumed by the investor while JETS gives a negative return for every unit of risk assumed. This shows that investing in JETS alone would be detrimental to an investor’s portfolio. 
* **Combined Returns vs Covid Timeline**- As expected, when Covid hit the United States, all three stocks plummeted. As the combined returns plot shows, returns turned negative mid-March and remained on a downward trend until June. This coincides with our Covid timeline because this is the time when states started to reopen, and people were starting to travel again. The stocks started an upward trend as both the country and the world were trying to return to some form of normalcy. Around July, we see the stocks take another dip and by looking at our Covid timeline, this makes sense because the US started to experience a second wave. However, returns didn’t stay down for long, the increase in travel helped boost stock market performance even though returns were nowhere near pre-Covid returns. Around December we see a much bigger jump which coincides with news of the vaccines. Finally, by March 2021 we see that stocks have surpassed pre-Covid returns, with SPY having the highest returns.

## Summary

* Is the industry performance a reflection of the entire sector?
  * Overall, the industry underperformed both the sector and the overall market and the above financial analysis shows that the industry was not able to compensate the investor for the risk and volatility they would assume if they only invested in the airlines industry.


*Second Notebook*

## Part 2- Recommendation
#### A potential investor has approached you looking for a portfolio recommendation. He's been looking at the overall market performance and wants to know if his profile is better suited for a diversified portfolio across industries and sectors or is he better off focusing on one industry. Based on his interests, the industry he had in mind is the Airline Industry. What is your recommendation?

* Investor profile
  * Risk tolerance- low
  * Age- 55
  * Time horizon- 10 years
  * Asset type- stocks
  * Investment amount- $100,000
* Run a MCS to compare different outcomes using a variety of weights (JETS, XLI, SPY)
  *	1/3, 1/3, 1/3
  *	0.9, 0.1, 0.1
  *	0.1, 0.1, 0.9

### Based on the results, give the potential investor your recommendation 
After looking at all three simulations, the portfolio breakdown with the highest upside potential is the portfolio with a majority of JETS stock. However, I would not recommend this portfolio to the investor because it does not align with the investor’s profile. The investor has a low risk tolerance, and the JETS portfolio is both the riskiest and the most volatile portfolio out of all three. Also, based on the time horizon and age of the investor, it would not be prudent to make such a risky investment because assuming the worst-case scenario where the portfolio crashes, there is a limited time period to recoup losses. If the investor was younger with a higher risk tolerance, I would recommend the JETS portfolio but, in this case, I would recommend the evenly distributed portfolio. The upside potential is less than the JETS portfolio, but it has the least risk and the least volatility which aligns with the investor’s profile. 

Lastly, based on the simulations, it is also important to note how diversification plays a big role in investing. By investing across asset classes, markets, industries and sectors, an investor can hedge against market volatility as well as reduce the risk of the overall portfolio. While some investors may prefer to stick to one industry or asset class because it offers short term high returns, in the long term, a diversified portfolio will offer higher returns and peace of mind. Always remember that slow and steady wins the race! 




## Sources

1. COVID-19 and the aviation industry: Impact and policy responses
  * https://www.oecd.org/coronavirus/policy-responses/covid-19-and-the-aviation-industry-impact-and-policy-responses-26d521c1/
2. SPY Data 
  * https://finance.yahoo.com/quote/SPY?p=SPY&.tsrc=fin-srch
3. XLI Data
  * https://finance.yahoo.com/quote/XLI?p=XLI&.tsrc=fin-srch
4. JETS Data
  * https://finance.yahoo.com/quote/JETS?p=JETS&.tsrc=fin-srch
5. Covid Timeline
  *	https://www.yalemedicine.org/news/covid-timeline
  * https://www.ajmc.com/view/a-timeline-of-covid19-developments-in-2020
  * https://www.cdc.gov/museum/timeline/covid19.html
6. Impact of the COVID-19 pandemic on the US Economy and Financial Markets
  * https://www.ncbi.nlm.nih.gov/pmc/articles/PMC8454271/
  * https://www.forbes.com/sites/mikepatton/2020/10/12/the-impact-of-covid-19-on-us-economy-and-financial-markets/?sh=43548c5a2d20 
7. Travel restrictions
  *	https://travel.state.gov/content/travel/en/us-visas/visa-information-resources/covid-19-travel-restrictions-and-exceptions.html
8. How US air travel has been affected by global crises
  * https://www.oliverwyman.com/our-expertise/insights/2021/mar/airline-economic-analysis-2020-2021.html
  *	https://www.sciencedirect.com/science/article/pii/S2590198220301883
  *	https://www.cnbc.com/2021/01/01/us-airline-2-losses-expected-to-top-35-billion-in-dismal-2020-from-pandemic.html
  * https://www.theguardian.com/world/2020/sep/29/inside-the-airline-industry-meltdown-coronavirus-pandemic
9. Financial definitions
  *	https://www.investopedia.com 



