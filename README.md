# MultiPEER: A Deep, Multi-Task Framework for Identifying Aspect Categories and Their Sentiments in Scientific Peer Reviews
This repository contains dataset and code of the "MultiPEER: A Deep, Multi-Task Framework for Identifying Aspect Categories and Their Sentiments in Scientific Peer Reviews" Authors: Prabhat Kumar Bharti,  Mayank Agrawal, Asif Ekbal, Affiliation: Indian Institute of Technology, Patna, India


## Download the project source folder

Can download the source code using `git clone` or the `zip file`.

## Dataset:

The dataset contains of all the annotated review sentences, SciBERT embeddings, BERT_BASE embeddings, POS one-hot-encoded data, reviews(X) and annotations and it's polarity(Y). We have also stored the embeddings to expedite the training process.

#### NOTE: Since the entire dataset sums upto 1.92 GB, we have uploaded it [HERE](https://drive.google.com/drive/folders/1LihpGHcTZPZQh14mU-YFH5vM-bSmDiQv?usp=share_link)

## Notebooks:

### 1) Our Proposed Model:

This [notebook](https://github.com/meithnav/IIT-multi-task-aspect/blob/main/notebooks/our-model.ipynb) consists our proposed multi-task model for aspect category classification and sentiment detection.

### 2) POS-SciBERT Model:

This [notebook](https://github.com/meithnav/IIT-multi-task-aspect/blob/main/notebooks/pos_scibert_multitask_model.ipynb) consists another competitve variant of our proposed model, wherein we feed <b>POS one-hot-encoded </b> and <b> SciBERT embeddings</b> parallelly.

### 3) Ablation Variants Models:

This [notebook](https://github.com/meithnav/IIT-multi-task-aspect/blob/main/notebooks/ablations.ipynb)
consists 3 variants viz, WithoutBiLSTM, WithoutAttention, WithoutBoth. In the notebook we have 3 different cells in section <b>5) Define Ablation Models</b> for initialising each variant. `Uncomment` the one that you want to reproduce and let the other two be commented.

### 4) Attention Analysis:

This [notebook](https://github.com/meithnav/IIT-multi-task-aspect/blob/main/notebooks/Attention_Analysis.ipynb) loads our proposed model and produces a sentence-wise heatmap distribution for aspect categories for 2 selected Reviews which is discussed in depth in our paper.

#### IMPORTANT POINTS BEFORE RUNNING:

a) Change the `URL PATH` accordingly before loading the dataset(pickle files) <br>
b) The 1st tab in the notebook consists all the additional dependencies required and will be downloaded on running the cell <br>
c) For `SAVE_PATH` set the URL path where you want to save the trained model <br>

Once all the setup is complete then execute `run all`.

## Libraries & Dependencies used:

  <li>TensorFlow
  <li>Keras
  <li>Hugging Face
  <li>Matplotlib, numpy, pandas, pickle
