# openbci-brainflow

This repository contains an example of integrating psychopy with brainflow to get EEG data with markers from compatible devices such as openBCI Cyton etc.

## Installation / setup

1. Install PsychoPy
2. Open PsychoPy -> Tools -> Plugin/packages manager
3. Go to the Packages tab
4. Click on the 'Open PIP terminal' button
5. At the prompt, enter `pip install brainflow` and hit enter

## Try out the code here

1. Clone or download this repository
2. Open 'test.psyexp' in PsychoPy builder
3. The code is written to work with openBCI Cyton board. If you are using a different platform, you will have to change the code accordingly:
    1. Open the 'coder' window
    2. All changes introduced to incorporate EEG data collection with brainflow are enclosed between `# BrainFlow Code ---------` comments
    3. Check the serial port for your device in Device Manager and update it
    4. Cyton board has ID 0, used in the BoardShim initialization. For other devices, you will have to update it
    5. In the `endExperiment` function, code to store the EEG data and markers as a pandas dataframe is included. For different devices, this code may have to be modified. Specifically, the `channel_names` list should be modified.