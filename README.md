# RNN
Bi-LSTM:(Bi-directional long short term memory):
Bidirectional recurrent neural networks(RNN) are really just putting two independent RNNs together. This structure allows the networks to have both backward and forward information about the sequence at every time step

Using bidirectional will run your inputs in two ways, one from past to future and one from future to past and what differs this approach from unidirectional is that in the LSTM that runs backward you preserve information from the future and using the two hidden states combined you are able in any point in time to preserve information from both past and future.


What they are suited for is a very complicated question but BiLSTMs show very good results as they can understand the context better, I will try to explain through an example.

Let's say we try to predict the next word in a sentence, on a high level what a unidirectional LSTM will see is

“The boys went to ….”

And will try to predict the next word only by this context, with bidirectional LSTM you will be able to see information further down the road for example
