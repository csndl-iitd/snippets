# Synchronization of EEG and ET data

The notebook here contains code snippets to synchronize the eye tracking, video and EEG data.

**Required files:**
1. The raw exported file from Tobii Pro 2 glasses (livedata.json.gz)
2. (Optional) processed ET file
3. BrainVision EEG data files (.eeg, .vhdr and .vmrk)
Note that the .eeg file is too large, and not included in the repo.

**Dependencies:**

1. mne-python
2. numpy
3. pandas
4. openpyxl (for importing Excel files, see [2] above)
5. matplotlib
6. (Optional) ipywidgets (to make interactive plots work in the notebooks; if not, comment out the `%matplotlib widget` line in the first cell of the notebook)