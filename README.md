# CTR Prediction through Hierarchical Attention Transformers

## Run

### Dependencies
Please check `requirements.txt` for dependent packages or run
```bash
$ pip install -r requirements.txt
```

### Preprocess dataset
1. Create following structure in the folder
```text
Code
|-- data
|   |-- raw
|   |   |-- criteoDAC (put unzipped data)
|   |   |-- avazu (put unzipped data)
|   |-- parse
|-- Code
    |-- ...
```
2. Run preprocess
```bash
$ python Code/preprocess.py [dataset] [n_buckets]
```

### Run `Code`
Run `run.sh` as an example.

## Datasets
This section introduces the datasets.
### Criteo
```
$ curl -O http://azuremlsampleexperiments.blob.core.windows.net/criteo/day_{'seq -s ',' 0 23'}.gz
```
An useful repo: https://github.com/rambler-digital-solutions/criteo-1tb-benchmark#task-and-data

### Avazu
Avazu dataset is from Kaggle: https://www.kaggle.com/c/avazu-ctr-prediction

### Frappe
Frappe: https://github.com/hexiangnan/neural_factorization_machine/tree/master/data/frappe
