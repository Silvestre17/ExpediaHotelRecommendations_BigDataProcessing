# 🏨 Expedia Hotel Recommendations: Big Data Analysis and Predictive Modeling 🚀

<p align="center">
  <img src="./img/Expedia_HomePage2016.png" alt="Expedia Hotel Recommendations Banner" width="800">
</p>

## 📝 Description

This project explores a large dataset of hotel booking data from Expedia to build a predictive model for user hotel preferences. The goal is to leverage the power of **Big Data** and **Machine Learning** techniques to better understand and anticipate which hotel clusters a user is likely to choose, based on their search history and other relevant information.

<p align="center">
    <!-- Project Links -->
    <a href="https://github.com/Silvestre17/ExpediaHotelRecommendations_BigDataProcessing/"><img src="https://img.shields.io/badge/Project_Repo-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Repo"></a>
</p>

## ✨ Objective

The key objectives of this project are to:

*   Develop a computational solution for the study and analysis of large-scale datasets.
*   Predict the clusters of hotels a user will choose based on their search history.
*   Provide insights into user behavior and hotel preferences on the Expedia platform.
*   Leverage distributed computing power for the tasks required in order to work with Big Data.

<p align="center">
    <a href="https://www.expedia.com/">
        <img src="https://img.shields.io/badge/Expedia-0073A8?style=for-the-badge&logo=expedia&logoColor=white" alt="Expedia" />
    </a>
    <a href="https://www.kaggle.com/">
        <img src="https://img.shields.io/badge/Kaggle-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white" alt="Kaggle" />
    </a>
</p>

## 🎓 Project Context

