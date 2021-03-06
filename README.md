# Road-Crack-Segmentation--Keras
The project uses Unet-based improved networks to study road crack segmentation, which is based on keras.  
GCUnet is an improvement to Unet that introduces the Global Context Block in Unet.  
----  
## Requirements  
- python 3.6.8  
- tensorflow-gpu 1.8 
- Keras 2.2.4
- opencv  
- tqdm  
- numpy  
- glob  
- argparse  
- matplotlib  

## Usage  
### 1. Download dataset  
> [CRACK500, key: j54r](https://pan.baidu.com/s/1rGBMwQUSfl3iEXAVG6hO4A)  
  
### 2. Train  
  eg. `python train.py --train_images dataset/CRACK500/traincrop/ --train_annotations dataset/CRACK500/traincrop/ --epoch 100 --batch_size 32`  

### 3. Test  
  eg. `python test.py --save_weights_path 'checkpoint/'+ 'Unet/' + 'weights-099-0.1416-0.9787.h5 --vis False`  
  
## Results 
![](https://github.com/TachibanaYoshino/Road-Crack-Segmentation--Keras/blob/master/result.png)  

![](https://github.com/TachibanaYoshino/Road-Crack-Segmentation--Keras/blob/master/Unet_predict/20160222_081839_641_721.jpg)  


