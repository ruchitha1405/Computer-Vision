Hi everyone,

Just a couple points of clarification about assignment 2.
- You do not have to implement SIFT from scratch. Please use OpenCV libraries. The overall goal of this assignment is to understand how various design choices (hyperparameters) can affect classification performance.
- Similarly, please use existing libraries for Kmeans, SVM, etc. (e.g., sklearn).
- Use pytorch for the CNN question.
- The final question about the transformer - you are expected to create a simple 2 layer Transformer encoder architecture. Look at pytorch's `nn.TransformerEncoderLayer` to create 1 layer and `nn.TransformerEncoder` to create multiple (in this case 2) layers. Don't use a pre-trained ViT or so on this task, it is an overkill!

Best
Makarand