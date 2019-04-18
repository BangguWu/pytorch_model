## Model with PyTorch
I have trained model with [PyTorch](https://pytorch.org/) on the Imagenet,Places365 and so on.
## Accuracy
Model|Dataset|top1|top5
:-:|:-:|:-:|:-:
resnet50|Imagenet|76.364|93.122
senet50|Imagenet|77.264|93.612
resnet50|Places365|55.18|85.29
densenet161|Places365|-|-

## Model check
```
    python load_bestmodel.py [model_path]
```

## Test
```
    python main.py -a resnet50 -e [data-folder with train and val folders]
```
if you use places365 dataset, you should change the code of data_load, and change the number of classes