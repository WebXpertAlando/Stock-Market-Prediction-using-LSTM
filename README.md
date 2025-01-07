# Stock-Market-Prediction-using-LSTM

# Introduction to LSTMs: 

Making Stock Movement Predictions Far into the Future Long-short-term memory models are extremely powerful time-series models. They can predict an arbitrary number of steps into the future. An LSTM module (or cell) has 5 essential components, which allow it to model both long-term and short-term data. 

# LSTM Modeling
Long short-term memory is a type of recurrent neural network aimed at mitigating the vanishing gradient problem commonly encountered by traditional RNNs. Its relative insensitivity to gap length is its advantage over other RNNs, hidden Markov models, and other sequence learning methods.
See the example diagram  below:

![lstm_pic](https://github.com/user-attachments/assets/c3f32725-de0a-45e7-b059-7e82964d8c34)

**Cell state (ct)** - This represents the internal memory of the cell, which stores both short-term memory and long-term memories.

**Hidden state (ht)** - This is output state information calculated w.r.t. current input, previous hidden state, and current cell input, which you eventually use to predict the future stock market prices. 

Additionally, the hidden state can decide to only retrieve short- or long-term memories or both types of memory stored in the cell state to make the next prediction. 

**Input gate (it**) - Decides how much information from current input flows to the cell state.

**Forget gate (ft)** - Decides how much information from the current input and the previous cell state flows into the current cell state. 

**Output gate (ot)** - Decides how much information from the current cell state flows into the hidden state so that if needed LSTM can only pick the long-term memories or short-term memories and long-term memories.

# Data Source:

You will be using data from the following sources:

The stock Market Data is derived from [www.alaphavintage.co] Alpha Vantage Stock API.   This stock market data retrieves 20 years of historical data for the American Airlines stock. 

