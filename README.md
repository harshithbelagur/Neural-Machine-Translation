# Neural Machine Translation 

## TensorFlow 2.0 implementation of the popular NLP paper by Bahdanau et al. - Neural Machine Translation by Jointly learning to Align and Translate (ICLR, 2015) 

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

PS. Will add a presentation soon for the same
