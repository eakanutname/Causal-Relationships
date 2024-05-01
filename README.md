# Causal-Relationships

ESG Predictive Power Thailand
Businesses with good ESG (Environmental, Social, and Governance) practices reflect their ability to compete and potential for long-term growth.

Since business is about solving problems, increasing positive impacts, and reducing negative impacts, it is the responsibility of businesses to be concerned with ESG.

The source of funds in the business sector comes from investments in finance. This leads to the question of whether businesses with good ESG performance benefit investors.

We specifically focus on two aspects: returns and investor sentiment, using EV/EBITDA (Enterprise Value to Earnings Before Interest, Taxes, Depreciation, and Amortization) as a proxy for stock premium.

Before starting the research, we hypothesized that ESG would have a positive relationship with return rates, as sustainable growth should be reflected in returns. Additionally, we hypothesized that ESG would have a positive relationship with EV/EBITDA, as companies with good ESG scores should receive a premium valuation due to their impact on consumer choices.

We began by running a simple linear regression, using ESG Factors (data from LSEG, using 2022 data as it was the most complete and closest to the current year, 2024) as the independent variables, and returns and EV/EBITDA as the dependent variables.

Since linear regression assumes no multicollinearity among independent variables, we used the Variance Inflation Factor (VIF) to filter out correlated variables, removing those with a VIF greater than 10, leaving us with 10 independent variables.

Additionally, we ran multiple linear regressions, varying the number of independent variables from 1 to 10, to gain insights into how the model's behavior changes.For the return linear regression, we found two significant variables: Emissions Score and Workforce Score, which remained significant in many cases as we added more variables. These variables had a positive relationship with returns, aligning with our hypothesis. Therefore, focusing on Emission Score and Workforce Score could increase the chances of higher returns.

For the EV/EBITDA linear regression, we found four significant variables: Human Rights Score, Resource Use Score, CSR Strategy Score (which captures the communication of ESG practices), and Emission Score. The first three had a negative relationship, contrary to our hypothesis, while Emission Score had a positive relationship.

Furthermore, when running a single-variable linear regression, the only significant ESG variable for EV/EBITDA was Human Rights Score. The researcher attributes this to the lack of interaction terms in the model, which could explain why some variables became significant when combined but not when isolated.

Number of grandslam final played by Roger Federe is highly correlate to the number of electrical engineer in the mexico.

Motivated by these findings, we went deeper into the cause-effect relationships using the PC algorithm, which tests for conditional independence between variable pairs. The output from this algorithm is represented in the network diagram below:

Interestingly, three of the four significant variables from the linear regressions are present in this network. However, contrary to expectations, returns and EV/EBITDA were removed during the PC Algorithm, suggesting that their relationships with the ESG variables may have been merely correlational.

In the network, Shareholders Score is a cause of CSR Strategy Score, which in turn affects Emissions Score. However, the researcher does not see a clear connection between Resource Use Score being a cause of CSR Strategy Score and Emissions Score, and CSR Strategy Score being a cause of Workforce Score. The researcher hypothesizes that this could be due to the absence of other dominating variables in the network or a lack of understanding of the relationships.

In summary, the researcher approached model building from both predictive (linear regression) and causal (PC algorithm) perspectives, using ESG variables as independent variables and returns and EV/EBITDA as dependent variables.

For returns, although some ESG variables were significant in the linear regression, returns were removed during causal discovery, suggesting that the observed relationships may have been merely correlational.

For EV/EBITDA, the results aligned with the linear regression, as EV/EBITDA was also removed from the network, indicating a potential correlation rather than a causal relationship.The study has limitations, including:

1.The researcher used data only from 2022

2.If investor behavior in 2024 deviates significantly from 2022, the results may change.

3.The researcher included only ESG variables, returns, and EV/EBITDA in the network.

Finally, the researcher concludes that although ESG research is still in its early stages, investments in ESG products are already worth billions of dollars. This study is intended as a prototype for ESG research in Thailand, which is also in its early stages, with the goal of leading to larger-scale, more comprehensive, and timely research that will benefit investors.
