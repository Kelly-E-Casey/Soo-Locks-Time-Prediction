# Using Machine Learning to predict the time a ship spends in the Soo Locks
Note: The data required to run this project are publicly available at the University of Michigan's Deep Blue Data website. Because it is multiple gb in size, it is not included in this file, and must be downloaded separately.

Python packages required:
- pandas
- numpy
- seaborn
- scikit-learn
- matplotlib

## Instructions: 
1. Download transponder data
   - Go to the Deep Blue Data website to download ship transponder data (https://deepblue.lib.umich.edu/data/concern/data_sets/3b591875f)
   - Download the trimmed csv for the year you want (Note: I used `Trimmed_NY2016_new.csv`, so to use another year, change DATA_PATH in the configuration section of `01_data_cleaning.ipynb` to match the selected year)
   - Move the csv into this repo
2. Create a cleaned csv with only the required data
   - Run all cells in `01_data_cleaning.ipynb`
3. Run the ML models
   - Run all cells in `02_modeling.ipynb`
   - Compare results of various ML models near the end
   - Each row shows that model's RMSE (in minutes) 

### License:
- Data is from University of Michigan's Deep Blue Data project.
- Data author: Sugrue, Dennis P.
- Data source: https://deepblue.lib.umich.edu/data/concern/data_sets/3b591875f
- License: CC BY-NC 4.0 - https://creativecommons.org/licenses/by-nc/4.0/
