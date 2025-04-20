# reproduce

shakespeare_char

```bash
cd data/shakespeare_char
python prepare.py
```

```bash
python train.py config/train_shakespeare_char.py 2>&1 | tee logs/shakespeare_char_v2.log

python sample.py --out_dir=out-shakespeare-char 2>&1 | tee logs/sample_shakespeare_char_v2.log
```

---


```bash
cd data/shakespeare
python prepare.py
```

```bash
python train.py config/train_shakespeare_bpe.py 2>&1 | tee logs/shakespeare_bpe.log

python sample.py --out_dir=out-shakespeare-bpe 2>&1 | tee logs/sample_shakespeare_bpe.log
```
