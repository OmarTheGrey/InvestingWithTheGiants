# InvestingWithTheGiants

# Comprehensive Stock Performance Analysis of Leading Tech Giants (2018-2024)

## Abstract

This report presents a comprehensive data analysis of the stock performance of five major technology companies: Apple (AAPL), Amazon (AMZN), Google (GOOGL), Microsoft (MSFT), and Nvidia (NVDA), spanning from early 2018 to late 2024. Leveraging historical daily stock data, this study explores their individual growth trajectories, quantifies their risk-reward profiles, and investigates the profound impact of the COVID-19 pandemic on their financial volatility. Furthermore, it delves into the interconnectedness of these tech giants and presents an attempt to forecast their future stock trajectories using time series models. The findings reveal distinct narratives of growth, resilience, and adaptability within the tech sector, highlighting Nvidia's explosive ascent and Microsoft's consistent stability, while also underscoring the market's dramatic shifts in response to global events.

## 1. Introduction: The Tech Titans' Arena

In an era defined by rapid technological advancement, the digital landscape is dominated by a handful of companies that have not only revolutionized industries but have also become titans in the financial markets. Apple, Amazon, Google, Microsoft, and Nvidia stand as beacons of innovation and economic power. Understanding their historical stock performance is crucial for investors, analysts, and anyone keen on deciphering market dynamics.

This project embarks on a data-driven journey to dissect the stock stories of these five giants. Our objectives are multifaceted: to visualize their paths to growth, assess their inherent risks, quantify the impact of a global disruptor like COVID-19, understand how their movements are intertwined, and explore the possibilities (and limitations) of predicting their future.

## 2. Unveiling the Journey: Price & Growth Trajectories

Our initial glimpse at the raw closing prices reveals a stark difference in absolute values across companies. While some stocks like Google and Amazon trade at higher dollar amounts, this raw view can be misleading when comparing overall performance. It simply shows current price levels, not how much an investor would have gained relative to their starting point.

To truly understand which companies delivered the most impressive returns, we normalized their prices. By setting all stocks to a base value of 100 at the start of our analysis period (January 2, 2018), we could clearly visualize their percentage growth trajectories. This transformed the narrative: Nvidia emerged as the undisputed champion of growth, showcasing an explosive upward trend, particularly in the later years. Microsoft demonstrated remarkably strong and consistent growth, while Apple also delivered substantial, though less dramatic, percentage gains. Amazon and Google, while ultimately achieving significant growth, exhibited more pronounced volatility along the way.

## 3. The Balance Act: Risk vs. Reward

Beyond mere growth, investors are keenly interested in volatility, a key measure of risk. Our analysis of daily returns shed light on the "ride" accompanying these growth stories. Typically, higher returns come hand-in-hand with higher volatility.

By examining the distribution of daily returns and calculating annualized volatility, we found that Nvidia, while delivering exceptional growth, also experienced the highest volatility, confirming its status as the most thrilling, yet potentially turbulent, investment among the group. Microsoft, however, presented an impressive balance, offering substantial returns with comparatively lower volatility, positioning itself as a reliable blend of growth and stability. Apple, too, proved to be a relatively steady performer, providing good returns with manageable risk. Amazon and Google generally occupied a middle ground, with decent returns but more pronounced daily swings compared to Microsoft and Apple.

## 4. The Investor's Story: Hypothetical Returns

To make these abstract growth figures tangible, we simulated a hypothetical investment: what if an investor had put $1000 into each of these tech giants at the beginning of our dataset (February 19, 2020), holding them until the end of 2024?

The results vividly illustrate the immense wealth generation potential. Nvidia's growth was truly extraordinary, transforming an initial $1000 into over $17,000 – a staggering 1614% return. While Apple, Google, and Microsoft also delivered significant returns (ranging from 135% to 219%), and Amazon a solid 102%, Nvidia's performance dwarfed them all. This highlights the powerful effect of compounding returns and the outsized impact of leading high-growth companies.

## 5. Market Pulse: Trading Volume & Interconnectedness

Trading volume offers insights into investor interest and market activity. Our analysis showed a general upward trend in trading volume for most companies over the years, signaling increased market participation. Nvidia, in particular, consistently commanded exceptionally high trading volumes during its rapid growth phase, reflecting intense investor activity and liquidity. These volume spikes often coincided with major news events or earnings reports, indicating heightened market reactions.

