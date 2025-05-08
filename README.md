The objective of this project was to perform a comprehensive Exploratory Data Analysis (EDA) on the Ford GoBike System Dataset, a public dataset containing ride-sharing trip data collected in the Greater San Francisco Bay Area. The dataset includes variables such as trip duration, station locations, bike IDs, timestamps, user demographics (like gender and age), and user type (Subscriber or Customer). The core aim was to uncover patterns, trends, and business-critical insights by using statistical exploration and data visualization techniques — following the UBM structure (Univariate, Bivariate, Multivariate analysis).

Business Objective The primary business goal was to investigate the factors affecting trip duration, a key performance metric that directly impacts revenue generation for the bike-share system. Additionally, we aimed to understand seasonal patterns, user behaviors by type, and demographic influence to help design better marketing strategies, service plans, and user acquisition/retention tactics.

Data Preparation & Cleaning

The dataset was first loaded, and then several data preprocessing steps were applied:

-Missing values in fields like member_gender and member_birth_year were identified and handled.

-Data types were converted appropriately (e.g., date columns to datetime format).

-A new field age was derived from the member_birth_year for meaningful demographic analysis.

-Outliers were detected and filtered (e.g., extremely long trip durations were capped to improve visual clarity).

-Columns were renamed or formatted for consistency and ease of use.

Univariate Analysis (U)

We explored the distribution of individual variables using histograms, bar charts, and pie charts:

-Trip duration was found to be right-skewed, with most trips under 30 minutes.

-User type distribution revealed that a large majority (~75%) were Subscribers, indicating a stable user base.

-Gender and age distributions showed male dominance, with most riders between the ages of 25 and 45.

-Temporal variables like hour, weekday, and month revealed peak usage during weekdays and working hours, aligning with commuter behavior.

Bivariate Analysis (B)

This part focused on the relationship between two variables at a time:

-Subscribers tend to take shorter, more frequent trips, while Customers often have longer trip durations.

-Trip duration vs. age showed younger riders tend to take longer trips, especially among casual users.

-Day-of-week and user type analysis confirmed that Subscribers use the service more during weekdays, whereas Customers peak during weekends.

Multivariate Analysis (M)

Using correlation heatmaps, pair plots, and segmented visualizations:

-We found weak correlations between trip duration and numeric features like latitude/longitude and age.

-Pair plots gave visual confirmation of segmentation in trip behavior based on age and user type.

-Combining gender, user type, and trip duration, we identified potential demographic targets for expanding market reach.

Key Insights and Business Impact

-User type is the most influential factor in determining trip duration — which is closely tied to revenue.

-Weather and month have negligible impact, but day of the week and hour of day are significant usage predictors.

-The company can increase revenue by converting more casual users into subscribers via loyalty offers or weekend promotions.

-Gender and age segmentation can help create targeted campaigns to diversify and grow the user base.

Conclusion

This analysis provided deep insights into how various factors influence trip duration and user behavior in a bike-share system. With these findings, the business can take data-driven actions to optimize marketing strategies, improve customer experience, and boost overall usage and revenue. The code was written in a modular, exception-handled, and deployment-ready manner with over 20 insightful visualizations, making it ready for presentation and scaling.
