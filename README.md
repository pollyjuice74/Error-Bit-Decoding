# Error Bit Decoding

This is a github repo for current research conducted at the UPRRP for Graph Neural Network decoders and their use in bit error correction from a transmiter and a reciever through a noisy channel.

They are our focus of study due to current algorithms for error decoding codes such as LDPC codes that use the Sum Product Algorithm for decoding which can be represented as a graph. Essentially we are trying to better the algorithm through the heuristic approach that neural networks provide.

  ## Overview

This repo contains Jupyter Notebooks and a `Journal.md` file. 

- `Journal.md` Contains To-Dos, Daily logs and Resource links.

- `DDECCT_train.ipynb` BCH 63,45 code on DDECCT model training with zero codewords containing 3 error bits. Forked repo with trained weights: https://github.com/pollyjuice74/DDECC/tree/main  

- `Transformer_Captioning.ipynb` Contains practice for incorporating Transformer architecture. 

- `BCHDecoder.ipynb` Implements a Belief Propagation decoder with trainable weights that acheives around ~0.00019 bit error rate.

- `GNNDecoder.ipynb` Implements a GNN decoder architecture's performance in a noisy end-to-end channel and trains it to ~0.012 bit error rate. 
  
- `NeuralDemapper.ipynb` Using the Sionna framework, there is an implementation of a End-to-End channel that uses a demapper/decoder Neural Network containing 3 dense layers.

- `HammingCode.ipynb` Simple implementation of Hamming Codes using numpy. 

- `quintuple_decoder.ipynb` Implements some functions for creating bit data, and a noisy channel. It then decodes them using Majority Voting System algorithm. This algorithm is compared to a 2 layer dense Neural Network that is also built in the notebook. 



# Resources

- Hyper-Graph-Network Decoders for Block Codes

https://ai.meta.com/research/publications/hyper-graph-network-decoders-for-block-codes/

- Denoising Diffusion Error Correction Code Transformer

https://github.com/yoniLc/DDECC

- Spotify PyG GNN Recomender

https://medium.com/stanford-cs224w/spotify-track-neural-recommender-system-51d266e31e16

- CS224w Machine Learning with Graphs (Stanford)

https://web.stanford.edu/class/cs224w/

- TFGNN Transformer-style multi-head attention

https://github.com/tensorflow/gnn/blob/main/tensorflow_gnn/models/multi_head_attention/README.md

- Error Correcting Transformer

https://github.com/yoniLc/ECCT

- NVlabs gnn decoder

https://github.com/NVlabs/gnn-decoder/blob/master/GNN_decoder_LDPC_5G.ipynb

- Sionna

https://github.com/NVlabs/sionna?tab=readme-ov-file

- Graph Neural Networks for Channel Decoding

https://arxiv.org/pdf/2207.14742.pdf

- LDPC Codes Overview

https://arxiv.org/ftp/arxiv/papers/2009/2009.08645.pdf

- Bayesian Reasoning and Machine Learning

http://web4.cs.ucl.ac.uk/staff/D.Barber/textbook/090310.pdf

- 5G LDPC Codes

https://webdemo.inue.uni-stuttgart.de/webdemos/08_research/5G_LDPC_Codes/index.php?id=2&action=table_of_contents

- Machine Intelligence in Decoding
of Forward Error Correction Codes

https://www.diva-portal.org/smash/get/diva2:1146212/FULLTEXT02.pdf

- GNN Decoder GH

https://github.com/NVlabs/gnn-decoder

- Optical High Data Rate (HDR)

https://public.ccsds.org/Pubs/141x11o1e2.pdf

- Sum Product Nodes

https://github.com/ilyakava/sumproduct/blob/master/sumproduct.py#L4C1-L24C40

- SPFlow

https://github.com/SPFlow/SPFlow
