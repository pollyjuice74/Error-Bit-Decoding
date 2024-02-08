# Error Bit Decoding

This is a github repo for current research conducted at the UPRRP for Graph Neural Network decoders and their use in bit error correction from a transmiter and a reciever through a noisy channel.

They are our focus of study due to current algorithms for error decoding codes such as LDPC codes that use the Sum Product Algorithm for decoding which can be represented as a graph. Essentially we are trying to better the algorithm through the heuristic approach that neural networks provide.

  ## Overview

This repo contains Jupyter Notebooks and a `Journal.md` file. 

- `Journal.md` Contains To-Dos, Daily logs and Resource links. 

- `BCHDecoder.ipynb` Implements a Belief Propagation decoder with trainable weights that acheives around ~0.00019 bit error rate.

- `GNNDecoder.ipynb` Implements a GNN decoder architecture's performance in a noisy end-to-end channel and trains it to ~0.012 bit error rate. 
  
- `NeuralDemapper.ipynb` Using the Sionna framework, there is an implementation of a End-to-End channel that uses a demapper/decoder Neural Network containing 3 dense layers.

- `HammingCode.ipynb` Simple implementation of Hamming Codes using numpy. 

- `quintuple_decoder.ipynb` Implements some functions for creating bit data, and a noisy channel. It then decodes them using Majority Voting System algorithm. This algorithm is compared to a 2 layer dense Neural Network that is also built in the notebook. 
