# Starbucks-Customer-Segmentation

As someone who enjoys coding and staying updated on the latest trends, I became interested in the role of data science in marketing, especially after watching *"The Social Dilemma"* on **Netflix**. It made me realize how companies, like Starbucks, use massive amounts of data to personalize their marketing strategies. This sparked my curiosity about how Starbucks' rewards program works, particularly how it encourages customers to deposit money into their rewards accounts and how this data is leveraged.

I read an article discussing how Starbucks earns revenue through the interest on funds in these accounts. This got me thinking about how data science could be applied to segment Starbucks customers based on their responses to different offers, which could help improve marketing strategies. 

Being someone with a passion for both coffee and business, I decided to work on a project that uses data science techniques to segment customers and analyze their behaviors. The goal is to help the marketing team optimize their strategies, and it’s been a great opportunity to blend my love for coffee with my interest in data science and problem-solving.

<p float="left">
  <img src="https://media.licdn.com/dms/image/v2/D5612AQHIfhYYdvpdMA/article-cover_image-shrink_720_1280/article-cover_image-shrink_720_1280/0/1710479763411?e=2147483647&v=beta&t=zLyw1_JVfFD7dvvr-O4-1UzKVcQvjnurr1WGg-_6oXg" width="45%" />
  <img src="https://starbucksstatic.cognizantorderserv.com/Items/Small/103515.jpg" width="45%" />
</p>

- **ML Techniques used**: K-Means, PCA, t-SNE, Gaussian Mixture Models, Silhouette plot, SSE/Inertia, Cluster Analysis
- **Project Domains**: Market Segmentation, Marketing, Data Science, Cluster Analysis

### Q: Why segment customers?

Ans - Well, because it is still a very difficult and computationally intensive task to target each customer in unique ways. As well as there would be lots of customers on which similar Marketing strategies and Discount offers would work well. Hence, it makes intuitive sense to break the customer base into clusters on the basis of how and which offers they react to and then proceed to make targeted strategies.

# If I had a minute to tell u about this project -

* Coffee, Business, Marketing, Data Science , Action !

