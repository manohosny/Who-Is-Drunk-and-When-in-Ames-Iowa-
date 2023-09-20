# Breath Alcohol Analysis in Ames

This project provides a Python script that analyzes a dataset containing breath alcohol test results in Ames. The dataset is named `breath_alcohol_ames.csv` and is expected to be located in a `datasets` directory.

## Features

- Load and inspect the breath alcohol test results data.
- Obtain counts for each year.
- Tally up the totals for each department.
- Visualize the data:
  - Count by hour and arrange by descending frequency.
  - Count by month and arrange by descending frequency.
  - Compare the mean blood alcohol levels of men and women using side-by-side boxplots.
  - Visualize the number of DUIs over time.
- Calculate the proportion of tests that would have resulted in a DUI.
- Data transformation:
  - Handle missing values in the gender column.
  - Create a mean test result variable.
  - Create date and week variables.

## Requirements

- Python 3.x
- pandas library
- matplotlib library

## Usage

1. Ensure you have the required libraries installed:

   ```bash
   pip install pandas matplotlib
   ```

2. Place the `breath_alcohol_ames.csv` dataset in a directory named `datasets`.

3. Run the script:

   ```bash
   python <script_name>.py
   ```

## TODO

- The bar plot for hourly data is not in descending frequency. This needs to be addressed for better visualization.

## Dataset Columns

- `year`: The year the test was conducted.
- `month`: The month the test was conducted.
- `day`: The day the test was conducted.
- `hour`: The hour the test was conducted.
- `location`: The department that conducted the test.
- `gender`: Gender of the individual tested.
- `Res1`: First test result.
- `Res2`: Second test result.

## Notes

- The dataset might contain missing values, especially in the gender column.
- DUI (Driving Under the Influence) is considered if either `Res1` or `Res2` is greater than 0.08.

## License

This project is open-source and available to everyone. Please make sure to reference this repository if you use it in your work or research.

---

For any issues or suggestions, please open an issue on the project's GitHub page.
