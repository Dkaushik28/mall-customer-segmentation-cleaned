## Dataset
- Source: Kaggle – [Mall Customer Dataset]([https://www.kaggle.com/datasets/kahkashanmanzoor/mall-customer-dataset](https://www.kaggle.com/datasets/vjchoudhary7/customer-segmentation-tutorial-in-python))
- File used: `/content/Mall_Customers.csv`

## Cleaning Steps Done
1. Checked missing values using `.isnull()` → none found.
2. Removed duplicate rows using `.drop_duplicates()`.
3. Standardized text values (`Gender` → male/female lowercase).
4. Renamed column headers into snake_case.
5. Fixed data types for numeric columns.

## Final Output
- Cleaned dataset: `/content/Mall_CustomersCleaningandPreprocessing.csv`
