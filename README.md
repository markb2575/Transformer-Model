# Transformer-Model
Implemented two transformer models, one with both a decoder and encoder, and one with just a decoder, trained on book taken from online.

# Note
Transformers using both a decoder and encoder are more useful for cases when the prompt will be using a different vocabulary than the expected output (such as translating languages). This is due to the encoder taking the prompt and encoding it using a different token embedding table and positional encoding table before integrating with the cross-multi-head attention in the decoder. Due to my use case allowing for the same vocabulary for the input and output, the decoder-only model is better suited.
