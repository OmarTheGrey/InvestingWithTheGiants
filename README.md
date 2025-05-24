
# 📈Investing with the Giants: A Comprehensive Stock Performance Analysis of Leading Tech Giants (2016-2024)

This serves as a comprehensive data analysis project exploring the stock performance of five leading technology companies: **Apple (AAPL), Amazon (AMZN), Google (GOOGL), Microsoft (MSFT), and Nvidia (NVDA)**.

We will delve into historical stock data to:
*   Visualize their growth trajectories.
*   Analyze their risk and reward profiles.
*   Examine the impact of key market events, suchally the COVID-19 pandemic.
*   Investigate correlations between these tech giants.
*   Attempt to predict future stock price movements.

This project aims to provide insights into market dynamics, investment strategies, and the resilience of tech innovation through data-driven storytelling.

# ✒️ Authors

This project was collaboratively developed by the following individuals for the Data Analysis Course at EUI:

*   **[Omar Shafiy](https://www.linkedin.com/in/theomarshafiy/)** (23-201356)
*   **[Omar Sharaf](https://www.linkedin.com/in/omar-sharaf-545220293?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app)** (24-101236)
*   **[Omar Wafa](https://www.linkedin.com/in/omar-wafa-5b04b9238?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_appE)** (23-101281)
*   **[Eiad Essam](https://www.linkedin.com/in/eiad-essam-50771a254?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app)** (23-101108)

Feel free to reach out with any questions or feedback.
## Abstract

This report presents a comprehensive data analysis of the stock performance of five major technology companies: Apple (AAPL), Amazon (AMZN), Google (GOOGL), Microsoft (MSFT), and Nvidia (NVDA), spanning from early 2016 to late 2024. Leveraging historical daily stock data, this study explores their individual growth trajectories, quantifies their risk-reward profiles, and investigates the profound impact of the COVID-19 pandemic on their financial volatility. Furthermore, it delves into the interconnectedness of these tech giants and presents an attempt to forecast their future stock trajectories using time series models. The findings reveal distinct narratives of growth, resilience, and adaptability within the tech sector, highlighting Nvidia's explosive ascent and Microsoft's consistent stability, while also underscoring the market's dramatic shifts in response to global events.

## 1. Introduction: The Tech Titans' Arena

In an era increasingly shaped by digital innovation, a select group of technology companies stands out as global economic powerhouses. Apple, Amazon, Google, Microsoft, and Nvidia have not only reshaped industries but have also become dominant forces in the financial markets. Understanding their historical stock performance is not merely an academic exercise; it's crucial for investors, market analysts, and anyone seeking to grasp the intricate dynamics of the modern economy.

This project embarks on a data-driven journey to dissect the stock stories of these five tech giants. Our analysis is structured to achieve several key objectives: to vividly illustrate their paths to growth, assess the inherent risks associated with investing in them, meticulously quantify the specific impact of the unprecedented COVID-19 pandemic on their stock behavior, uncover the subtle ways their market movements intertwine, and explore the intriguing, albeit challenging, realm of predicting their future stock trajectories.

## 2. The Landscape of Growth: Price Trajectories

Our initial examination of the raw closing prices across these tech giants immediately highlights the vast differences in their absolute stock values. While companies like Google and Amazon may trade at higher dollar amounts per share, this raw view can be misleading. It offers a snapshot of their current price but tells us little about the actual percentage growth an investor would have experienced relative to their initial investment.

To gain a truly comparable understanding of their performance, we normalized all stock prices to a common starting point (a base of 100) on January 2, 2016. This transformation allowed us to visualize their percentage growth trajectories side-by-side, painting a far clearer picture of who truly led the charge.

![Raw Closing Prices of Tech Giants (2016-2024)](IWTG%20Results/Raw%20Closing%20Prices%20of%20Tech%20Giants%20(2016-2024).png)

From this normalized perspective, Nvidia emerged as the undisputed champion of growth, showcasing an exceptionally explosive upward trend that dramatically outpaced its peers, particularly in the later years of our analysis. Microsoft, while perhaps less flashy, demonstrated remarkably strong and consistent growth throughout the period, solidifying its position as a reliable performer. Apple also delivered substantial percentage gains, though its curve was not as dramatically steep as Nvidia's. Amazon and Google ultimately achieved significant overall growth, but navigated a somewhat more volatile path, marked by noticeable fluctuations.

![Normalized Closing Prices of Tech Giants (Base 100)](IWTG%20Results/Normalized%20Closing%20Prices%20of%20Tech%20Giants%20(Base%20100).png)

## 3. Unpacking Risk: Volatility and Returns

Beyond just growth, a savvy investor deeply considers risk, which is often measured by volatility – the degree of price fluctuation. Our deep dive into the daily returns of these tech giants aimed to illuminate the "ride" accompanying their growth stories. Common wisdom in investing suggests that higher potential returns often come with higher inherent risk.

Our analysis of the distribution of daily returns, complemented by a scatter plot comparing annualized volatility against mean annualized returns, provided crucial insights. Nvidia, while boasting unparalleled returns, also exhibited the highest volatility, confirming its identity as the most thrilling, yet potentially turbulent, investment among the group. Microsoft, however, struck an impressive balance, delivering substantial returns with notably lower volatility compared to its peers. This positions Microsoft as a unique blend of robust growth and relative stability. Apple also demonstrated itself as a comparatively steady performer, offering solid returns with manageable risk. Amazon and Google typically fell into a middle ground, providing decent returns but with more pronounced daily swings than Microsoft and Apple.

![Distribution of Daily Returns for Tech Giants](IWTG%20Results/Distribution%20of%20Daily%20Returns%20for%20Tech%20Giants.png)

![Risk (Volatility) vs. Annualized Return](IWTG%20Results/Risk%20(Volatility)%20vs.%20Annualized%20Return.png)

To further understand the dynamic nature of this risk, we also examined the 30-day rolling annualized volatility. This revealed how volatility itself shifted over time, providing a granular view of fluctuating risk levels across different market phases.

![30-Day Rolling Annualized Volatility for Tech Giants](IWTG%20Results/30-Day%20Rolling%20Annualized%20Volatility%20for%20Tech%20Giants.png)

## 4. Investor's Lens: Hypothetical Investment Returns

To translate abstract growth percentages into a more tangible understanding, we posed a compelling hypothetical: what if an investor had allocated $1000 to each of these tech giants at the start of the post-COVID period (February 19, 2020), holding them until the end of 2024?

The results powerfully underscore the immense wealth generation potential within this sector. Nvidia's performance was nothing short of extraordinary; a hypothetical $1000 investment would have swelled to over $17,000, representing a staggering 1614% return. While Apple, Google, and Microsoft also delivered substantial gains (ranging from 135% to 219%), and Amazon a solid 102%, Nvidia's remarkable trajectory truly set it apart. This simulation vividly demonstrates the profound impact of compounding returns and the outsized financial rewards achievable from investing in leading high-growth companies.

![Final Value of $1000 Invested on 2020-02-19 (Held until 2024-12-31)](IWTG%20Results/Final%20Value%20of%20$1000%20Invested%20on%202020-02-19%20(Held%20until%202024-12-31).png)

## 5. Market Interplay: Volume & Correlations

Understanding trading volume and inter-stock correlations is vital for comprehending the broader market context and portfolio diversification strategies. Trading volume serves as a pulse check on investor interest and market activity. Our analysis revealed a general upward trend in daily trading volume for most tech giants throughout our period, reflecting growing market participation and institutional engagement. Nvidia, in particular, consistently commanded exceptionally high trading volumes during its rapid growth phase, signaling intense investor activity and robust liquidity. Spikes in volume often coincided with major news events or earnings reports, indicating heightened market reactions.

![Daily Trading Volume of Tech Giants (2016-2024)](IWTG%20Results/Daily%20Trading%20Volume%20of%20Tech%20Giants%20(2018-2024).png)

Furthermore, we examined the correlation between the daily returns of these tech titans. As expected for large-cap companies operating within the same sector, all five exhibited a high degree of positive correlation (generally ranging from 0.5 to 0.7 or higher). This strong positive correlation implies that these stocks tend to move in tandem, largely influenced by shared sector-wide trends and macroeconomic forces. From a portfolio diversification perspective, this suggests that holding solely these tech giants, while potentially lucrative, would offer limited protection against downturns that broadly affect the technology sector. Diversification would necessitate looking beyond this specific group of large-cap tech.

![Correlation Matrix of Daily Returns for Tech Giants](IWTG%20Results/Correlation%20Matrix%20of%20Daily%20Returns%20for%20Tech%20Giants.png)

## 6. The Pandemic's Mark: COVID-19 Impact Analysis

The COVID-19 pandemic served as an unprecedented global disruptor, leaving an indelible mark on financial markets. To meticulously quantify its impact on stock volatility, we established **February 20, 2020**, as our critical demarcation date, dividing our dataset into "Pre-COVID" and "Post-COVID" periods.

### 6.1 Investigating Shift in Stock Volatility

Our primary inquiry focused on hwether the volatility (risk) was significantly affected following the COVID-19 pandemic.

H0: σ<sup>2</sup><sub>pre</sub> = σ<sup>2</sup><sub>post</sub>

H0: σ<sup>2</sup><sub>pre</sub> != σ<sup>2</sup><sub>post</sub>

for that purpose we employed Levene's Test, a robust statistical tool, to rigorously assess whether the variance (our chosen measure of volatility) of daily returns for each company underwent a statistically significant change between these two distinct periods.

**our Levene test findings:**

| Company | Std Dev Pre-COVID (Annualized) | Std Dev Post-COVID (Annualized)  | Levene Statistic | P-value | Conclusion                        |
|---------|--------------------------------|----------------------------------|------------------|---------|-----------------------------------|
| AAPL    | 0.2441                         | 0.3181                           | 38.5449          | 0.0000  | Reject H0 (Significant Change)    |
| AMZN    | 0.2785                         | 0.3618                           | 59.0576          | 0.0000  | Reject H0 (Significant Change)    |
| GOOGL   | 0.2225                         | 0.3276                           | 86.3460          | 0.0000  | Reject H0 (Significant Change)    |
| MSFT    | 0.2195                         | 0.3067                           | 56.2356          | 0.0000  | Reject H0 (Significant Change)    |
| NVDA    | 0.4437                         | 0.5422                           | 51.8879          | 0.0000  | Reject H0 (Significant Change)    |

Our statistical findings from Levene's Test indicated a statistically significant change in volatility for most, if not all, of these tech giants in the post-COVID era. This conclusion was vividly supported by our visualizations, which often showed a notably wider spread of daily returns in the post-COVID period. This observed increase in volatility directly reflects the heightened uncertainty, rapid economic shifts, and accelerated digital transformation spurred by the pandemic.

![Total Percentage Stock Growth: Pre-COVID vs. Post-COVID](IWTG%20Results/Total%20Percentage%20Stock%20Growth%20Pre-COVID%20vs.%20Post-COVID.png)

### 6.2 A Comprehensive Exploratory Analysis of the Data

Beyond just volatility, a comparison of total percentage growth in the pre- and post-COVID periods offered a compelling narrative. For nearly every company, the post-COVID era delivered substantially higher total growth, even accounting for the initial market shock. This powerfully underscores how the pandemic, despite its initial market shock, acted as a catalyst for growth across many segments of the tech sector, driving increased adoption of digital services.

![Distribution of Daily Returns: Pre-COVID vs. Post-COVID (Violin Plot)](IWTG%20Results/Distribution%20of%20Daily%20Returns%20Pre-COVID%20vs.%20Post-COVID.png)

A focused visualization on Nvidia further illuminated this acceleration. By overlaying its normalized growth trajectory from the three years before COVID-19 with the three years after, the dramatic steepening of its post-pandemic growth curve became strikingly apparent. This highlights Nvidia's unique position and exceptional capitalization on the shifts towards remote work, online entertainment, and the burgeoning AI landscape.

![Nvidia Stock Growth: 3 Years Before vs. 3 Years After COVID-19 (Normalized)](IWTG%20Results/Nvidia%20Stock%20Growth%203%20Years%20Before%20vs.%203%20Years%20After%20COVID-19%20(Normalized).png)

### 6.3 Examining Intra-day Trading Dynamics

Our analysis also extended to the subtle shifts in intra-day trading dynamics. We observed changes in the proportion of "up" days (where the closing price was higher than the opening price) before and after the pandemic. 

H0: p<sub>post</sub> = p<sub>pre</sub>

H1: p<sub>post</sub> != p<sub>pre</sub>

for that purpose we employed z-test, a robust statistical tool, to rigorously assess whether the proportion percentage of up days (close > open) for each company underwent a statistically significant change from pre covid to post covid.

**our z-test test findings:**

| Company | Prop_Up_Pre (Close > Open)  | Prop_Up_Post (Close > Open)  | Z_Statistic | P_Value  | Conclusion                                 |
|---------|-----------------------------|------------------------------|-------------|----------|--------------------------------------------|
| AAPL    | 0.508434                    | 0.496899                     | 0.408777    | 0.682704 | Fail to Reject H0 (No Significant Change)  |
| AMZN    | 0.508434                    | 0.492248                     | 0.573628    | 0.566220 | Fail to Reject H0 (No Significant Change)  |
| GOOGL   | 0.438554                    | 0.506202                     | -2.397888   | 0.016490 | Reject H0 (Significant Change)             |
| MSFT    | 0.484337                    | 0.509302                     | -0.884763   | 0.376285 | Fail to Reject H0 (No Significant Change)  |
| NVDA    | 0.513253                    | 0.522481                     | -0.327289   | 0.743449 | Fail to Reject H0 (No Significant Change)  |

Interestingly for some companies, like Google, this shift was statistically significant. For the other tech giants (AAPL, AMZN, MSFT, NVDA), we failed to reject the null hypothesis, suggesting no statistically significant shift in this particular intra-day pattern based on our data and chosen significance level. This indicates that even the short-term trading patterns were affected by the new market environment.

![Comparison of Intra-day "Up" Day Proportions: Pre- vs. Post-COVID](IWTG%20Results/Comparison%20of%20Intra-day%20Up%20Day%20Proportions%20Pre-%20vs.%20Post-COVID.png)

![Shift in Intra-day Up Days (Close > Open): Post-COVID vs. Pre-COVID](IWTG%20Results/Shift%20in%20Intra-day%20Up%20Days%20(Close%20%20Open)%20Post-COVID%20vs.%20Pre-COVID.png)

## 7. Glimpsing the Future: Stock Trajectory Prediction

Forecasting stock prices is an inherently complex challenge, often likened to predicting the future. Financial markets are influenced by an intricate web of unpredictable factors, making definitive predictions extremely difficult. However, time series forecasting models can attempt to capture underlying trends, seasonality, and historical patterns to make informed projections about future movements. For this project, we leveraged **Facebook's Prophet library**, a robust and flexible forecasting tool well-suited for capturing various time series components.

We prepared the data by splitting each stock's historical prices into a training set (the majority of the data) and a test set (the most recent six months, which the model had not seen). This allowed us to evaluate the model's predictive accuracy against actual, unseen market behavior.

Our Prophet models were trained for each of the five tech stocks. The resulting visualizations showed that the models generally succeeded in capturing the overall long-term trends and broader movements for these companies. However, consistent with the inherent unpredictability of stock markets, the models struggled to perfectly forecast sharp, sudden price changes or capture the precise daily fluctuations in the unseen test data.

![NVDA Stock Price Prediction (Prophet)](IWTG%20Results/NVDA%20Stock%20Price%20Prediction%20(Prophet).png)

![MSFT Stock Price Prediction (Prophet)](IWTG%20Results/MSFT%20Stock%20Price%20Prediction%20(Prophet).png)

![GOOGL Stock Price Prediction (Prophet)](IWTG%20Results/GOOGL%20Stock%20Price%20Prediction%20(Prophet).png)

![AMZN Stock Price Prediction (Prophet)](IWTG%20Results/AMZN%20Stock%20Price%20Prediction%20(Prophet).png)

![AAPL Stock Price Prediction (Prophet)](IWTG%20Results/AAPL%20Stock%20Price%20Prediction%20(Prophet).png)

The evaluation metrics (Root Mean Squared Error, Mean Absolute Error, and Mean Absolute Percentage Error) provided a quantitative measure of our models' performance. These metrics, while indicating a reasonable fit to the historical data, also underscored the substantial challenge of achieving highly accurate short-to-medium term stock price predictions in a dynamic market environment. The accuracy typically degrades as the prediction horizon extends, and unforeseen events can drastically alter trajectories.

## 8. Conclusion: A Legacy Forged in Data

Our comprehensive analysis of Apple, Amazon, Google, Microsoft, and Nvidia's stock performance from 2016 to 2024 offers a compelling narrative of growth, resilience, and adaptability within the technology sector.

**Nvidia's explosive ascent**, particularly in the post-COVID digital acceleration, stands out as a stark illustration of how a company at the forefront of critical technologies can achieve unparalleled market capitalization. **Microsoft**, on the other hand, consistently demonstrated a remarkable blend of **robust growth and relative stability**, cementing its role as a reliable pillar of the tech market.

The **COVID-19 pandemic** proved to be a powerful, albeit disruptive, catalyst. It profoundly **reshaped the risk profiles** of these companies, leading to statistically significant shifts in their stock volatility. Despite the initial market shock, the pandemic significantly **accelerated growth trajectories** for many tech giants, driven by rapid digital transformation and increased reliance on technology. While their stock movements remained highly correlated, reflecting shared susceptibilities to broader market forces, the intensity of their growth and volatility often surged in the wake of the pandemic.

Our exploration into **stock trajectory prediction** with Prophet offered valuable insights into the patterns embedded within historical data. While precise forecasting remains an elusive goal in the inherently unpredictable financial markets, such models provide useful frameworks for understanding general trends and the underlying momentum of these tech titans.

Ultimately, the stories embedded within this data are not just about numbers; they are narratives of innovation, market adaptation, and the powerful interplay between technological advancement and profound global events. Understanding these data-driven sagas is fundamental to comprehending the essence of modern financial markets and the companies that shape them.

## 9. Limitations & Future Work

### 9.1 Limitations:

*   **Binary Period Definition:** Our analysis relies on a single, sharp demarcation date for "Pre-COVID" and "Post-COVID." In reality, the pandemic's economic and market impacts unfolded gradually, and investor sentiment evolved over time.
*   **Causation vs. Correlation:** While we observe statistically significant changes in volatility and growth *after* the pandemic's onset, our analysis, by nature, establishes correlation, not definitive causation. Other concurrent macroeconomic factors or geopolitical events could also have contributed to these observed shifts.
*   **Normality Assumptions in Testing:** While Levene's test is more robust than others, extreme non-normality in daily returns (which are common in financial data) can still potentially affect the power or Type I error rate of the statistical tests.
*   **Model Simplification (Prophet):** Prophet is a powerful tool, but it simplifies the complex dynamics of stock markets. It primarily models additive/multiplicative trends and various seasonalities. It does not inherently account for complex non-linear relationships, sudden market shocks (unless explicitly modeled as events), or intricate inter-stock dependencies without additional explicit regressors.
*   **Data Granularity:** Using daily returns captures day-to-day volatility but does not delve into intraday dynamics or longer-term structural shifts requiring lower-frequency data.

### 9.2 Future Work:

*   **Advanced Volatility Modeling:** Employ more sophisticated time-series models, such as **GARCH (Generalized Autoregressive Conditional Heteroskedasticity) models**, to explicitly model and forecast time-varying volatility, offering a more dynamic and nuanced view of risk.
*   **Formal Event Study Analysis:** Conduct a rigorous event study to quantify the abnormal returns and volatility around specific, well-defined pandemic-related events (e.g., major vaccine announcements, specific lockdown/reopening news, significant earnings reports during the pandemic).
*   **External Regressors in Forecasting:** Enhance prediction models by incorporating external factors (e.g., key economic indicators like GDP growth, inflation, interest rates; sentiment analysis from news or social media; company-specific fundamental data) as **external regressors** to potentially improve predictive accuracy.
*   **Comparison to Market Benchmarks:** Extend the analysis by comparing the volatility and growth shifts of these tech giants against broader market indices (e.g., S&P 500, Nasdaq Composite) to discern whether their observed changes were unique or broadly reflective of overall market behavior.
*   **Deep Learning for Forecasting:** Explore the application of deep learning models, such as Long Short-Term Memory (LSTM) networks, which are designed to capture complex temporal dependencies in time series data, though this would significantly increase model complexity and computational requirements.
*   **Sector-Specific Analysis:** Broaden the study to include more companies within the tech sector (and perhaps other sectors) to gain a more comprehensive understanding of industry-wide impacts and potential leadership changes.
