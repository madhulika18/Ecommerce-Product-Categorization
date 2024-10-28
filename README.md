# ECOMMERCE PRODUCT CATEGORIZATION

## 1. Problem Statement:

In the rapidly evolving world of eCommerce, accurate product categorization is crucial for ensuring seamless customer experiences, reducing search friction, and increasing product discoverability. However, the sheer volume of diverse products poses a significant challenge. Current classification systems struggle to handle ambiguities, unconventional naming conventions, and multi-language data. This hackathon aims to address these challenges by inviting participants to create innovative solutions that enhance product categorization efficiency, accuracy, and scalability.

Develop a multi-class text classifier that categorizes products with maximum accuracy based on the given dataset.

## 2.	Dataset Description

Here's a detailed description for each column name:

**1. uniq_id:** 
   - Description: A unique identifier for each product.
   - Purpose: Acts as the primary key to distinguish each product record uniquely.

**2. crawl_timestamp:**
   - Description: The timestamp when the product data was last scraped or collected.
   - Purpose: Helps identify the data's recency and track changes over time.

**3. product_url:** 
   - Description: The URL linking directly to the product's page on the eCommerce platform.
   - Purpose: Allows direct access to the product's information and purchasing page.

**4. product_name:** 
   - Description: The name or title of the product as displayed on the eCommerce platform.
   - Purpose: Provides a searchable and readable identification of the product.

**5. product_category_tree:** 
   - Description: The hierarchical structure representing the product's category on the platform.
   - Purpose: Useful for categorization, analysis, and filtering of products.

**6. pid:** 
   - Description: A unique identifier specific to the eCommerce platform for each product.
   - Purpose: Used to reference products internally on the platform.

**7. retail_price:** 
   - Description: The original or retail price of the product before any discounts.
   - Purpose: Helps understand the product's standard market value.

**8. discounted_price:** 
   - Description: The price of the product after applying any discounts or offers.
   - Purpose: Reflects the final price a customer would pay.

**9. image:** 
   - Description: URL linking to the main image of the product.
   - Purpose: Provides visual representation for the product.

**10. is_FK_Advantage_product:** 
* Description: A boolean indicator (True/False) showing g if the product is part of Advantage program.
* Purpose: Denotes if the product has additional benefits like faster delivery or special quality checks.

**11. description:** 
* Description: Detailed information about the product, including features, specifications, and usage.
* Purpose: Helps customers understand the product's value proposition and unique selling points.

**12. product_rating:** 
* Description: The product's overall rating on the platform, based on customer reviews.
* Purpose: Indicates customer satisfaction and product quality.

**13. overall_rating:** 
* Description: The aggregate rating of the product across different platforms or periods.
* Purpose: Offers a comprehensive view of the product's reception.

**14. brand:**
* Description: The name of the brand or manufacturer of the product.
* Purpose: Assists in brand-based analysis and filtering.

**15. product_specifications:**
* Description: Detailed specifications of the product, often in JSON or structured format.
* Purpose: Provides technical and functional details to aid customer decision-making.


## 3.	Model Implementation 
a) **Exploratory Data Analysis:** Analyse and understand the data to identify patterns, relationships, and trends in the data by using Descriptive Statistics and Visualizations.

b) **Data Cleaning:** This might include standardization, handling the missing values and outliers in the data.

c) **Dealing with Imbalanced data:** This data set is highly imbalanced. The data should be balanced using the appropriate methods before moving onto model building.

d) **Feature Engineering:** Create new features or transform the existing features for better performance of the ML Models.

e) **Model Selection:** Choose the most appropriate model that can be used for this project.

f) **Model Training:** Split the data into train & test sets and use the train set to estimate the best model parameters.

g) **Model Validation:** Evaluate the performance of the model on data that was not used during the training process. The goal is to estimate the model's ability to generalize to new, unseen data and to identify any issues with the model, such as overfitting.


## 4.	Data Insights
Count of each category

![hackathon im1](https://github.com/user-attachments/assets/da49c76d-e8dc-4729-8227-1ba9a75e4b88)

### 4.1. Word Cloud
Word clouds are a great way to visualize the frequency of words in text data.

![wordCloud](https://github.com/user-attachments/assets/65e7d8dd-e1b6-43be-a757-4f99ed95deca)

## 5. Models Used
We have used the following 4 models:

a) Extreme Gradient Boosting

b) Random Forest Classifier

c) Extra Trees Classifier

d) Logistic Regression


## 6. Future Work
In future, this work will be extended to hyperparameter tuning for further boosting the performance of the model. The additional features based on domain knowledge and different data techniques to overcome class imbalance will also be explored. We will try to test this model on different datasets as well to see how it works on unseen data. Finally, we will focus on enhancing model interpretability to better understand the decision-making process behind predictions.

## 7. Conclusion
The project involved developing models as mentioned earlier and addressing the imbalance in the data using techniques such as SMOTE and feature scaling. The results indicated significant improvement over the baseline models in terms of accuracy, precision, and recall, demonstrating the effectiveness of our approach. However, the current study has limitations. The overall performance of the models may be influenced by data quality, data collection, data size, and modelling, so further research is necessary. Overall, this project highlights the importance of reducing class imbalance and improving model performance in predictive analytics, laying the foundation for robust and dependable applications in future research.


