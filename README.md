# Zero-Shot classification for summarization of screenplays

This repository contains the code for reproducing the results on the CSI corpus reported in the paper "Stories of love and violence: Zero-Shot interesting events classification for unsupervised TV series summarization" which is under currently under review.
In this paper, we propose an unsupervised approach to generate TV series summaries using screenplays that are composed of dialogue and scenic
textual descriptions. In the last years, the creation of large language models has enabled Zero-Shot text classification to perform effectively in some
conditions. We explore if and how such models can be used for TV series summarization by conducting experiments with varying text inputs.

Method 



Results 
The results obtained with Entail (Bart MNLI) unveils the potential of zero-shot classification for unsupervised summarization with events representative of a genre as candidate labels for crime series and soap operas. When provided with a screenplay, we were able to observe that the Entail model performs best when handling only visual information data. We think our approach is helping to push interpretability: contrary to modelling interestingness without proxies, this approach allows to justify the choice of summary scenes by their closeness to non subjective labels. Another major strength of this approach is its flexibility. 



Please cite the following if you use this code.
```
@inproceedings{reboud2021stories,
  title={Stories of love and violence: Zero-Shot interesting events classification for unsupervised TV series summarization},
  author={Reboud, Alison and Harrando, Ismail and Lisena, Pasquale and Troncy, Rapha{\"e}l},
  year={2022}
}
```



Follow the notebook [`Zero_Shot_Pipeline.ipynb`](./Zero_Shot_Pipeline.ipynb) to reproduce the experiments using named-events for screenplays summarization with BART MNLI. The notebook also contains the code for the experiment that combines zero-shot classification scores and centrality scores as computed by 

These centrality scores can found under [`centralities.npy`](./centralities.npy)

The csi corpus can be found [here](https://github.com/EdinburghNLP/csi-corpus) and should be placed under [`/coref/csi-corpus`](./coref/csi-corpus)




