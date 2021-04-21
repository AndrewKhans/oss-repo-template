# Checkpoint 1

## Tensorflow Version and Plot Pop-up
![image](https://i.gyazo.com/9591801332e2857e1809515a0db36e14.png)

# Checkpoint 2

## Classification of 15 Images

![image](https://i.gyazo.com/b2cdb50e61d244b8ee84fad4bcdf7eb4.png)


# Checkpoint 3

## 1. Classifying Iron Pants from Minecraft

### Original Image
<img src="https://i.gyazo.com/882eaa1e550b08a1535feb698f4dc5dc.png" alt="image" width="200"/>

### 28x28 Greyscale Image
<img src="https://i.gyazo.com/ab22a16773481c5505769a1bc3ed214c.png" alt="image" width="200"/>

### Classification Result
[[7.7438641e-13 2.0234550e-24 1.7068619e-15 5.1624251e-31 1.2915340e-19
  1.1437321e-22 1.1005605e-11 1.1686592e-15 1.0000000e+00 9.1719814e-09]]
Prediction:  Bag


## 2. Classifying Dwight's Pizza Shirt from Dead by Daylight

### Original Image
<img src="https://i.gyazo.com/0c1d926be2a56581ad8965233833f319.png" alt="image" width="200"/>

### 28x28 Greyscale Image
<img src="https://i.gyazo.com/eb865db854b95a4b2c0e41c70ed8cd7f.png" alt="image" width="200"/>

### Classification Result
[[5.10053635e-01 5.59813088e-05 5.46065606e-02 6.44419342e-03
  1.26873655e-02 5.20058904e-07 4.02082801e-01 7.27073370e-08
  1.40627762e-02 6.10420102e-06]]
Prediction:  T-shirt/top

## 3. Classifying Boots from League of Legends

### Original Image
<img src="https://i.gyazo.com/4fb73c5f67b5d658ae5089a24def773d.png" alt="image" width="200"/>

### 28x28 Greyscale Image
<img src="https://i.gyazo.com/596b79711feed77d234174ac81567abb.png" alt="image" width="200"/>

### Classification Result
[[7.5906985e-16 4.9073923e-25 6.7610712e-17 1.6680557e-28 8.4868269e-23
  1.7390087e-28 2.0800757e-12 1.4432891e-22 1.0000000e+00 1.6853657e-18]]
Prediction:  Bag

The model guessed 1 out of the 3 items correct. It seems like video game items (things with a cartoon style) may be harder for the model, as it was not trained on images that looked similar to these. However, I am still surprised that it was incorrect when classifying the Iron Pants, as these seem like any generic pair of pants from the dataset. It could be related to the fact that the image's resolution appears to be lower than the other images, despite the fact that it's a 28x28 image file.
