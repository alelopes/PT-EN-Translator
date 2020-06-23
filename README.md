# PT-EN-Translator

This repository brings an implementation of T5 for translation in PT-EN and EN-PT tasks. We propose some changes in tokenizator and post-processing that improves the result. We are also going to share a report about our findings and we will share the weights of the trained models.

For this project, we used https://paracrawl.eu/ corpus. We trained using 5M+ data from ParaCrawl. We just did not use more data because it was taking too much time. In theory, it would improve the results.

Another important contribution of this repository is the creation of two small corpus of paracrawl containing the Google Translate En - PT-pt and Google Translate PT-pt - En translations of 128000 sentences. This costed around $300 each to train, so you can save some money if you want to compare your results with Google Translate (GT).

# Organization

Here we have code for reproducing our results (training the algorithm) and for using it. Modules and notebooks are available for testing.

# Results

Here we are going to compare the results of our algoritm with GT with the translated subset of ParaCrawl and in WMT19' Biomedical Pt-En and En-Pt tasks, comparing our results with the winning algorithm and MarianMT Implementation from https://huggingface.co/transformers/model_doc/marian.html. 

The results are available in Table 1. It is important to note that we obtain SOTA results in PT-EN translation in WMT19'. It is also important to note that our project was trained in Pt-pt and as WMT19' is Pt-br, the results will possible increase if trained in a Pt-br corpus (both direction of translation).

# Future Work

We are going to participate in the WMT'20 Biomedical challenge. If we win, a report will be shared in this project as well. We believe that the same strategy could be improved if using a PT-br corpus. For the WMT'20 biomedical challenge it would be interesting to train in a larger corpus than what you did.
