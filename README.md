# AL_step
This repo is for archive AL rounds for image analysis and model construction

### Dispense_volume folder
- In this folder, data are ordered by the data of creation. For example, 'dispense_df_20240416.xlsx' is the initial random experiments, 'dispense_df_20240429.xlsx' and 'dispense_df_20240513.xlsx' are sequential active learning rounds.

### Data_model folder
- This folder include the direct input data set for training AL models. Note, the concentration of each amphiphiles are transformed by using logarithm (log1p, natural logarithm of one plus the input array)
- 'df_input_20240429.csv' is the data set for first AL round, 'df_input_20240510.csv' is the data set for second AL round...etc.  
