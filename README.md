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

| Product Name                          | Review Date | Rating | Reviewer Comment                                                                                                                                                                                                 | Usage Period        | Purchase Point | Product URL                                                                                                                        | Review Page |
|---------------------------------------|-------------|--------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------------|----------------|------------------------------------------------------------------------------------------------------------------------------------|-------------|
| AHA/BHA Clarifying Treatment Toner    | 09 Apr 2025 | 5      | Aku udah langganan pake ini. Sampe sekarang masih pake. Udah 3 tahun pake dan puas banget. Puas banget sama toner ini. Bikin seger juga. Kalian yang pemula terus pengen nyoba pake toner AHA/BHA ini cocok banget. Terus isinya banyak jadi hemat banget. Love parahhhh. Emang COSRX tuh bagus-bagus semua gaesss. | More than 1 year    | Shopee         | [Link](https://reviews.femaledaily.com/products/cleanser/toner/cosrx/aha-bha-clarifying-treatment-toner)                           | 1           |
| Low pH Good Morning Gel Cleanser      | 08 Feb 2025 | 5      | Cosrx low Ph good morning gel cleanser tipe facial wash tekstur gel gentle dengan busa sedikit tapi puas ngerasa bersih di wajah dan engga bikin kulit kering dan ketarik. Cocok buat kulit kering kombinasi dan ga bikin breakout di wajah. | 6 months - 1 year  | Shopee         | [Link](https://reviews.femaledaily.com/products/cleanser/facial-wash/cosrx/good-morning-gel-cleanser)                             | 6           |

---

## 📊 Results  

- 🔗 Scraped **2 COSRX products**  
- 📝 Collected **8,500+ reviews**  
- 💾 Stored in a clean **CSV format**
- 📊 The complete scraped dataset is available on [Kaggle](https://www.kaggle.com/datasets/jessicaberliani/female-daily-cosrx/data)

---

