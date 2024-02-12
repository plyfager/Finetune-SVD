# SVD-Lora
Using Lora for finetuning stable video diffusion(`image-to-video` model).

## Progress
First, I'm trying to use peft for training lora.

```
python train_lora.py
```

## SVD-MV(Multi-View Generation)
| Init Image        | Before Fine-tuning |After Fine-tuning |
|---------------|-----------------------------|-----------------------------|
| ![demo](https://github.com/wangqiang9/Finetune-SVD/blob/main/data/1.jpg)    | ![ori](https://github.com/wangqiang9/Finetune-SVD/blob/main/data/1.gif)   | ![ft](https://github.com/wangqiang9/Finetune-SVD/blob/main/data/11cdaf2939502622815a10e5a35009c9%20(1).gif)|

The original dataset is ShapeNet, and the method for processing it into videos is referenced [binvox_rw](https://github.com/wangqiang9/binvox_rw). I processed 1k image-to-3D datasets and attempted to finetune the effect of reproducing SVD-MV. I am trying to add more data to train and opensource it up in the future.

## Datasets
The `train.csv` file format is as follows:
```
video path
...
```

## Start
```
pip install -r requirements.txt
```

```
python train.py
```

# Acknowledgements
* [diffusers](https://github.com/huggingface/diffusers)
* [Text-To-Video-Finetuning](https://github.com/ExponentialML/Text-To-Video-Finetuning)
