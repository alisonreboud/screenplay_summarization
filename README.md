# Zero-Shot classification for summarization of screenplays

This repository contains the code for reproducing the results on the CSI corpus reported in the paper "Stories of love and violence: Zero-Shot interesting events classification for unsupervised TV series summarization" which is under currently under review.

Please cite the following if you use this code.
```
@inproceedings{reboud2021stories,
  title={Stories of love and violence: Zero-Shot interesting events classification for unsupervised TV series summarization},
  author={Reboud, Alison and Harrando, Ismail and Lisena, Pasquale and Troncy, Rapha{\"e}l},
  year={2022}
}
```



Follow the notebook`Zero_Shot_Pipeline.ipynb`](./Zero_Shot_Pipeline.ipynb) to reproduce the experiments using named-events for screenplays summarization with BART MNLI. The notebook also contains the code for the experiment that combines zero-shot classification scores and centrality scores as computed by 

These centrality scores can found under [`centralities.npy`](./centralities.npy)

The csi corpus can be found [here](https://github.com/EdinburghNLP/csi-corpus) and should be placed under [`/coref/csi-corpus`](./coref/csi-corpus)




