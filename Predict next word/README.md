
### Next Word Prediction 
is the task of predicting what word comes next based on the previous word. It is one of the fundamental tasks of NLP and has many applications.

### Model
The model is based on Markov’s model. The main concept of Markov’s model is the next state depends only on the current state 
so s(t) depends only on s(t-1), where s(t) is the state at time t. 
This is called the first-order Markov model. 
In general, if the current state of a system depends on n previous states, then it is called n-th order Markov model. 
The model I used here is the first-order Markov model, which means I am predicting the next word based only on the previous word.
