# Melbourne Housing Data — Missing Values Handling

Data cleaning exercise on the Melbourne housing dataset, focused on identifying and 
handling missing (`NaN`) values using pandas.

## What this covers

- Inspecting the dataset: row count and summary statistics (`describe()`)
- Counting `NaN` values per column
- Calculating the percentage of missing values per column
- Comparing different strategies for handling missing data:
  - Dropping all rows containing any `NaN` (exploratory — not saved)
  - Dropping all columns containing any `NaN` (exploratory — not saved)
  - Dropping rows with `NaN` in the column with the *most* missing values (exploratory — not saved)
  - Dropping rows with `NaN` in the column with the *least* missing values (applied and saved to the working `df`)
- Exporting the cleaned dataset to both `.csv` and `.h5` (HDF5) formats

## Why this approach

Rather than dropping all missing data outright (which can throw away too much useful 
information), this notebook compares the trade-offs of different NaN-handling strategies 
before settling on the least aggressive one: removing rows only where the column with the 
fewest missing values has gaps.

## Files

- `melb_data.csv` — cleaned dataset (CSV format)
- `melb_data.h5` — cleaned dataset (HDF5 format)
- `notebook.ipynb` — full analysis and cleaning steps

## Tools

Python, pandas

## Dataset

Melbourne housing market dataset.
