# Autoencoder Simple

Autoencoder más simple posible utilizando las imágenes de MNIST.

Lenguaje de programación: Python

Lenguaje del tutorial: Español.

## Descripción
Un autoencoder es una red neuronal artificial cuyo objetivo es aprender a copiar el input, y esta copia será el output de la red. Esta copia será útil a nuestros propósitos solo si en el proceso al red es capaz de aprender algunas características del input.

En este caso, usaremos como input imágenes de un sólo canal, las del dataset MNIST, por lo que esperamos que la red aprenda a hacer una copia de las imágenes.

El autoencoder simple consta de dos partes:
- Encoder: produce una salida h denominada code o representación latente; es la capa oculta de la red; h=f(x).
- Decoder: g(h) reconstruye la imagen a partir de la representación latente.

No sería util que el autoencoder aprenda a copiar la imágen como si fuera una función identidad. El objetivo será que la capa oculta retenga algunas de las propiedades más importantes de la imágen, idealmente sólo la cantidad de variables cercanas a su representación intrínseca. Este tipo de redes se denominan *undercomplete autoencoders* y su forma de aprender es a través de backpropagation, utilizando una función de costo o *loss* que penaliza la diferencia entre el input y el output.

En esta notebook se programo el autoencoder más simple posible utilizando Python como lenguaje de programación y PyTorch como librería para construir las redes neuronales artificiales, programando en el entorno de Jupyter notebooks. 

Se utilizaron las imagenes del conocido dataset MNIST como ejemplo; son imágenes de números escritos a mano  "en blanco y negro", es decir, poseen un solo canal de color.

## Getting Started
Al estar escrito el código en una notebook de Jupyer, es posible correrlo en alguna plataforma online:

* Google Colab: 
* Kaggle: https://www.kaggle.com/polavr/autoencoder-simple-con-mnist (presionar el botón de los 3 puntos en la parte superior derecha -> copy and edit notebook)
* Binder: [![Binder](https://mybinder.org/badge.svg)](http://mybinder.org/v2/gh/paula-rj/AutoencoderSimple/main)

O bien simplemente descargarlo y correrlo localmente.

## Referencias:
https://www.deeplearningbook.org/contents/autoencoders.html

## Version History

* 0.1
    * Initial Release
