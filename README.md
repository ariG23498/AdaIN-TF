# AdaIN-TF
Minimal Implementation of [AdaIN](https://arxiv.org/abs/1703.06868) with TensorFlow.

## Architecture
![image](https://user-images.githubusercontent.com/36856589/121852570-4f155880-cd0d-11eb-91ee-e78eced49bfe.png)
The architecture of the model is simple, it consists of the following parts:
- Encoder: Pretrianed VGG19
- AdaIN Layer
- Decoder: The generator that produces the stylised images
- Loss_Net: Pretrained VGG19.

## Dataset
The dataset used here is taken from the Kaggle Competition [I’m Something of a Painter Myself](https://www.kaggle.com/c/gan-getting-started).
They provide preprocessed `tfrecords` for us to use TPUs for faster training. In the notebook present I have indeed used TPUs to train the model.

## Inference
![stylised_images](https://user-images.githubusercontent.com/36856589/121852788-9a2f6b80-cd0d-11eb-8975-36fcf6fc2276.png)
