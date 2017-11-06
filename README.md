# Word2Vec

## Description

Word2Vec model for chinese word

## Dataset

[Wikimedia Backup](https://dumps.wikimedia.org/zhwiki/)

## Dependency

- CMake
- Doxygen
- OpenCC
- jieba
- jieba extra_dict : [dict](https://github.com/fxsjy/jieba/tree/master/extra_dict)

## Train

`python3 wiki_to_txt.py [DATASET].xml.bz2`
`opencc -i wiki_texts.txt -o wiki_zh_tw.txt -c s2tw.json`
`python3 segment.py`
`python3 train.py`

## Reference

[word2vec with gensim](http://zake7749.github.io/2016/08/28/word2vec-with-gensim/)
