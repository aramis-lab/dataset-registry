# dataset-registry

Public dataset registry for aramis team using dvc.

## Example

Download a toy machine learning example where the goal is to classify cats and dogs:

```
$ dvc get https://github.com/aramis-lab/dataset-registry examples/classification
$ cd classification
$ ls
data.zip
$ unzip -q data.zip
$ rm -f data.zip
$ tree data --filelimit 10
data
├── train
│   ├── cats  [500 entries exceeds filelimit, not opening dir]
│   └── dogs  [500 entries exceeds filelimit, not opening dir]
└── validation
    ├── cats  [400 entries exceeds filelimit, not opening dir]
    └── dogs  [400 entries exceeds filelimit, not opening dir]
```
