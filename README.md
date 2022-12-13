# transformer-poet

<a href="https://colab.research.google.com/github/domschl/transformer-poet/blob/main/transformer_poet.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>
[![License](http://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat)](LICENSE)

Character, ngram or word based transformer model for text generation. Uses [ml-indie-tools](https://github.com/domschl/ml-indie-tools) to run locally on M1-Mac, Nvidia or remotely on Colab with single code-base.

You can find the transformer attention implementation at the [ml-indie-project](https://github.com/domschl/ml-indie-tools/blob/42859f8036aae3455f0231fbeb1b71d982f25d14/src/ml_indie_tools/keras_custom_layers.py#L244), it's minimal and well documented and can server as base for further experimentations with transformer-like architecture.

## History

* 2022-12-13: ml-indie-tools 0.4.0 removed all recurrence and gated memory, since it didn't improve things. Work-around for M1 tensorflow 2.11 problems with ADAM and XLA (crash on train), fixed using `legacy.ADAM`.
* 2022-12-11: ml-indie-tools 0.3.17 has new RecurrentSelfAttention layer that introduces a state similar to RNNs into key matrix of the Attention.
* 2022-11-21: ml-indie-tools ngram support.
* 2022-06-16: Tests with autoencoder-like bottlenecks in multi-head attention: in the middle of the layer-stack, decrease attention-units and increase attention-heads.
* 2022-01-13: Project split from [LSTM-version tensor-poet](https://github.com/domschl/tensor-poet). Further project-siblings are [torch-poet](https://github.com/domschl/torch-poet), implementing char-based text generation with pytorch  and [syncognite rnnreader](https://github.com/domschl/syncognite/tree/master/rnnreader), implementing char-based text generation completely from scratch with c++.
