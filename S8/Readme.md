# Objective
The objective is to refactor the below models using the modern way of building data pipeline using torchtext instead of torchtext.legacy.
* Learning Phrase Representations using RNN Encoder-Decoder for Statistical Machine Translation
* Neural Machine Translation by Jointly Learning to Align and Translate

Link to above models : https://github.com/bentrevett/pytorch-seq2seq

# Implementation

The old approach was changed and the below are the functions/approaches that got changed/added in the new pipeline
1. Tokenization
2. Building Vocab
3. Collate function
4. Used Dataloaders instead of Iterators in Train, Evaluate and Test functions.

## Model Architecture

[1. Learning Phrase Representations using RNN Encoder-Decoder for Statistical Machine Translation](https://github.com/bentrevett/pytorch-seq2seq/blob/master/2%20-%20Learning%20Phrase%20Representations%20using%20RNN%20Encoder-Decoder%20for%20Statistical%20Machine%20Translation.ipynb)

This model will be based off an implementation of [Learning Phrase Representations using RNN Encoder-Decoder for Statistical Machine Translation](https://arxiv.org/abs/1406.1078), which uses GRUs.

[2. Neural Machine Translation by Jointly Learning to Align and Translate](https://github.com/bentrevett/pytorch-seq2seq/blob/master/3%20-%20Neural%20Machine%20Translation%20by%20Jointly%20Learning%20to%20Align%20and%20Translate.ipynb)

In this model we learn about attention by implementing [Neural Machine Translation by Jointly Learning to Align and Translate](https://arxiv.org/abs/1409.0473). This further allievates the information compression problem by allowing the decoder to "look back" at the input sentence by creating context vectors that are weighted sums of the encoder hidden states. The weights for this weighted sum are calculated via an attention mechanism, where the decoder learns to pay attention to the most relevant words in the input sentence.

# Link to Changed Approach:

[1. Learning Phrase Representations using RNN Encoder-Decoder for Statistical Machine Translation](https://github.com/ganeshkcs/END2/blob/master/S8/2_Learning_Phrase_Representations_using_RNN_Encoder_Decoder_for_Statistical_Machine_Translation.ipynb)

[2. Neural Machine Translation by Jointly Learning to Align and Translate](https://github.com/ganeshkcs/END2/blob/master/S8/3_Neural_Machine_Translation_by_Jointly_Learning_to_Align_and_Translate.ipynb)



