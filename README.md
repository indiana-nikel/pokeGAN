# pokeGAN

<a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-sa/4.0/">Creative Commons Attribution-ShareAlike 4.0 International License</a>.

Original code pulled from Siraj Raval's [Pokemon_GAN](https://github.com/llSourcell/Pokemon_GAN). The full tutorial can be found on his Youtube video: [https://youtu.be/yz6dNf7X7SA](https://youtu.be/yz6dNf7X7SA)

## Overview

Over it's lifespan, Nintendo has created over 800 unique creatures for one of its flagship titles: Pokemon. Artists and developers create and re-create these pokemon during a game's development, spends large amounts of time and effort, most of which never make it. In one news article, we can see some of of the pokemon that never made it into one of the games: http://digg.com/2018/prototype-pokemon-gold-silver.  

My approach to creating pokemon from scratch did not come from drawing, rather from machine learning: generative adversarial networks (GANs). In this model, two networks are set against each other. One is trained on every one of the 800+ pokemon images (the discriminator) and the other tries to create new pokemon images (the generator). When an image is generated, the discriminator classifies the image as real or fake, and the generator updates. After many back-and-forth passes between the two, eventually some of the generated images are classified as real.


## Dependencies (pip install)
```
cv2
tensorflow( >=1.0)
scipy
numpy
```
## Usage
```
cd pokeGAN
python resize.py
python RGBA2RGB.py
python pokeGAN.py
```
