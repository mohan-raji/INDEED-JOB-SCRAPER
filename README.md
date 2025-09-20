# Indeed Scraper using Apify

This project scrapes job postings from **Indeed** using the [Apify Indeed Scraper](https://apify.com/misceres/indeed-scraper).  
It fetches job details (title, company, location, salary, job type, rating, reviews, posted date, apply link, and description) and saves the results into a clean **Excel file**.

---

## 🚀 Features
- Fetch job postings from Indeed automatically  
- Extracts and cleans job descriptions (removes HTML)  
- Saves results in a structured Excel file  
- Keeps API keys secure with `.env`  

---

## 📂 Project Structure
```text
├── indeed_scrapper.py     # Main Python script for the scraper
├── .env                   # Stores APIFY_TOKEN and ACTOR_ID (you need to create this)
├── requirements.txt       # Lists the required Python packages
└── README.md              # Project documentation
```

---

## 🛠️ Setup & Installation

### 1. Clone this repository
```text
git clone https://github.com/MOHAMMEDFAISALSM/indeed_scrape_using_apify.git

cd indeed_scrape_using_apify
```
### 2. Install dependencies
```text
pip install -r requirements.txt
```
### 3. Get your Apify API Token & Actor ID
- Go to [Apify Indeed Scraper](https://apify.com/misceres/indeed-scraper)  
- Click "**Try for free**" and sign in (new accounts get **$5 free credits**)  
- Find your **API Token** and **Actor ID** from Apify dashboard  

### 4. Update your `.env` file

Create a `.env` file in the project root (template included):  
```text
APIFY_TOKEN=your_apify_token_here

ACTOR_ID=your_actor_id_here
```

### 5. Run the scraper
```text
python indeed_scrapper.py
```
- Enter the job title you want (e.g., `Python Developer`)  
- Wait while the scraper runs  
- Results will be saved as:  

Python Developer_cleaned_jobs.xlsx


---

## 📊 Example Output

| Job Title        | Company | Location | Salary  | Job Type  | Rating | Reviews | Posted     | Apply Link      | Description          |
|------------------|---------|----------|---------|-----------|--------|---------|------------|-----------------|----------------------|
| Python Developer | XYZ Ltd | Chennai  | ₹8L-12L | Full-time | 4.2    | 123     | 2 days ago | apply_link_here | Job description text |

---

## ⚠️ Notes
- The first run may take up to **1 minute** (Apify fetches data in the background)  
- Free accounts have **limited credits** on Apify  

---

## 📧 Author
👤 **Mohammed Faisal**  
- GitHub: [MOHAN-RAJI](https://github.com/mohan-raji)  
- LinkedIn: [MOHAN-RAJI](https://www.linkedin.com/in/mohan-raji-2173a0297/)

---

## 🤝 Contributing
Contributions are welcome!  

1. Fork the repo  
2. Make your changes  
3. Submit a pull request  

Let’s build this together 🚀  
