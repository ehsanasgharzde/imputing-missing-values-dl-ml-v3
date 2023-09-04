Version 3 - Missing Value Imputation Using DL and ML Methods

This program is designed for imputing missing values in a dataset using deep learning (DL) and machine learning (ML) methods. It focuses on multivariate imputation techniques and normalization of the data.

## Usage

To run this program, ensure you have the following libraries installed:
- pandas
- seaborn
- matplotlib
- scikit-learn

You can install these libraries using pip or your preferred package manager.

After installing the required libraries, follow these steps:

1. Place your dataset file in the same directory as `main.py`. The dataset should be in the Excel format (`.xls`).

2. Open `main.py` and make sure the dataset file's name matches the one you placed in the directory. In this version, it should be `"clean-xls-files/AMR-and-NSH-Buoy-Data1394-Clean-Data.xls"`.

3. Run the `main.py` script.

4. The program will perform the following steps:
   - Load the dataset.
   - Slice out "DateTime Processor" and "SunDateTime" columns.
   - Normalize the dataset using Min-Max scaling.
   - Generate new date and time values.
   - Apply Linear Regression-based imputation for missing values.
   - Save the imputed dataset to a CSV file in the "multivariate-method-results" directory.

5. Once the program finishes, you'll find the imputed dataset in the "multivariate-method-results" directory with the name "AMR-and-NSH-Buoy-Data1394-normalized-mice-linear-regression.csv".

## Important Notes

- Ensure your dataset is in the specified format, or you may need to adjust the column names and file paths in the code accordingly.
- This version uses Linear Regression-based imputation for missing values. You can explore other ML techniques as needed.
- You can modify the code to suit your dataset and specific requirements.
