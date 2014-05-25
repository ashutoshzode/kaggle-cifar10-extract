kaggle-cifar10-extract
======================

Python script for extraction of pixel data from CIFAR10 images. This will convert the images into an easily-accessible CSV file with the format:

```
"pxr0","pxg0","pxb0","pxr1","pxg1","pxb1","pxr2","pxg2","pxb2","pxr3","pxg3","pxb3",...,"class"
59,62,63,16,20,20,25,24,21,33,25,17,50,32,21,71,48,29,97,69,40,115,82,49,137,...,"horse"
...
```

Where `pxr0` is red value for pixel 0, `pxg2` is green value for pixel 2, etc.

Instructions
---

Download `train.7z` from the Kaggle site and extract it in the same directory as this repo. Then run:

```
python getpx.py > train.csv
```

Dependencies
---

This script depends on `PIL` (Python Imaging Library). You can probably install this by running this command (if you have Pip):

```
pip install PIL
```
