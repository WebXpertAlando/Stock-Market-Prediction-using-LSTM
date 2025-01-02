# Stock-Market-Prediction-using-LSTM

# #Introduction to LSTMs: 

Making Stock Movement Predictions Far into the Future Long-short-term memory models are extremely powerful time-series models. They can predict an arbitrary number of steps into the future. An LSTM module (or cell) has 5 essential components, which allow it to model both long-term and short-term data. 

**Cell state (ct)** - This represents the internal memory of the cell, which stores both short-term memory and long-term memories.

**Hidden state (ht)** - This is output state information calculated w.r.t. current input, previous hidden state, and current cell input, which you eventually use to predict the future stock market prices. 

Additionally, the hidden state can decide to only retrieve short- or long-term memories or both types of memory stored in the cell state to make the next prediction. 

**Input gate (it**) - Decides how much information from current input flows to the cell state.

**Forget gate (ft)** - Decides how much information from the current input and the previous cell state flows into the current cell state. 

**Output gate (ot)** - Decides how much information from the current cell state flows into the hidden state so that if needed LSTM can only pick the long-term memories or short-term memories and long-term memories.

See the example  below:


![lstm_pic](https://github.com/user-attachments/assets/02984314-e125-43eb-89d3-861684e93dee)

