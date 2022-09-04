# Graph Convolutional Networks for Text Classification in PyTorch

Implementation of Graph Convolutional Networks for Text Classification [1].

Tested on the 20NG/R8/R52/Ohsumed/MR data set, the code on this repository can achieve the effect of the paper.

## Benchmark

| dataset       | 20NG | R8 | R52 | Ohsumed | MR  |
|---------------|----------|------|--------|--------|--------|
| [yao8839836 (official)](https://github.com/yao8839836/text_gcn) | 0.8634    | 0.9707 | 0.9356   | 0.6836   | 0.7674   |
| [chengsen](https://github.com/chengsen/PyTorch_TextGCN)    | 0.8618     | 0.9704 | 0.9354   | 0.6827  | 0.7643  |
| [this repo](https://github.com/agusth24/PyTorch-TextGCN)    | 0.000     | 0.000 | 0.000   | 0.000  | 0.000  |

NOTE: The result of the experiment is to repeat the run 1.

Adding dataset kontan1: Multiclass classification (5 class), news in Indonesia. Accuracy: 0.000

Adding dataset kontan2: Sentiment classification, news in Indonesia. Accuracy: 0.000

## Requirements
* python==3.8.13
* fastai==2.0.15
* torch==1.10.2
* scipy==1.5.2
* pandas==1.3.5
* spacy==2.3.1
* nltk==3.7
* prettytable==1.0.0
* numpy==1.21.5
* networkx==2.6.3
* tqdm==4.62.3
* scikit_learn==1.1.2
* matplotlib==3.5.2

## Usage
1. Process the data first, run `data_processor.py`
2. Generate graph, run `build_graph.py`
3. Training model, run `trainer.py`

add -h for help on each usage command.

## References
[1] [Yao, L. , Mao, C. , & Luo, Y. . (2018). Graph convolutional networks for text classification.](https://arxiv.org/abs/1809.05679)
