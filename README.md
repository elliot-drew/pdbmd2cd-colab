## pdbmd2cd-colab

# PDBMD2CD-colab - Predicting circular dichroism spectra from atomic coordinates using Colab

This notebook is an Colab implementation of the PDBMD2CD algorithm described here: https://academic.oup.com/nar/article/48/W1/W17/5826170

The original webserver version of this program is available here: https://pdbmd2cd.cryst.bbk.ac.uk/

We would encourage users who wish to do very large numbers of predictions (>1000 at a time) to do so using this Colab notebook or the standalone version of PDBMD2CD available here: TBC

## Usage

- Upload a zip file called "proteins.zip" containing all the PDB files of the structures you want to run predictions for.
  - Click the folder icon on the left hand side of the page
  - Right click in the panel that opens up, and click the "Upload" option
  - Browse to and select the zip file you created in the dialog that appears
- Once this file is uploaded, in the "Runtime" menu at the top of the page, click "Run all"
- A number of dependencies need to be downloaded and installed for the prediction to run - this can take a few minutes, so be patient.
- When the predictions are done, a dialog window will appear with the results in a zip file - you can open or save this to your computer.

Inside the results file are: 
- the predicted CD spectrum for each structure - if any of the PDB files you uploaded had multiple models a spectrum will have ben produced for each model.
- The average CD spectrum of all uploaded structures
- A log file containing information on the run, including the identities of any structures that failed during the prediction process
