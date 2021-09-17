# Translator ( English To Hindi )
![Keras](https://img.shields.io/badge/Keras-%23D00000.svg?style=for-the-badge&logo=Keras&logoColor=white) ![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white) ![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white) ![TensorFlow](https://img.shields.io/badge/TensorFlow-%23FF6F00.svg?style=for-the-badge&logo=TensorFlow&logoColor=white)

**Encoder-Decoder Model On The Surface**

- **Encoder:** The purpose of an encoder is to absorb the information present in the input sentence and encode this information into an lower dimentional feature rich coding, hence the name Encoder.

- **Decoder:** Similarly, for the decoder, its job is to learn how to use the information that was provided to it by the encoder to convert it into another language sentence having the same meaning as the sentence/text that was provided to the encoder.

## Diving Deep Into The Model
<br>
<img src = "https://miro.medium.com/max/875/1*lf4C7Z3TJk1V9gUPb3ao0w.png" height="350px">
<br>

<br>

### Main Layers


- **Embedding layer** : This layer creates a high-dimensional space in which each token is mapped to, e.g. let's assume `<sos>` has token `2` the output of the embedding layer will be a vector of shape `(1, embedding-dimension)`, now the embeddings for each token are optimised during training, another advantage of embeddings is that it is not discrete but vectorized thus, the model might learn `great` and `est` as different words during training but it will be able to understand `greatest` during predicting.

	![Embedding Layer](https://miro.medium.com/max/2000/1*sXNXYfAqfLUeiDXPCo130w.png "Embedding Layer")

<br>

- **LSTM Layer** : Long Short-Term Memory Network or LSTM, is a variation of a recurrent neural network (RNN) that is quite effective in predicting the long sequences of data like sentences and stock prices over a period of time. It differs from a normal feedforward network because there is a feedback loop in its architecture. It also includes a special unit known as a memory cell to withhold the past information for a longer time for making an effective prediction.

	<img src = "https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fcdn-images-1.medium.com%2Fmax%2F1000%2F1*Ht2-sUJHi65wDwnR276k3A.png&f=1&nofb=1" height="300px">

## Training and Results

Traing Loop and other code can be found in notebook, for detailed explanation visit this [Medium Article](https://medium.com/analytics-vidhya/neural-machine-translations-implementing-encoder-decoder-658c3facd530 "Medium Article").

![Results](https://miro.medium.com/max/875/1*WVBJTVIZS_YwQR1bBS1O0A.png "Results")



