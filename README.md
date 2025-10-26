# Raw Nuclear Imaging Data
Raw intensity data for Tc-99m sulfur colloid in each section of each 16 x 8 grid from manuscript, "A Physiologically-based Model of Localized Mucociliary Clearance in the
Airways."

## Data Format
Data can be found in `GridActivity_DataFrame.csv` and is formatted as as wide format dataframe with the following columns:

* `STUDY_ID` - unique ID for each study day (total of 77)
* `LABEL` - original string used to identify study visit (*note:* numbers are not all consecutive due to drop outs)
* `PID` - unique ID for each participant (total of 52)
* `COHORT` - study group (HC=healthy control, P=parent, CF=cystic fibrosis)
* `TRT` - treatment (IS=isotonic saline, HS=hypertonic saline); only CF participants had an HS day
* `ROW` - row number on grid (1-16 from top to bottom)
* `COLUMN` - column number on grid (1-8 from left to right)
* `GRID_ID` - grid identifier (0-127 from top to bottom, left to right)
* `TIME` - time point in minutes (0-78)
* `VALUE` - intensity of nuclear image in specified grid/time point
