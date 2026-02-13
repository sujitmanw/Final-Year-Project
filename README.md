Developed a lightweight deep learning architecture named Attentive-LiteSeqCNN for multi-label protein function prediction using protein sequence data. The model integrates dilated Convolutional Neural Networks (CNNs) with a multi-attention mechanism to effectively capture both short- and long-range dependencies in amino acid sequences.

Protein sequences were segmented into overlapping k-mers (k=4) and passed through an embedding layer (dimension = 64) with dropout regularization. The architecture consists of five dilated CNN blocks with varying dilation rates (1, 3, 5, 7, 9), followed by batch normalization, LeakyReLU activation, and a multi-head attention mechanism to emphasize important sequence regions.

The model was trained and evaluated on the Data2017 dataset (Biological Process and Molecular Function categories). It achieved improved Fmax and AUPR scores compared to baseline Lite-SeqCNN and other existing approaches, demonstrating better precision and recall performance while maintaining computational efficiency.

The model uses Binary Cross-Entropy loss with Adam optimizer (learning rate = 0.0005) and supports deployment on standard hardware due to its lightweight architecture.
