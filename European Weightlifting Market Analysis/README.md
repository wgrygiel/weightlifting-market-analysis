# European Weightlifting Championships Analysis (2019-2024)
## Business Case: Lift & Lead Startup

### Project Overview
***Lift & Lead*** is a specialized startup interested in opening elite training centers dedicated exclusively to weightlifting. Capitalizing on the global rise of CrossFit which heavily incorporates Olympic weightlifting techniques. The founders believe there is a prime investment opportunity in this niche market.

To validate their business hypotheses and understand the European weightlifting sector, its athletes, and performance benchmarks, this data analysis project was structured and executed in two distinct phases.

---

### Project Phases

#### **Phase 1: Historical Baseline**
* **Objective:** Establish an initial understanding of the sector using existing internal data assets.
* **Data Sources:** Accessed and structured the 2019 and 2021 databases compiled from:
  * [2019 European Weightlifting Championships (Wikipedia)](https://es.wikipedia.org/wiki/Campeonato_Europeo_de_Halterofilia_de_2019)
  * [2020 European Weightlifting Championships (Wikipedia)](https://es.wikipedia.org/wiki/Campeonato_Europeo_de_Halterofilia_de_2021)

#### **Phase 2: Data Expansion & Web Scraping**
* **Objective:** Expand the analytical timeframe from 2022 to 2024 to discover long-term trends.
* **Methodology:** Since the startup lacked this information, Python web scraping techniques were utilized to programmatically extract raw tables from the following official tournament records:
  * [2022 European Weightlifting Championships](https://es.wikipedia.org/wiki/Campeonato_Europeo_de_Halterofilia_de_2022)
  * [2023 European Weightlifting Championships](https://es.wikipedia.org/wiki/Campeonato_Europeo_de_Halterofilia_de_2023)
  * [2024 European Weightlifting Championships](https://es.wikipedia.org/wiki/Campeonato_Europeo_de_Halterofilia_de_2024)

---

### Tech Stack & Tools
* **Language:** Python
* **Libraries:** Pandas, Plotly Express, Matplotlib, BeautifulSoup / Requests (Web Scraping)
* **Environment:** Jupyter Notebook (Anaconda)

---

### Repository Structure
* `data/`: Contains the baseline CSV datasets provided for the project (**2019** and **2021**). 
* `notebook.ipynb`: Core Python script handling the end-to-end pipeline. **When executed, it automatically performs web scraping to fetch, clean, and append the data for 2022, 2023, and 2024.**
* `presentation.pptx`: Executive PowerPoint presentation tailored for ***Lift & Lead*** management with key strategic insights.

---

### Key Analytical Metrics Covered
* Evolution of the average performance (total weight lifted in kg) required to achieve a podium finish (Gold, Silver, Bronze) over the years.
* Historical performance trends grouped by country and gender over time.
* Metric validation to assist ***Lift & Lead*** in strategic market positioning across Europe.


### How to Run the Project
To replicate the full analysis and generate the complete dataset (2019-2024):
1. Clone this repository or download the files.
2. Ensure the `data/` folder contains the initial `2019` and `2021` CSV files.
3. Open `notebook.ipynb` in Jupyter Notebook.
4. Run all cells; the script will programmatically scrape Wikipedia to extract data for `2022`, `2023`, and `2024`, merge it with the baseline files, and generate the final interactive visualizations.
