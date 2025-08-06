# Matches

In the original version of track2p there are two types of output:

- A matrix (`plane#_match_mat.npy`) containing the indices of matched neurons across the session for a given plane (`#` is the index of the plane). Since matching is done from first day to last, some neurons will not be sucessfully tracked after one or a few days. In this case the matrix contains `None` values. To get neurons tracked across all days only take the rows of the matrices containing no `None` values. 

- A `track_ops.npy` object that contains the parameters used for the algorithm and some intermediate results that can be used for visualisations (e. g. registered images and ROIs etc.)

Since the original `plane#_match_mat.npy` depends on the method used for filtering cells (e. g. ROIs are re-indexed depending on if the user chooses manual curation or different versions of iscell_threshold), we decided to add outputs that are agnostic to this (e. g. using the default suite2p indices before filtering depending on `iscell.npy`). Using this makes it much easier to load data. This output is saved as `plane#_suite2p_indices.npy` (and the equivalents in `.mat` and `.csv` formats). 