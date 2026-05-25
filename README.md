# Customer Perception & Text Mining Analysis: Southwest Airlines

## 📊 Project Overview
This project examines domestic aviation market trends and leverages text mining to evaluate customer perception of Southwest Airlines. Between 2018 and 2022, Southwest Airlines experienced a drop in domestic market share from **20% to 17%**, losing its position as the top US domestic carrier to American Airlines. To understand this decline, this project utilizes Natural Language Processing (NLP) and Latent Dirichlet Allocation (LDA) topic modeling to analyze unfiltered consumer discussions and pinpoint key structural and service pain points affecting Southwest's customer acquisition and retention.

---

## 🔍 Problem Statement
Despite its historic uniqueness—operating with a single-class cabin (economy only) and an open seat selection policy, Southwest Airlines faces decreasing consumer preference. Traditional customer feedback channels (like surveys) are often limited by response bias. This project explores the question: **What are the genuine, unprompted consumer perceptions and structural issues causing customers to choose competitors over Southwest Airlines?**

---

## 🛠️ Data Pipeline & Methodology
The project follows a text-mining data pipeline managed using **Python, Excel, and Tableau**:
[Data Gathering] ➔ [Data Filtering & Cleaning] ➔ [LDA Topic Modeling] ➔ [Sentiment & Visual Analysis]

1. **Data Gathering:** Scraped an initial dataset of **39,443 text comments** from the popular online forum community `r/Travel` (7.2M subscribed members) to capture organic airline travel discussions.
2. **Data Filtering & Cleaning:**
   * **Issue:** The raw dataset contained severe noise from non-airline travel discussions. 
   * **Solution:** Applied an "Airline" filter keyword match and performed typical NLP preprocessing (tokenization, lowercase conversion, and removing English stopwords).
   * **Result:** Extracted a refined corpus of **5,878 highly relevant comments** spanning 2,624 unique authors.
3. **Exploratory Text Statistics:**
   * Total corpus size: 363,752 words.
   * Average comment length dropped from ~62 words down to ~32 words after stopword elimination.
4. **Data Mining (Topic Modeling):** Applied **Latent Dirichlet Allocation (LDA)** to mathematically cluster vocabulary into 8 distinctive operational and brand clusters across the industry.
5. **Visualization:** Built semantic Word Clouds and structural charts in Tableau to visually interpret sentiment factors.

---

## 📈 Key Findings & Insights
The 8-cluster LDA topic modeling revealed how consumers contrast Southwest with other domestic and international carriers:

* **The Southwest Boarding Bottleneck (Cluster 5):** Text mining explicitly grouped Southwest with sentiments describing their famous open-seating format as a **"stupid boarding procedure"**. While Southwest saves operational costs with this setup, it causes measurable anxiety and frustration for modern fliers compared to conventional seat assignment.
* **Competitive Contrast Matrix:** * *Expedia (Clusters 1 & 3):* Highlighted consumer reliance on third-party aggregators, emphasizing a desire for direct carrier contact and flexible booking.
  * *Legacy/International Competitors (Clusters 2 & 4):* Qatar Airways and Singapore Airlines heavily clustered with terms around "direct routes to popular destinations" and "excellent customer service," setting a premium standard that domestic low-cost models struggle to match organically.
  * *United & Alaska Airlines:* United clustered positively around an "absence of rebooking fees" (threatening a legacy Southwest value proposition), while Alaska and Spirit heavily clustered around "luggage and landing delays" and "hidden add-on fees".

---

## 💡 Strategic Recommendations
Based on the text mining insights, Southwest Airlines can reverse market share loss by adopting the following data-driven adjustments:

1. **Re-evaluate the Boarding & Seating Experience:** Given the negative sentiment clustering around the open boarding configuration, Southwest should introduce preferred or assigned seat selection tiers to alleviate passenger friction and capture premium-economy customer segments.
2. **Expand Route Architecture:** Add direct routes to high-demand domestic hubs and introduce strategic **international flight operations** to directly compete with premium legacy carrier expansion.
3. **Diversify Revenue Streams:** Capitalize on underserved cargo capacity by allowing and optimizing small-scale freight operations to offset passenger revenue fluctuations.
4. **Regulatory & Policy Transparency:** Keep consumer policies highly compliant with emerging government consumer protection mandates (such as automated flight refund rules) to match competitors like United who score positively on rebooking flexibility.
