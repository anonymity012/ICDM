# Modeling Aspect-Level Interactions with Boundary Probabilities for Targeted  Sentiment Analysis

This repo contains the code and data of the following paper:

In this paper, we design a novel span-based framework for the task of targeted sentiment analysis.
Specifically, we combine the position and semantic information to detect the boundaries of an aspect, and for sequentially connecting the sub-problems of aspect extraction and sentiment prediction, we design a distributional input strategy. And it is shown as below:

<p>
<img src="image/model.pdf" width="600">
</p>


This framework consists of two components:  
- Aspect extraction  
- Sentiment prediction

## Usage
1. Install required packages：

      Python 3.6

      [Pytorch 1.1](https://pytorch.org/)

      [Allennlp](https://allennlp.org/)

2. Download pre-train models used in the paper unzip it in the current directory

    uncased [BERT-Large](https://drive.google.com/file/d/13I0Gj7v8lYhW5Hwmp5kxm3CTlzWZuok2/view?usp=sharing) model
3. To make it easier for the reader to run our program, we have written all the parameter commands in the     
   run.py file. You can run the following commands and the results are in /result like this:

   ```  
   python run.py
   ```
## Detailed information

The range of parameter in this paper is as follows:

```
the learning rate:[1e-5,2e-5,3e-5,3e-4]
the batch size:[16,32,64,128,256]
the \tau:[0.0,0.1,0.2,0.3,0.4,0.5,0.6,0.7,0.8,0.9,0.9,1.0]
the compatibility threshold m_{s,e}:[1e-7,1e-5,1e-2,0,0.1,0.3,0.5,0.7,0.9]
the num_train_epochs:[20,30,40,50,100,200]
the span length: [1,2,3,4,5]
```

## Acknowledgements
We sincerely thank Xin Li for releasing the [datasets](https://github.com/lixin4ever/E2E-TBSA).


# ICDM2023
