

## Dataset
- Source: Kaggle – [Mall Customer Dataset]
- Raw file used: `/content/Mall_Customers.csv`


## Data Cleaning Steps
1. Checked missing values using `.isnull()` → none found.
2. Removed duplicate rows using `.drop_duplicates()`.
3. Standardized text values:
   - Converted `Gender` column to lowercase (`male`, `female`).
4. Renamed column headers into clean snake_case:
   - `CustomerID` → `customer_id`
   - `Annual Income (k$)` → `annual_income`
   - `Spending Score (1-100)` → `spending_score`
5. Converted data types:
   - `customer_id`, `age`, `annual_income`, `spending_score` → integer type
6. Saved the cleaned dataset as **`mall_customers_cleaned.csv`**


## Data Preprocessing Steps
1. **Encoding categorical values**  
   - Encoded `gender` into numeric form (`male` = 1, `female` = 0) using `LabelEncoder`.
2. **Feature Scaling (Normalization)**  
   - Scaled numeric features (`age`, `annual_income`, `spending_score`) into 0–1 range using `MinMaxScaler`.
3. (Optional) Created standardized features using `StandardScaler` (mean=0, std=1).
4. Selected features for modeling:
   - `age_scaled`, `income_scaled`, `score_scaled`, `gender_encoded`

 
 ##Final Output Files
- **/content/Mall_Customers.csv** → Original raw dataset  
- **/content/Mall_CustomersCleaningandPreprocessing.csv** → After cleaning + preprocessing  
