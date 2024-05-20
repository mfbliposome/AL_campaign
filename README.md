# AL_step
This repo is for archive AL rounds for image analysis and model construction

### Dispense_volume folder
- In this folder, data are ordered by the data of creation. For example, 'dispense_df_20240416.xlsx' is the initial random experiments, 'dispense_df_20240429.xlsx' and 'dispense_df_20240513.xlsx' are sequential active learning rounds...etc.

### Data_model folder
- In subfolder 'Data_model_LogScale', including the direct input data set for each training AL iteations. Note, the concentration of each amphiphiles are transformed by using logarithm (log1p, natural logarithm of one plus the input array). e.g.'df_input_20240429.csv' is the data set for first AL round, 'df_input_20240510.csv' is the data set for second AL round...etc.
- In subfolder 'Update_datapool', 'df_input_update_20240511.csv' is the updated data pool combining initial random experiments and subsequent AL round...etc. 'df_input_update_OriginalScale_20240520.csv' is the updated data pool wiht original scale data
- In subfolder 'Data_model_OriginalScale', including data pool combining initial random experiments and subsequent AL rounds and the concentration of each amphiphiles are in original scale.

### Model folder
- This folder archive the training models in AL rounds. For example, 'model_20240429.pkl' is the trained model based on initial random data pool, 'GPC_model_20240513.pkl' is the trained model based on updated data pool (initial random data pool + first round AL data pool)...etc
