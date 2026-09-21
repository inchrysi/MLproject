# MLproject
This project builds a full machine learning pipeline on the [Online Shoppers Purchasing
Intention](https://archive.ics.uci.edu/dataset/468/online+shoppers+purchasing+intention+dataset)
dataset, split into three linked tasks:
 
1. **Regression**: recover the corrupted `Exit Rate` feature.
2. **Classification**: predict `Revenue` (whether a visitor made a purchase).
3. **Clustering**: repeat the classification task with unsupervised methods and compare
   against the best supervised model.
The dataset contains ~12,000 browsing sessions, each with behavioral (page counts,
durations, bounce/exit rate, page value), temporal (month, special day, weekend), and
categorical (operating system, browser, region, traffic type, visitor type) features. A
significant portion of the `Exit Rate` values were deliberately corrupted (set to missing) for this assignment.

## Repository Structure
 
```
.
├── README.md
├── notebook.ipynb          # Main notebook: all three tasks, end to end
├── data/
│   ├── train.csv            # Training set (Exit Rate partially missing)
│   └── test.csv              # Test set (Exit Rate partially missing)
```
## How to Run
 
1. Install dependencies:
```bash
   pip install -r requirements.txt
```
2. Open `notebook.ipynb` in Jupyter and run all cells top to bottom
   (Kernel → Restart & Run All is recommended to guarantee a clean execution).


