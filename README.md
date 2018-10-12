# NeuralChemdner
Neural Based Chemdner Task 

## Architecture

```
Dataset(file_path, tokenize=None)
input:
  file_path: .txtと.annが複数あるディレクトリのパス。
  tokenize: Word LevelやSubword Levelに分割するtokenizeを指定。Noneの場合はCharacter Levelで行う。
>>> dataset.get(batch_size=10, padding=True)
>>> [["I", " ", "a", "m", " ", "a", " ", "h", "e", "r", "o", "."] * batch_size]

>>> token2id, label2id = dataset.make_vocab(init_key=(["UNK"], []))

```
