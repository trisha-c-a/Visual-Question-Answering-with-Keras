# Visual Question Answering on the FloodNet Dataset

As a step towards learning more about multimodal systems, I took part in the [FloodNet Challenge @ EARTHVISION 2021](http://www.classic.grss-ieee.org/earthvision2021/challenge.html) - [Track 2](https://competitions.codalab.org/competitions/30320). 
The track involved developing a Visual Question Answering (VQA) algorithm that could effectively answer questions based on the [FloodNet Dataset](https://github.com/BinaLab/FloodNet-Challenge-EARTHVISION2021).

<p align="center">
  <img src="https://user-images.githubusercontent.com/56964258/122712736-0831e080-d282-11eb-8577-f4fc24e2a646.png" width="600" height="400" />
  <br>
  Image Credits: <a href="https://arxiv.org/abs/2012.02951">arXiv:2012.02951v1</a> 
  <br><br>
</p>


In my work, I built a simple Joint Embedding VQA-based model, taking inspiration from Akshay Chavan's [articles](https://data-science-blog.com/blog/2019/07/29/visual-question-answering-with-keras-part-1/) and [Github repository](https://github.com/Akshayc1/visual-question-answering).

For image feature extraction, I experimented with two models—VGG16 and InceptionResNetv2. For textual features, I explored the usage of RNNs and LSTMs while attempting to use self-attention.

The model gave an overall accuracy 0.4254 which could be improved by doing the following:

* Training the model for a greater number of epochs or till it converges.
* Using attention based models for image features, text features or both.
* Implementing other concatenation techniques such as Multimodal Compact Bilinear Pooling (MCBP)

The challenge was a first for me as I attempted to use the knowledge I gained from months of reading about VQA systems to finally working on implementing them. 
As a way forward, I plan to improve my understanding of language models and attention mechanisms before working on more multimodal-based projects. 

* To understand how I extracted image features take a look at [Image_Features_Extraction.ipynb](https://github.com/trisha-c-a/Visual-Question-Answering-with-Keras/blob/main/Image_Features_Extraction.ipynb)
* The code to extract textual data is available in [Text_Extraction.ipynb](https://github.com/trisha-c-a/Visual-Question-Answering-with-Keras/blob/main/Text_Extraction.ipynb)
* The complete VQA notebook is in [VQA.ipynb](https://github.com/trisha-c-a/Visual-Question-Answering-with-Keras/blob/main/VQA.ipynb)
