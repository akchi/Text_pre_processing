## Text Pre-Processing and Feature extraction

This project aims to analyse textual data. Initially it downloads a set of published papers from a given list of URLs. The papers are then pre-processed after which, a set of features are from them. These features are nothing but a numerical representation of the paper which could be used in downstream modelling tasks.

The dataset <b>Urls.pdf</b> contains 200 URLs of published papers from a popular AI conference. The features extracted from the processed documents are stored in:

<ol>
  <li><b>vocab.txt</b> : contains the unigrams and bigrams. These tokens are stored alphabetically as token_string:token:index.</li>
  <li><b>count_vectors.txt</b> : each row of the file contains the sparse representation of a particular paper. The format - paper id, token 1 index, token1 word count, token2 index, token2 word count, and so on is used respectively.</li>
</ol>

A preliminary analysis on the processed data is done and the results are stored in <b>stats.csv</b>.

Please Note : For Pyhon 2, pdfminer needs to be installed and for Python 3 pdfminer.six needs to be installed (both through pip).
