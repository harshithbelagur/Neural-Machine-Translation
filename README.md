# Neural Machine Translation 

## TensorFlow 2.0 implementation of the popular NLP paper by Bahdanau et al. - Neural Machine Translation by Jointly Learning to Align and Translate (ICLR, 2015) 

Find the paper @ https://arxiv.org/pdf/1409.0473.pdf

For detailed implementation with replicated results, use NMT_6400000 

Following are the specifications followed as per the authors: 
- AdaDelta Optimizer with epsilon = 10-6 , rho = 0.95 
- Minibatch SGD with batch_size = 80 
- Embedding Dimension = 620 
- Hidden Layer Size = 1000 
- Output Layer Size = 500 
- Weights initialization = RandomNormal with Mean = 0 and Standard Deviation = 0.001 
- Bias initialization = Zeros
- L2 Regularization

Model sizes -

Model: "encoder_4"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
embedding_8 (Embedding)      multiple                  18600000  
_________________________________________________________________
bidirectional_4 (Bidirection multiple                  9732000   
=================================================================
Total params: 28,332,000
Trainable params: 28,332,000
Non-trainable params: 0
_________________________________________________________________

Model: "decoder_4"
_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
embedding_9 (Embedding)      multiple                  18600000  
_________________________________________________________________
gru_9 (GRU)                  multiple                  10866000  
_________________________________________________________________
attention_4 (Attention)      multiple                  3003001   
_________________________________________________________________
dense_19 (Dense)             multiple                  30030000  
=================================================================
Total params: 62,499,001
Trainable params: 62,499,001
Non-trainable params: 0
_________________________________________________________________

Total number of parameters = 28,332,000 + 62,499,001
                           = **90,831,001**
                           
PS. Presentation will be uploaded soon
