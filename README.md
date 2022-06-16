# transformer-poet [WIP]

<a href="https://colab.research.google.com/github/domschl/transformer-poet/blob/main/transformer_poet.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
[![License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](LICENSE)

Character based transformer model for text generation. Uses [ml-indie-tools](https://github.com/domschl/ml-indie-tools) to run locally on M1-Mac, Nvidia ore remotely on Colab with single code-base.

## History

* 2022-06-16: Tests with autoencoder-like bottlenecks in multi-head attention: in the middle of the layer-stack, decrease attention-units and increase attention-heads.
* 2022-01-13: Project split from [LSTM-version tensor-poet](https://github.com/domschl/tensor-poet). Further project-siblings are [torch-poet](https://github.com/domschl/torch-poet), implementing char-based text generation with pytorch  and [syncognite rnnreader](https://github.com/domschl/syncognite/tree/master/rnnreader), implementing char-based text generation completely from scratch with c++.