Furthermore, we examined the correlation between the daily returns of these tech giants. As anticipated for large-cap companies within the same sector, all five exhibited a high degree of positive correlation (generally above 0.5 and often above 0.6-0.7). This strong positive correlation implies that these stocks tend to move in the same direction, influenced by broader market trends. From a portfolio diversification standpoint, this suggests that holding only these tech giants would offer limited protection against downturns specifically affecting the broader technology sector.

## 6. The COVID-19 Divide: Pandemic's Impact on Volatility

The COVID-19 pandemic marked a pivotal moment in global markets. To quantify its impact on stock volatility, we chose February 20, 2020, as the demarcation date, splitting our data into "Pre-COVID" and "Post-COVID" periods. We then performed Levene's Test, a robust statistical tool, to determine if the variance (a measure of volatility) of daily returns for each company significantly changed between these two periods.

Our findings indicated a statistically significant change in volatility for most, if not all, of these tech giants in the post-COVID era. This was often visually supported by violin plots, which clearly showed a wider spread of daily returns (larger "violins") for many companies in the post-COVID period. This increase in volatility was a direct consequence of the unprecedented uncertainty, rapid economic shifts, and accelerated digital transformation brought about by the pandemic.

Looking at the total percentage growth for each company before and after COVID-19 provided an even more compelling picture. For nearly every company, the post-COVID period delivered significantly higher total growth than the pre-COVID period. This phenomenon underscores how the pandemic, despite its initial market shock, acted as a catalyst for growth in many tech sectors, driving increased adoption of digital services. Interestingly, the proportion of intra-day "up" days (where closing price was higher than opening) also shifted for some, notably Google, indicating a change in the intraday trading dynamics as well.

## 7. Glimpsing the Horizon: Stock Trajectory Prediction

Forecasting stock prices is a challenging endeavor due to the inherent unpredictability of financial markets. However, time series models can identify and project historical patterns. For this project, we utilized Facebook's Prophet library, known for its ability to handle trends and seasonality in time series data. We split our data into a training set (up to roughly 6 months before the end of the dataset) and a test set (the final 6 months) to evaluate the model's accuracy on unseen data.

For each tech stock, the Prophet model was trained on the historical data, and then used to predict prices for the test period. The visualizations showed the model generally captured the overall trends and large-scale movements for these companies. However, like any forecasting model in a dynamic market, it struggled to perfectly predict sharp, sudden turns or daily fluctuations, particularly during periods of high volatility. This is an expected limitation, as Prophet primarily models underlying trends and periodic patterns, not unforeseen market shocks or complex non-linear interactions. While root mean squared error (RMSE), mean absolute error (MAE), and mean absolute percentage error (MAPE) metrics provided quantitative assessments of prediction accuracy, they also highlighted the inherent challenges of forecasting in volatile financial environments.

## 8. Conclusion: A Legacy Forged in Data

The journey through 15 years (2018-2024) of stock data for Apple, Amazon, Google, Microsoft, and Nvidia has revealed a compelling story of growth, resilience, and adaptation within the technology sector. Nvidia's explosive ascent, particularly in the post-COVID digital acceleration, stands out as a testament to the transformative power of its technology. Microsoft, on the other hand, demonstrated a remarkable blend of robust growth and consistent stability, cementing its role as a reliable pillar of the tech market.

The COVID-19 pandemic acted as a powerful catalyst, profoundly reshaping the risk profiles and accelerating the growth trajectories of these companies. While their stock movements remained highly correlated, indicating their shared susceptibility to broader market forces, the intensity of their growth and volatility often surged in the wake of the pandemic.

Our foray into stock prediction with Prophet offered valuable insights into the patterns embedded in historical data. While precise forecasting remains an elusive goal in financial markets, such models provide useful frameworks for understanding general trends and the underlying momentum of these tech titans.

Ultimately, this analysis underscores that the stories of these tech giants are not just about numbers; they are narratives of innovation, market adaptation, and the powerful interplay between technological advancement and global events. Understanding these data-driven sagas is key to grasping the essence of modern financial markets.
