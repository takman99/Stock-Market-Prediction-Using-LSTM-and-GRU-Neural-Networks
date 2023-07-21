# Stock-Market-Prediction-Using-LSTM-and-GRU-Neural-Networks
Stock Market Prediction Using LSTM and GRU Neural Networks - Research Project

The current S&P500 testing range is 400-day. To adjust the testing range, simply update the following code under each model:
training_data_len = len(dataset) - 400



The results can be downloaded using the 'pickle' library. Afterwards, the data can be unpacked using the following command:

import pickle
with open('gru_multi_400.pickle', 'rb') as f:
    loaded_variables = pickle.load(f)

# Unpack the variables
data = loaded_variables['data']
training_data_len = loaded_variables['training_data_len']
scaler = loaded_variables['scaler']
x_train = loaded_variables['x_train']
y_train = loaded_variables['y_train']
x_test = loaded_variables['x_test']
y_test = loaded_variables['y_test']
predictions = loaded_variables['predictions']
rmse = loaded_variables['rmse']
mae = loaded_variables['mae']
mape = loaded_variables['mape']
amape = loaded_variables['amape']
opt_learning_rate = loaded_variables['opt_learning_rate']
opt_epochs = loaded_variables['opt_epochs']
opt_batch_size = loaded_variables['opt_batch_size']
opt_dropout = loaded_variables['opt_dropout']
opt_activation_function = loaded_variables['opt_activation_function']
opt_optimizer = loaded_variables['opt_optimizer']
opt_neurons_1 = loaded_variables['opt_neurons_1']
opt_neurons_2 = loaded_variables['opt_neurons_2']
opt_neurons_3 = loaded_variables['opt_neurons_3']
opt_neurons_4 = loaded_variables['opt_neurons_4']
opt_l2_lambda = loaded_variables['opt_l2_lambda']



