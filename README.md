# TREC-Microblog-Datasets
TREC Microblog 2011-2014 Datasets. More details in:

[Multi-Perspective Relevance Matching with Hierarchical ConvNets for Social Media Search](https://arxiv.org/abs/1805.08159)

## Dataset Description
- a.toks: query file, one line per query
- b.toks: document file, one line per tweet
- sim.txt: relevance judgements, 0 or 1
- url.txt: URLs contained in the tweet, one line per tweet
- id.txt: the originial run using Query Likelihood (QL), which also provides the query id, tweet id, etc.

## TREC_EVAL
```
$ tar -xvzf trec_eval.8.1.tar.gz
$ cd trec_eval.8.1
$ make
$ ./trec_eval ../data/qrels.microblog2011-2014.txt ../data/trec-2011/id.txt
```
This should return the original QL score on TREC 2011 dataset (MAP: 0.3576, P30: 0.4000).

## Reference
If you are using this dataset, please kindly cite the paper below:
```
@article{rao2018multi,
  title={Multi-Perspective Relevance Matching with Hierarchical ConvNets for Social Media Search},
  author={Rao, Jinfeng and Yang, Wei and Zhang, Yuhao and Ture, Ferhan and Lin, Jimmy},
  journal={arXiv preprint arXiv:1805.08159},
  year={2018}
}
```