* Performed Data Engineering to merge the 3 datasets, performed Data Cleaning (Some enteries were errors cause their data was missing as well as age was 118 which seemed to be an error). (coe == customer offer engagement)
![Biz](https://private-user-images.githubusercontent.com/86561124/268485273-c0a1feb4-1d85-447b-baf9-54024092318d.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzM5MzQ3NDAsIm5iZiI6MTczMzkzNDQ0MCwicGF0aCI6Ii84NjU2MTEyNC8yNjg0ODUyNzMtYzBhMWZlYjQtMWQ4NS00NDdiLWJhZjktNTQwMjQwOTIzMThkLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEyMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMjExVDE2MjcyMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTczYmE3OTNjN2FiODVlZWNhZmYyZGYyMzc3OWRlZjE4NWEwY2U5NGVhNWFkZGUxZTE1NDZiMWU1YjkzMDYyMjUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.1ysAuaOLgRgSIkJVwW8h4RkjhUnYn9eBCQN3JuW55ns)

* Used Power Transforms to make dataset more gaussian since K-means likes rounder (isotropic) clusters.

* Performed PCA ( Principal Component Analysis ) to reduce Data Dimensionality and avoid Curse of Dimensionality , and also so that redundant features would be removed and the data would be in continuous so that we don't need to bother ourselves with K-Prototype kind of algorithms ( its K-means plus K-mode for mixed (continuous plus categorical) data modelling )

![Insight1](https://private-user-images.githubusercontent.com/86561124/268485347-1a255f79-1cc9-4951-a4b7-80d41a1d8a93.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzM5MzQ3NDAsIm5iZiI6MTczMzkzNDQ0MCwicGF0aCI6Ii84NjU2MTEyNC8yNjg0ODUzNDctMWEyNTVmNzktMWNjOS00OTUxLWE0YjctODBkNDFhMWQ4YTkzLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEyMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMjExVDE2MjcyMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWFhNzFhYjU5MWVjOWJmNDUzZGZkN2NhNjBjZTYyMDdhZWI2NTk0Y2NkZDg3ZTAzMjEzZTM1YTc2MmU5ZmRhMjImWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.8Syp3WAJr-nMfDzf0o6H6oOcR8D5Zq5-OnbIsu9wNkE)

* Used K-means clustering to form clusters, along with Silhouette score and SSE(Sum of Squared Errors)/Inertia to determine optimal number of clusters, and then Silhouette Plots to further analyse quality of clusters.
![Insight2](https://private-user-images.githubusercontent.com/86561124/268485381-155c5309-a368-4d9d-b12b-5e11b42cc21c.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzM5MzQ3NDAsIm5iZiI6MTczMzkzNDQ0MCwicGF0aCI6Ii84NjU2MTEyNC8yNjg0ODUzODEtMTU1YzUzMDktYTM2OC00ZDlkLWIxMmItNWUxMWI0MmNjMjFjLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEyMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMjExVDE2MjcyMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTNiZmQyNDBlNDAxNDhjYTUzMjQwYzZmOTMwNTdjN2U0OTg1MzRlNDJlMzg5ZGFiMDFiYmNkN2E5Njk5ZjJkZWQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.pUUGGsc_8IXt4ZhVFavLfpoLxNA7bxwXgA99wj6dJkc)

![Insight3](https://private-user-images.githubusercontent.com/86561124/268485609-8d942e41-e5d4-4a51-baa5-d3b98c8eb68b.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzM5MzQ3NDAsIm5iZiI6MTczMzkzNDQ0MCwicGF0aCI6Ii84NjU2MTEyNC8yNjg0ODU2MDktOGQ5NDJlNDEtZTVkNC00YTUxLWJhYTUtZDNiOThjOGViNjhiLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEyMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMjExVDE2MjcyMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPThiMzA1MTkxNjI1YTBhYWMzNTdiNWMxNDBkMTdiNzBkYjMxNTMwMjRjYWM4ZDVkYzdlNTA3ZGFkNjUzMTFmOTUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.EZFOznIAlN8rXMfAjrOI1F_vaBDuxNmn3CJpgO3XQ0s)

* Visualized Clusters in 2-D using t-SNE to further confirm the feasiblity of clusters.
* Performed Gaussian Mixture Modelling since it is a Generative and not Discriminative classifier, also it's a soft classifier, to allow further scope for data-points on borders of clusters or customers which behave like 2 or more clusters. Also it can form "non-round" clusters better too.


![Insights4](https://private-user-images.githubusercontent.com/86561124/268485617-0ab1cd2a-f119-41d3-9087-843c254f21ba.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzM5MzQ3NDAsIm5iZiI6MTczMzkzNDQ0MCwicGF0aCI6Ii84NjU2MTEyNC8yNjg0ODU2MTctMGFiMWNkMmEtZjExOS00MWQzLTkwODctODQzYzI1NGYyMWJhLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEyMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMjExVDE2MjcyMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWNlMjgxM2U0NTc3MTVhZDMwYWNmMWU3MjNiZDVkYzc5MTk0MDUxNGJjZTU5YmQyYjg2MTIwNzU5MzhmNzNjMmMmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.df-Vc8GM6wCGn5nXZljgWDLhjHgNVs6g-aVRkJ9_Pjg)

* Performed **Cluster Analysis** to determine properties and behaviours of clusters, understood the physical significance of the clusters in real life, and went ahead to think of how the company should make different strategies for these clusters.


![Insight5](https://private-user-images.githubusercontent.com/86561124/268485805-4c00ceb4-8854-4e78-a2d9-37ae7697cc90.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzM5MzQ3NDAsIm5iZiI6MTczMzkzNDQ0MCwicGF0aCI6Ii84NjU2MTEyNC8yNjg0ODU4MDUtNGMwMGNlYjQtODg1NC00ZTc4LWEyZDktMzdhZTc2OTdjYzkwLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEyMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMjExVDE2MjcyMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTI2MjNhMzRlOTkwZWEwYzkyM2Y2OGUyZTQxMTY4ZDE3NWJmMmNmNGQ4M2JmZTBjNWYyOTRlYjNmMDY0YTNiZmImWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.0_JbxdjfWcS4nnnWj3yhi9DUphju2kg0UM4-zadSRaM)
![Insight6](https://private-user-images.githubusercontent.com/86561124/268485886-54e5b072-98b6-4ebb-ae5a-249c78387f0b.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzM5MzQ3NDAsIm5iZiI6MTczMzkzNDQ0MCwicGF0aCI6Ii84NjU2MTEyNC8yNjg0ODU4ODYtNTRlNWIwNzItOThiNi00ZWJiLWFlNWEtMjQ5Yzc4Mzg3ZjBiLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEyMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMjExVDE2MjcyMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTY3ODJkYjAyZmI3NzJmYzg5MmNmYzZlNTgwY2IxMTg2MjcxMmJhYWI5ZTgyMTNkZGIzZjgxZTE2YTI5OTQ4YTEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.SsuB6PRIJSSf_FQw7zq32d1YY3kow220FeFudPjLN1s)

* Studied present Starbucks site to see their presently deployed marketing strategies for a new customer. Developed Product Understanding and understanding of UI/UX for marketing used by them.


![Image](https://private-user-images.githubusercontent.com/86561124/268486022-f9dc02b5-9f9f-4196-96e5-dfe57887d4b0.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzM5MzQ3NDAsIm5iZiI6MTczMzkzNDQ0MCwicGF0aCI6Ii84NjU2MTEyNC8yNjg0ODYwMjItZjlkYzAyYjUtOWY5Zi00MTk2LTk2ZTUtZGZlNTc4ODdkNGIwLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEyMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMjExVDE2MjcyMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTk2MjY3NGRkODY4ZGZiOGEzYzg4ODJlYzc1YmJjZDkzMDliZDcwNTRmMzk3OTMxZGFkY2Y1YWVjOGM2NzdlOTAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.83GhLvW-YBY1upl0pHU3EKnDIN0wZOjqKWl7lwm8lZQ)

# My findings
(Hereby might refer to clusters as "segments" too sometimes)
* One cluster resembled people who were probably young office going people who were our regular customers, this is the customer segment which provides us the most monetary value currently. They react well to all offers, since they are regulars they already know the ins-and-outs of our schemes and hence use offers regularly. In my opinion, we can leave them as it is going, or even reduce the number of offers given to them slightly as long as they don't seem to be running away from us.
* Another cluster had a lot of Rich, older members of reward program who usually react to discounts but not to BOGO's (Buy One Get One). A clear indication is that they like to drink coffee alone, and we can give them more discount offers than anything which requires them to buy more than one food item, and specifically not give them a BOGO offer.
* Another customer segment was behaving in such a way that they only come to Starbucks when there is an offer (Us bhai us) , and their non-offer period spending is very low. I feel that by giving them small but regular offers on weekends, we can convert them to regular customers.
* Another cluster resembled lower-income groups which did not seemed to be tempted by any type of offers. Either starbucks can introduce lower cost drinks to target these, or it can maintain its brand image and ignore these customers. Since India is a price sensitive market, to thrive in such a market it wouldn't hurt much to introduce a few "Mid-Priced" meals targetting middle class customers, and then slowly introducing combo-meals where we can sell a mid-priced and high priced item together in the name of discount.
* One cluster had people who are moderate customers, with an okayish amount of spend, and I feel it is best to leave them as it is, and give them offers only when their frequency seems to have decreased.
* The last cluster had no appreciable features, some of them were "ghosts" who had come only once or twice, and had very irregular patterns. Which , is a gentle remainder that all things which make sense mathematically do not have to make business sense .

# The Starbucks Website Analysis
* The website was designed in such a way to pull all the customers to its Rewards program , which makes intutive sense since Starbucks is earning free money from the intrest .


![Websiteimg](https://private-user-images.githubusercontent.com/86561124/268487290-d174a74b-e9aa-4673-bf1f-b69ef68093c9.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzM5MzQ3NDAsIm5iZiI6MTczMzkzNDQ0MCwicGF0aCI6Ii84NjU2MTEyNC8yNjg0ODcyOTAtZDE3NGE3NGItZTlhYS00NjczLWJmMWYtYjY5ZWY2ODA5M2M5LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEyMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMjExVDE2MjcyMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTE5NjBjYTNkZTdiNzEyZTg5N2ZmNDA2ZmEzNzdlZmU5MjU2YzUwNDcwMjMyNGQ0OGRjZjU4ZTgyOWQ4MTNlY2UmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.Fhgyp2uINlOihk9f-DRjAQH9Kp4ZaLFW5e8-8WGmsk0)


* The prices weren't revealed until the billing time, since the feeling of "loosing" money would drive away customers.


![Websiteimg2](https://private-user-images.githubusercontent.com/86561124/268487401-bd2f5ef0-8b55-4ec7-adcd-f06f9086b373.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzM5MzQ3NDAsIm5iZiI6MTczMzkzNDQ0MCwicGF0aCI6Ii84NjU2MTEyNC8yNjg0ODc0MDEtYmQyZjVlZjAtOGI1NS00ZWM3LWFkY2QtZjA2ZjkwODZiMzczLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEyMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMjExVDE2MjcyMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTQxOTY1YTJhMDhiZmQwNWZkNzhjNzBkNzQ2MTJiM2E5YjZlZGZhYWIyMGEwNzUyMGY0Njk5NTYyOGEwNDQzYWMmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.-z-YKT-xEwqAMiBkftMMgu2UCkNPngwAHV2tIJac1cI)


* Simple, and clear cut message to anyone who opens the rewards tab. Luring them to join rewards program. Marketing in its true sense.


![Websiteimg3](https://private-user-images.githubusercontent.com/86561124/268487534-c56cbacf-6848-4f34-87a0-517aa40e802d.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MzM5MzQ3NDAsIm5iZiI6MTczMzkzNDQ0MCwicGF0aCI6Ii84NjU2MTEyNC8yNjg0ODc1MzQtYzU2Y2JhY2YtNjg0OC00ZjM0LTg3YTAtNTE3YWE0MGU4MDJkLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDEyMTElMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQxMjExVDE2MjcyMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTZkYWYwZjUwOWZmMTlkZDcxZjIyMjgxN2QwYmU3ZWJiZDhiMjg3N2QzNjM2MDIzMGI0ZWFjN2RjZDg1MGRjODImWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.29q_a2s4D9-vdjKkxaOHX1PP_i22HHDNM5VKKb3OlKE)
