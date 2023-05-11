# ubuntu-dataset-creator-py3
Creating Ubuntu Dialogue Corpus v2.0 with python 3


Original code for python 2 is [here](https://github.com/rkadlec/ubuntu-ranking-dataset-creator/tree/master)  
This code is work on python 3 with multiprocessing.

## Run command:
```
bash ./src/generate.sh
```

## Arguments:
* `--data_root`: directory where 1on1 dialogs will downloaded and extracted, the data will be downloaded from cs.mcgill.ca/~jpineau/datasets/ubuntu-corpus-1.0/ubuntu_dialogs.tgz (default = '.')
* `--seed`: seed for random number generator (default = 1234)
* `-o`, `--output`: output file for writing to csv (default = None)
* `-t`, `--tokenize`: tokenize the output (`nltk.word_tokenize`)
* `-s`, `--stem`: stem the output (`nltk.stem.SnowballStemmer`) - applied only when -t flag is present
* `-l`, `--lemmatize`: lemmatize the output (`nltk.stem.WorldNetLemmatizer`) - applied only when -t flag is present
