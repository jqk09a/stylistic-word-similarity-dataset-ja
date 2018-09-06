# Stylistic Word Similarity Dataset (Japanese)
Our paper titled "Unsupervised Learning of Style-sensitive Word Vectors" introduced a novel task to predict lexical stylistic similarity for evaluation of word embeddings and created a benchmark dataset for this task.
The project page for this work is [here](https://jqk09a.github.io/style-sensitive-word-vectors/).

This repository contains the benchmark dataset in Japanese, that is *Stylistic Word Similarity Dataset*.

## Dataset
Stylistic Word Similarity Dataset includes 399 word pairs with human judgments on the stylistic similarity between word pairs. In the dataset, each element has:
- `word/pos 1,2`: the word a pair with POS tag
- `human (mean)`: average of the similarity scores by 15 annotators
- `ann 1~15`: the similarity score by each annotator


<!-- | word/pos 1 | word/pos 2 | human (mean) | ann 1 | ... | ann 15 |
| --- | --- | --- | --- | --- | --- |
| よー/文末 | テメェ/名詞 | -1.07 | -2 | ... | 0 |
| いやぁ/感動詞 | だからね/文末 | 1.00 | 1 | ... | 2 |
| ... | | | | | | | -->

We constructed the dataset by performing the following two steps:
1. Collected only style-sensitive words and made the word pairs
1. Rated each of the pairs on five scales <br>
(`-2`: The style of the pair is different ~ `+2` :The style of the pair is similar)

Our paper provides the more detailed description about dataset construction and analysis.



## Reference
If you use anything in this repository, please cite:

Reina Akama, Kento Watanabe, Sho Yokoi, Sosuke Kobayashi and Kentaro Inui. **Unsupervised Learning of Style-sensitive Word Vectors.** Proceedings of *the 56th Annual Meeting of the Association for Computational Linguistics*, July. 2018.

```
@InProceedings{akama2018stylevec,
  title={Unsupervised Learning of Style-sensitive Word Vectors},
  author={Reina Akama and Kento Watanabe and Sho Yokoi and Sosuke Kobayashi and Kentaro Inui},
  booktitle={Proceedings of the 56th Annual Meeting of the Association for Computational Linguistics},
  year={2018}
}
```
