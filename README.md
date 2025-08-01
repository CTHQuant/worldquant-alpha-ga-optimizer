# WorldQuant Alpha Factor Generator using Genetic Algorithm  

This project implements a genetic algorithm (GA) framework to automatically generate and optimize Alpha factor expressions for the WorldQuant Brain platform. By combining structured templates and expression components, it enables large-scale strategy exploration and simulation-based filtering.  

---

## Project Objective  

- Automatically generate large volumes of candidate Alpha expressions based on predefined templates and variable spaces.
  
- Submit each Alpha to WorldQuant's simulate API for backtesting performance (Sharpe, Fitness, Margin, etc.).  

- Score, rank, and filter expressions based on performance and constraints (e.g., turnover).  

- Store top-performing Alphas in a local database for further refinement or ensemble.  

---

## Project Structure  


| Notebook                    | Description                                                | 
|-----------------------------|------------------------------------------------------------|
| `WorldQuant_template.ipynb` | Template definitions and randomized Alpha generation       |
| `WorldQuant_simulate.ipynb` | Simulate Alpha expressions and collect performance scores  |
| `WorldQuant_web_crawler.ipynb` | Scrape detailed results from simulate results pages     | 

---

## Results  
- 2025 WorldQunat IQC
  - World: 19th worldwide out of 73,200+ participants
  - Taiwan: 2nd among 1,100+ local competitors
  - ![IQC 排名證明](https://raw.githubusercontent.com/CTHQuant/projects/main/assets/iqc_ranking.png)
    
- Over 5,000 Alphas generated and scored automatically  

- Multiple strategies achieved Sharpe > 2.0 and Margin > 15‰  

- Automatic filtering of illegal expressions (e.g., excessive turnover, empty result)  

- Final output includes:  
  - Expression ranking table (CSV or Markdown)  
  - Alpha details and IS summary reports  
  - Best-in-class candidates for submission  

---

## Requirements  

- Python 3.9+
- Dependencies:
  ```bash
  pip install pandas, json, os, random, requests, beautifulsoup4, datetime
- Jupyter Notebook environment

## Future Work  

- Extend data space to include sentiment and fundamental metrics  

- Deploy GA optimization as an API service  

---

## Author

莊宗瀚 (Tsung Han Chuang)  
[GitHub](https://github.com/CTHQuant) ｜ [LinkedIn](https://linkedin.com/in/宗瀚-莊-1a8588358/)

---

## License  

This project is for academic and demonstration purposes only. Not financial advice.  
  
