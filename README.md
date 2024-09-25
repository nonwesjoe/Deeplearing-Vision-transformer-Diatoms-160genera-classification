# Data information
- Get from kaggle 
- The training and Testing dataset contain 160 diatoms genera, and about 20,000 images.
- Shot by Electron microscope.
# Model architecture
- DeepVit : paper: https://arxiv.org/abs/2103.11886
# Traning information
- ran on kaggle GPU P100 and Google Colab TPU 
- data augumentation by Random Rotation and Flip
- early stopping patience 10.
- model parameter: 162,162,278 (618.6MB)
- validation accuracy: 97.2%
# Model comparision Vison Transformer VS Cnn
- Vgg19(Cnn):<pre>
model parameter:45,879,520
val_accuracy:84.3%
</pre>
- ResNet43:(Cnn)<pre>
model parameter:21,392,288
val_accuracy:85.5%
- </pre>
- DenseNet(Cnn):<pre>
model parameter:7,201,504
val_accuracy:64.3%
</pre>
- Deep Vit(vision transformer):<pre>
model parameter:162,162,278
val_accuracy:97.2%
</pre>
