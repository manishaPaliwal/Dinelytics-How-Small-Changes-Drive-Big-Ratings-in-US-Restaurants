# 🍽️ **Dinelytics: Uncovering What Drives Restaurant Ratings with Yelp + Income Data**

## 📌 **Project Overview:**
**Dinelytics** is an end-to-end data engineering and analytics project exploring **US restaurant trends using Yelp, Census, and Zip Code data**. We analyzed **how income, business attributes, reviews, and ambiance impact restaurant ratings**—building insights to help restaurant owners and investors make data-driven decisions.

We engineered a complete AWS pipeline, integrating **S3, Glue, Redshift, Python, Tableau, and AWS S3-hosted website** to deliver actionable dashboards and visual stories.

---

## 🏗️ **Tech Stack & Their Roles in Dinelytics:**

✅ **AWS S3** – Storage for raw Yelp JSON, Census CSV, Zip Codes CSV; also hosted the static website  
✅ **AWS Glue** – ETL tool to cleanse Yelp JSON, flatten nested attributes, transform data for Redshift  
✅ **AWS Redshift** – Data warehouse for structured tables (Businesses, Reviews, Income, Zip Codes, Attributes)  
✅ **Python (Jupyter Notebook)** – Parsing nested JSON, additional wrangling, CSV exports, data validation  
✅ **MySQL EER Diagram** – Schema design visualization prior to Redshift implementation  
✅ **Tableau Public** – Built dashboards for insights: cuisine trends, price vs rating, attribute impacts, reviews  
✅ **AWS S3 Static Website Hosting** – Hosted the project website publicly without backend servers  
✅ **AWS EC2 (optional)** – Ran Python scripts or intermediary steps outside Glue environment

---

## 💡 **What Makes Dinelytics Unique:**

✨ **Multi-source data integration** → Linked Yelp data with US Census income and Zip Codes for richer analysis  
✨ **End-to-end AWS-native pipeline** → S3 → Glue → Redshift → Tableau → S3-hosted website  
✨ **Flattened nested JSON fields (ambience, attributes)** → Python-parsed for queryable schema  
✨ Insights go beyond Yelp → explored **how income, reviews, and business attributes shape ratings & customer perception**  
✨ Delivered **action-oriented dashboards** → e.g., small attribute changes (like allowing dogs or adding table service) boosting 2-star restaurants

---

## 📊 **Key Insights:**

🍔 **American, Sandwiches, Fast Food, and Mexican cuisines dominate US markets**  
⭐ **More reviews = better average rating** (until diminishing returns)  
💵 **Higher-income counties don’t always favor expensive restaurants**  
🏙️ **Top restaurant chains (by count) aren’t the highest-rated**  
📝 **2- and 3-star reviewers write the longest, most constructive feedback**  
🏡 **Business attributes like Table Service, Good for Groups, Credit Card acceptance improve ratings**

---

## ✅ **What Went Well:**

🌟 Delivered a **fully cloud-native pipeline from raw JSON → cleaned → Redshift → Tableau**  
🌟 Successfully integrated **income + zip code mapping** into Yelp data  
🌟 Created a **hosted static website** sharing dashboards and project artifacts  
🌟 Identified **"quick wins" for low-rated restaurants** through attribute analysis

---

## ⚠️ **Challenges We Solved:**

😅 Parsing **nested JSON attributes (ambience, business attributes)** into usable columns  
😅 Resolving **missing Zip → County mappings** via external datasets  
😅 Optimizing **Glue → Redshift ETL flow** for large JSON and CSV loads  
😅 Query optimization for **multi-table joins powering Tableau dashboards**  
😅 Cross-browser testing of the **AWS S3-hosted static website** for compatibility

---

## 🏆 **Why This Tech Stack Was Powerful:**

✅ Cloud-native, scalable, and cost-efficient  
✅ Glue eliminated need for managing ETL servers  
✅ Redshift allowed **fast querying across millions of Yelp records**  
✅ Tableau brought insights to life with interactive visual storytelling  
✅ S3 static website enabled **low-cost global access without backend complexity**

---

## 🔍 **Final Takeaway:**
✅ **Restaurant ratings aren’t driven solely by price or chain size—customer experience attributes and review count play a bigger role than cost or popularity.**

✅ Even small operational tweaks (adding table service, dog-friendly zones, credit card acceptance) can help 2-star restaurants improve ratings.

---

## 🚀 **Future Scope:**

➡️ Perform **sentiment analysis on reviews**  
➡️ Correlate restaurant density with **population and area data**  
➡️ Build **ML models to predict rating improvement strategies**  
➡️ Expand static website into a full web app dashboard  

---

## 🔗 **Explore Dinelytics:**

👉 Tableau Dashboard: [View Dashboard](https://public.tableau.com/app/profile/manisha.paliwal/viz/YelpInsightsByAbracaData/YelpInsights?publish=yes)  
👉 Live Website (AWS S3): [Yelp Insights Website](https://websiteyelpinsights.s3.us-west-1.amazonaws.com/YelpInsightsWebsite/Home.html)

