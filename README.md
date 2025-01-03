# 🚖 Social Media Data Analysis for Ola Cabs

Welcome to **Social Media Data Analysis for Ola Cabs** by [**Aditya Singh Yadav**](https://github.com/aditya-mnnit)!  
This repository contains a comprehensive end-to-end workflow for collecting, cleaning, analyzing, and visualizing social media data related to Ola Cabs. Our goal is to extract key insights about customer sentiment, engagement, and service improvements.

[![GitHub Repo stars](https://img.shields.io/github/stars/aditya-mnnit/OLA?style=social)](https://github.com/aditya-mnnit/OLA/stargazers)
[![LinkedIn Badge](https://img.shields.io/badge/Connect%20on-LinkedIn-blue)](https://www.linkedin.com/in/aadiitya/)
[![GitHub Badge](https://img.shields.io/badge/GitHub-aditya--mnnit-181717?logo=github)](https://github.com/aditya-mnnit)

---

## 🌟 Overview

- **Data Source**: Social media posts, primarily tweets, stored in `ola.json`.  
- **Tasks**:
  1. Data Cleaning & Preparation  
  2. Descriptive Analysis  
  3. Sentiment Analysis  
  4. Extracting & Categorizing Complaints  
  5. Engagement Analysis  
  6. Recommendations  

Whether you want to investigate customer feedback or study brand engagement, this project illustrates how to transform raw JSON data into actionable insights.

---

## 🏗️ Project Structure

```
.
├── data
│   └── ola.json               # Sample JSON dataset of social media posts
├── notebooks
│   └── OlaCabs_Analysis.ipynb # Jupyter Notebook with the entire workflow
├── output
│   └── ola_cleaned.csv        # Example of cleaned data (if you export it)
├── README.md                  # This file
└── requirements.txt           # Python dependencies (optional)
```

- **data/ola.json**  
  Contains sample social media posts about Ola Cabs.

- **notebooks/OlaCabs_Analysis.ipynb**  
  The main notebook that walks through:
  1. Data cleaning and preparation  
  2. Descriptive and statistical analysis  
  3. Sentiment analysis with TextBlob (or VADER)  
  4. Complaint categorization (driver issues, booking cancellations, etc.)  
  5. Engagement correlation and source-based patterns  
  6. Final recommendations  

- **output/ola_cleaned.csv**  
  An example CSV file with cleaned data (if you choose to export your results).

---

## 📋 Requirements

- Python 3.x  
- [pandas](https://pandas.pydata.org/)  
- [numpy](https://numpy.org/)  
- [matplotlib](https://matplotlib.org/)  
- [seaborn](https://seaborn.pydata.org/)  
- [textblob](https://textblob.readthedocs.io/en/dev/) (or [vaderSentiment](https://github.com/cjhutto/vaderSentiment) for sentiment analysis)  

You can install them via:

```bash
pip install pandas numpy matplotlib seaborn textblob
```

---

## ⚙️ Setup & Installation

1. **Clone the repository**  
   ```bash
   git clone https://github.com/aditya-mnnit/OLA.git
   ```
   or download the ZIP file from the [GitHub repo](https://github.com/aditya-mnnit/OLA).

2. **Navigate to the project folder**  
   ```bash
   cd OLA
   ```

3. **(Optional) Create & activate a virtual environment**  
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Linux/Mac
   venv\Scripts\activate     # On Windows
   ```

4. **Install dependencies**  
   ```bash
   pip install -r requirements.txt
   ```
   Or if `requirements.txt` is not provided, install them individually:
   ```bash
   pip install pandas numpy matplotlib seaborn textblob
   ```

5. **Run the Jupyter Notebook**  
   ```bash
   jupyter notebook notebooks/OlaCabs_Analysis.ipynb
   ```
   Then open it in your browser and run the cells.

---

## 🚀 Usage

1. **Data Cleaning**: Convert JSON to a Pandas DataFrame, handle missing values, and convert columns to appropriate types.  
2. **Descriptive Analysis**: Generate basic statistics (mean, median, mode) for engagement metrics and identify top posts by engagement.  
3. **Sentiment Analysis**: Use TextBlob (or VADER) to categorize each post into Positive, Negative, or Neutral.  
4. **Complaints Extraction**: Filter text for driver issues, booking cancellations, or customer service problems and visualize them.  
5. **Engagement Analysis**: Correlate followers with likes, shares, and comments. Analyze engagement by different social media sources.  
6. **Recommendations**: Summarize key findings and propose actionable steps for Ola Cabs to improve customer experience and brand engagement.

---

## 📊 Example Visualizations

<img src="https://user-images.githubusercontent.com/placeholder-123456/analysis-chart.png" alt="Sample Chart" width="600" />

<details>
<summary>Engagement By Source</summary>

```python
engagement_by_source = df.groupby('source')['total_engagement'].mean()
engagement_by_source.plot(kind='bar', color='skyblue')
plt.title("Average Engagement by Source")
plt.show()
```
</details>

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!  
Feel free to check [issues page](https://github.com/aditya-mnnit/OLA/issues) if you want to contribute.

---

## 📜 License

This project is under the **MIT License** - see the [LICENSE](LICENSE) file for details.

---

## 👋 About the Author

**Aditya Singh Yadav**  
- GitHub: [@aditya-mnnit](https://github.com/aditya-mnnit)  
- LinkedIn: [Aditya Singh Yadav](https://www.linkedin.com/in/aadiitya)

If you find this project useful, please ⭐ star the repository to show your support and follow me on [GitHub](https://github.com/aditya-mnnit) and [LinkedIn](https://www.linkedin.com/in/aadiitya/) for more projects and updates.

---

**Happy Coding!** 🚀
