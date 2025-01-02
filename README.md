Here's an improved and better-formatted version of your `README.md`:

---

# **How Are the Prices of Airbnb Listings in Berlin on 18 September 2018 Affected by Locations and Room Types?**  
**Author:** Felix Junious  

## **Overview**  
This project analyzes Airbnb listings in Berlin, Germany, focusing on the factors influencing the price of listings, particularly their **location** and **room type**. The analysis uses data from **18 September 2018**, providing insights into trends and patterns in pricing.  

A detailed summary of the findings can be found in [`reports/summary.ipynb`](./reports/summary.ipynb).  

---

## **Dataset Description**  
The dataset is sourced from [Inside Airbnb](https://insideairbnb.com/get-the-data/). The data used in this analysis pertains to Berlin, Germany, for **18 September 2018**, and the primary dataset utilized is `listings.csv`.  

### **Key Attributes in the Dataset:**  
- **Basic Details:**  
  - `id`, `name`, `host_id`, `host_name`  
- **Location Information:**  
  - `neighbourhood_group`, `neighbourhood`, `latitude`, `longitude`  
- **Listing Information:**  
  - `room_type`, `price`, `minimum_nights`, `availability_365`  
- **Reviews:**  
  - `number_of_reviews`, `reviews_per_month`, `last_review`, `number_of_reviews_ltm`  
- **Other Attributes:**  
  - `calculated_host_listings_count`, `license`  

### **Data Cleaning Process:**  
Before analysis, the dataset was cleaned using the **interquartile range (IQR) method** to handle outliers and ensure data quality.

---

## **Installation and Requirements**  
To run this project, you'll need:  
1. **Jupyter Notebook**: The primary tool for this analysis.  
2. **Python Libraries:**  
   - `pandas`: For data manipulation and cleaning.  
   - `matplotlib` and `seaborn`: For visualization.  

Install the dependencies using the following command:  
```bash
pip install pandas matplotlib seaborn
```

---

## **Usage Instructions**  
1. **Viewing the Summary:**  
   - Open `reports/summary.ipynb` to explore the key findings of the analysis.  

2. **Project Structure:**  
   - **`data/raw`**: Contains the raw dataset `listings.csv`.
   - **`data/cleaned`**: Contains the cleaned dataset `cleaned_listings.csv`.  
   - **`notebooks/`**: Includes Jupyter Notebooks for:  
     - **Data Cleaning**  
     - **Exploratory Data Analysis (EDA)**  
   - **`plots/`**: Stores generated visualizations.  
   - **`reports/`**: Summary and key insights (`summary.ipynb`).  

3. **How to Run:**  
   - Clone the repository:  
     ```bash
     git clone https://github.com/felixjunious/berlin-airbnb-analysis.git
     cd berlin-airbnb-analysis
     ```
   - Open the desired notebook:  
     ```bash
     jupyter notebook
     ```

---

## **Summary of Analysis**  
The analysis explores:  
- How **room type** (e.g., entire home, private room) impacts pricing.  
- The effect of **location** (geographical coordinates) on price trends.  

Key findings and visualizations are available in [`reports/summary.ipynb`](./reports/summary.ipynb).  