This project was undertaken as part of the **Processamento de Big Data** (*Big Data Processing*) course in the **[Licenciatura em Ciência de Dados](https://www.iscte-iul.pt/degree/code/0322/bachelor-degree-in-data-science)** at **ISCTE-IUL** during the 2022/2023 academic year (2nd Year, 2nd Semester). The focus was on applying distributed processing frameworks to handle a dataset too large for a single machine.

## 💾 Data Source

We utilized data from the Kaggle competition: [**Expedia Hotel Recommendations.**](https://www.kaggle.com/competitions/expedia-hotel-recommendations)
<br>

*   **`train.csv`**: Contains the primary dataset with booking and clickstream data.
*   **`test.csv`**: Includes test data for model evaluation.
*   **`destinations.csv`**: Provides latent features for destinations, which could enhance the model's predictive power.

<br>

## ⚙️ Technologies Used

*   **[Python](https://www.python.org/)**: The primary programming language.

<p align="center">
    <a href="https://www.python.org/">
        <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python" />
    </a>
    <a href="https://jupyter.org/">
        <img src="https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white" alt="Jupyter" />
    </a>
    <a href="https://www.pyspark.org/">
        <img src="https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white" alt="PySpark" />
    </a>
</p>

*   **[Apache Spark](https://spark.apache.org/)**: For distributed data processing and machine learning.

<p align="center">
    <a href="https://spark.apache.org/">
        <img src="https://img.shields.io/badge/Apache%20Spark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white" alt="Apache Spark" />
    </a>
</p>

*   **[Pandas](https://pandas.pydata.org/) & [NumPy](https://numpy.org/)**: For data manipulation and numerical computations.
  
<p align="center">
    <a href="https://pandas.pydata.org/">
        <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />
    </a>
    <a href="https://numpy.org/">
        <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy" />
    </a>
</p>

* **[Matplotlib](https://matplotlib.org/)** & **[Seaborn](https://seaborn.pydata.org/)**: For data visualization.

<p align="center">
    <a href="https://matplotlib.org/">
        <img src="https://img.shields.io/badge/Matplotlib-013243?style=for-the-badge&logo=matplotlib&logoColor=white" alt="Matplotlib" />
    </a>
    <a href="https://seaborn.pydata.org/">
        <img src="https://img.shields.io/badge/Seaborn-013243?style=for-the-badge&logo=seaborn&logoColor=white" alt="Seaborn" />
    </a>
</p>

*   **[MLlib](https://spark.apache.org/mllib/)**: Spark's Machine Learning Library. 

<p align="center">
    <a href="https://spark.apache.org/mllib/">
        <img src="https://img.shields.io/badge/MLlib-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white" alt="MLlib" />
    </a>
</p>

*   **[Amazon Web Services (AWS)](https://aws.amazon.com/)**: Used for cloud computing resources, particularly for running large-scale models.

<p align="center">
    <a href="https://aws.amazon.com/">
        <img src="https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazon&logoColor=white" alt="Amazon Web Services" />
    </a>
</p>

<br>

---

<br>

## 💻 Project Workflow (CRISP-DM)

1.  **Business Understanding:** 💡
    *   **Problem:** Predict which of the 100 `hotel_cluster` a user is most likely to book.
    *   **Context:** Explored the Kaggle competition rules and data dictionary to understand the problem domain.

<p align="center">
    <a href="https://www.kaggle.com/competitions/expedia-hotel-recommendations/data">
        <img src="https://img.shields.io/badge/Kaggle%20Data-20BEFF?style=for-the-badge&logo=kaggle&logoColor=white" alt="Kaggle Data" />
    </a>
</p>

2.  **Data Understanding:** 🔍
    *   Loaded and inspected the schema of the `train.csv` and `destinations.csv` files.
    *   Performed an initial EDA on a sample of the data to identify data types, distributions, and missing values.

<p align="center">
    <a href="https://spark.apache.org/docs/latest/api/python/index.html">
        <img src="https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white" alt="PySpark" />
    </a>
    <a href="https://pandas.pydata.org/">
        <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />
    </a>
    <a href="https://numpy.org/">
        <img src="https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white" alt="NumPy" />
    </a>
    <a href="https://matplotlib.org/">
        <img src="https://img.shields.io/badge/Matplotlib-013243?style=for-the-badge&logo=matplotlib&logoColor=white" alt="Matplotlib" />
    </a>
    <a href="https://seaborn.pydata.org/">
        <img src="https://img.shields.io/badge/Seaborn-013243?style=for-the-badge&logo=seaborn&logoColor=white" alt="Seaborn" />
    </a>
</p>

3.  **Data Preparation:** 🛠️
    *   **Data Cleaning:** Filtered out invalid or erroneous entries (e.g., booking dates in the future like year 2558, negative stay durations).
    *   **Data Reduction:** Sampled the dataset to create a smaller, more manageable subset (1.16 GB) for local development and prototyping before moving to the cloud.
    *   **Feature Engineering:**
        *   Extracted temporal features like year, month, and day of the week from `datetime` columns.
        *   Applied **Principal Component Analysis (PCA)** to the 149 latent features in `destinations.csv` to reduce dimensionality while retaining variance.

<p align="center">
    <a href="https://spark.apache.org/docs/latest/api/python/index.html">
        <img src="https://img.shields.io/badge/PySpark-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white" alt="PySpark" />
    </a>
    <a href="https://pandas.pydata.org/">
        <img src="https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white" alt="Pandas" />
    </a>
</p>

4.  **Modeling:** 🤖
    *   **Imbalanced Data:**
        > The `hotel_cluster` target variable is highly imbalanced. To address this, we implemented a combination of **undersampling** the majority classes and **oversampling** the minority classes to create a more balanced dataset for training the model.
    *   **Model Selection:** We chose a **Random Forest Classifier** from Spark's MLlib due to its robustness against overfitting and its effectiveness in handling complex interactions between features.

<p align="center">
    <a href="https://spark.apache.org/mllib/">
        <img src="https://img.shields.io/badge/MLlib-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white" alt="MLlib" />
    </a>
    <a href="https://spark.apache.org/docs/latest/api/python/reference/api/pyspark.ml.classification.RandomForestClassifier.html">
        <img src="https://img.shields.io/badge/Random%20Forest%20Classifier-8B0000?style=for-the-badge&logo=apachespark&logoColor=white" alt="Random Forest Classifier" />
    </a>
</p>


5.  **Evaluation & Deployment:** ✅
    *   The model's performance was evaluated, and although a live interactive dashboard was not deployed, the results were documented in the final report.

<p align="center">
    <a href="https://spark.apache.org/mllib/">
        <img src="https://img.shields.io/badge/MLlib-E25A1C?style=for-the-badge&logo=apachespark&logoColor=white" alt="MLlib" />
    </a>
</p>


## 🗺️ Datasets
* **`train.csv`:** Training data (**`4.07 Gb`**)
* **`test.csv`:** Test data (**`276.55 Mb`**)  
   * **Features:** *date_time, site_name, posa_continent, user_location_country, user_location_region, user_location_city, orig_destination_distance, user_id, is_mobile, is_package, channel, srch_ci, srch_co, srch_adults_cnt, srch_children_cnt, srch_rm_cnt, srch_destination_id, srch_destination_type_id, is_booking, cnt, hotel_continent, hotel_country, hotel_market, hotel_cluster*

* **`destinations.csv`:**  Data relating the id from each destination by latent features (**`138.16 MB`**)
   * **Features:** *srch_destination_id, d1 (feature1), d2 (feature2), d3 (feature3), d4 (feature4), d5 (feature5), d6 (feature6), d7 (feature7), d8 (feature8), d9 (feature9), d10 (feature10), d11 (feature11), d12 (feature12), d13 (feature13), d14 (feature14), d15 (feature15), d16 (feature16), d17 (feature17), d18 (feature18), d19 (feature19), d20 (feature20), d21 (feature21), d22 (feature22), d23 (feature23), d24 (feature24), d25 (feature25), d26 (feature26), d27 (feature27), d28 (feature28), d29 (feature29), d30 (feature30), d31 (feature31), d32 (feature32), d33 (feature33), d34 (feature34), d35 (feature35), d36 (feature36), d37 (feature37), d38 (feature38), d39 (feature39), d40 (feature40), d41 (feature41), d42 (feature42), d43 (feature43), d44 (feature44), d45 (feature45), d46 (feature46), d47 (feature47), d48 (feature48), d49 (feature49), d50 (feature50), d51 (feature51), d52 (feature52), d53 (feature53), d54 (feature54), d55 (feature55), d56 (feature56), d57 (feature57), d58 (feature58), d59 (feature59), d60 (feature60), d61 (feature61), d62 (feature62), d63 (feature63), d64 (feature64), d65 (feature65), d66 (feature66), d67 (feature67), d68 (feature68), d69 (feature69), d70 (feature70), d71 (feature71), d72 (feature72), d73 (feature73), d74 (feature74), d75 (feature75), d76 (feature76), d77 (feature77), d78 (feature78), d79 (feature79), d80 (feature80), d81 (feature81), d82 (feature82), d83 (feature83), d84 (feature84), d85 (feature85), d86 (feature86), d87 (feature87), d88 (feature88), d89 (feature89), d90 (feature90), d91 (feature91), d92 (feature92), d93 (feature93), d94 (feature94), d95 (feature95), d96 (feature96), d97 (feature97), d98 (feature98), d99 (feature99), d100 (feature100), d101 (feature101), d102 (feature102), d103 (feature103), d104 (feature104), d105 (feature105), d106 (feature106), d107 (feature107), d108 (feature108), d109 (feature109), d110 (feature110), d111 (feature111), d112 (feature112), d113 (feature113), d114 (feature114), d115 (feature115), d116 (feature116), d117 (feature117), d118 (feature118), d119 (feature119), d120 (feature120), d121 (feature121), d122 (feature122), d123 (feature123), d124 (feature124), d125 (feature125), d126 (feature126), d127 (feature127), d128 (feature128), d129 (feature129), d130 (feature130), d131 (feature131), d132 (feature132), d133 (feature133), d134 (feature134), d135 (feature135), d136 (feature136), d137 (feature137), d138 (feature138), d139 (feature139), d140 (feature140), d141 (feature141), d142 (feature142), d143 (feature143), d144 (feature144), d145 (feature145), d146 (feature146), d147 (feature147), d148 (feature148), d149 (feature149)*


## 🚀 How to Run the Code

This project was designed to run on a distributed computing environment like **Amazon Web Services (AWS)** due to the size of the dataset.

1.  **Environment:** The primary environment is a cloud-based cluster (e.g., **AWS EMR**) or a large instance notebook (e.g., **AWS SageMaker**).
2.  **Setup:**
    *   Upload the datasets (`train.csv`, `destinations.csv`) to a cloud storage bucket (e.g., **Amazon S3**).
    *   Configure a Spark cluster or notebook instance with sufficient memory and processing power.
    *   Use a **bootstrap script** to install necessary Python libraries (`pandas`, `numpy`, `matplotlib`, `seaborn`) on the cluster nodes.
3.  **Execution:**
    *   Open the Jupyter Notebook (`.ipynb` file).
    *   Ensure the notebook's Spark session is correctly configured to read from your S3 bucket.
    *   Run the cells sequentially to perform data loading, cleaning, feature engineering, and model training.

## 👥 Team Members

*   **André Silvestre** (Nº104532)
*   **Rita Matos** (Nº104936)

## 🇵🇹 Note

This project was developed using Portuguese from Portugal 🇵🇹.