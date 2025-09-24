# 🛍️ Female Daily Product Review Scraper  

This project demonstrates my web scraping expertise by extracting product reviews from **[Female Daily](https://reviews.femaledaily.com/)**, one of Indonesia’s largest beauty review platforms.  

The scraper automatically collects:  
- ✅ Product details (name, URL)  
- ✅ Review text and rating (1–5 stars)  
- ✅ Recommendation flag (Yes/No)  
- ✅ Review metadata (date, usage period, purchase point)  
- ✅ Works across multiple products with thousands of reviews  

All data is saved into a structured **CSV file**, making it ready for further **data analysis, NLP, or machine learning**.  

---

## 🚀 Workflow  

### 1. Load all product links  
- Open brand page (e.g., **COSRX**)  
- Click **“Load More”** until all products are displayed  
- Filter only products with **>1000 reviews**  

### 2. Scrape reviews per product  
- Extract review date, rating, text, and purchase details  
- Handle **pagination automatically**  
- Resume from last checkpoint if scraping is interrupted  

### 3. Save results  
- Continuously save reviews into `all_reviews_checkpoint.csv`  
- Ensures progress isn’t lost on errors or timeouts  

---

## 🛠️ Tech Stack  

- **Python** (automation & data handling)  
- **Selenium** – interact with dynamic pages  
- **BeautifulSoup** – parse HTML structure  
- **Pandas** – store and clean data  
- **Regex** – extract review counts  

---

## 📂 Sample Output  

| Product Name            | Review Date | Review Rating | Recommend | Review Text                  | Usage Period | Purchase Point | Product URL | Review Page |  
|--------------------------|-------------|---------------|-----------|------------------------------|--------------|----------------|-------------|-------------|  
| COSRX Low pH Cleanser   | 2023-05-10  | 5             | Yes       | "Great for sensitive skin..." | 1 month      | Official Store | https://... | 1 |  
| COSRX AHA Toner         | 2023-05-12  | 4             | Yes       | "Mild exfoliation, works well" | 2 months     | Online Shop    | https://... | 2 |  

---

## 📊 Results  

- 🔗 Scraped **2 COSRX products**  
- 📝 Collected **8,500+ reviews**  
- 💾 Stored in a clean **CSV format**
- 📊 The complete scraped dataset is available on [Kaggle](https://www.kaggle.com/datasets/jessicaberliani/female-daily-cosrx/data).

---

