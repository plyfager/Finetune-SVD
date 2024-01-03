# Finetune-SVD
Fine tune stable video diffusion.

![tile](tile.gif)

## Datasets
The `train.csv` file format is as follows:
```
video path, prompt
...
```

## Start
```
pip install -r requirements.txt
```

```
python train.py
```

# Memory usage
I have used xformers and the minimum requirement is to successfully train on 80GB A100. If you have a better plan to reduce graphics memory usage, please let me know or PR. Thanks.

# Acknowledgements
* [diffusers](https://github.com/huggingface/diffusers)
* [Text-To-Video-Finetuning](https://github.com/ExponentialML/Text-To-Video-Finetuning)
