# Special Tokens

Special tokens are specific placeholders or markers that help the model perform various tasks and handle specific tasks or instructions within the text. They are like signposts or markers that help the model understand the structure and context of the input text, and guide its behavior in various tasks. This ensures the output of the tokenization is in a format that your model of choice will understand.

## CLS and SEP (classification and separator)
The CLS tag is a classification tag. An Sep stands for separator. These special tokens are commonly used in tasks like text classification and sentence pair classification. In a typical scenario, you might have a sentence or text passage and you want the model to classify it into a category or determine its relationship with another sentence. The CLS token is usually placed at the beginning of the input, and the Sep token is used to separate different segments of text.

* Used in classification and sentence pair classification task
* CLS - place at the beginning of the input
* SEP - use to separate different segments of text

Example:
\[CLS\] Fine tuning is fun for all! \[SEP\]

## Mask Token
Used in task related to masked language modelling or text generation with a blank to fill in

Elample:
Fine tuning is \[MASK\] for all!

## Task specific token
you may need costume special tokens like \[SOURCE\] and \[TARGET\] to help guide the model's behaviour during traslation

## Special token for padding and truncation
when multiple sentences off varying lengths are fed into the model , special tokens for padding may be needed

padding - adding extra tokens to make all inputs the same length
truncation - shortening longer inputs to spesific length