# Confidence Estimation

## Running

Change to directory containing all the files.

`pip install -r requirements.txt`

Run `clf_model.py` to train and test several models using a grid search.

Run `read_reports.py` to get statistics about which models performed best on which metrics.

Run `filter_data.py` to produce a `.json`. The `.json` has the three best models as (0, 1, and 2) as keys, with the values being dictionaries, each with two keys. These keys are `agnostic` and `aware` for the respective splits of the training data. The values for these keys are lists of booleans. `true` means keep the corresponding example (in order) from the training data, and `false` means filter it out.
