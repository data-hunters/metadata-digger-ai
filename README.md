# Metadata Digger AI

This repository is intended for storing trained models that could be used in [Metadata Digger tool](https://github.com/data-hunters/metadata-digger), POC in AI area, etc.

## Models
We provide one Multi-Class, Multi-Label model currently that could be used to recognize objects on images in Metadata Digger for further analysis. Below you can read more information about it.

### General model capable of recognizing 80 types of objects on images.

| | |
|-|-|
| **Model path** | [`zoo_models/zoo_inception_v1_based_coco.model`](https://github.com/data-hunters/metadata-digger-ai/raw/master/zoo_models/zoo_inception_v1_based_coco.model) |
| **Type/Method** | Artificial Neural Networks, Convolutional Neural Networks |
| **Format** | Analytics Zoo |
| **Type of problem** | Multi-Class, Multi-Label |
| **Training Dataset** | [COCO](http://cocodataset.org) |
| **Description** | Model focused on 80 general categories provided with [COCO (Common Objects in Context)](http://cocodataset.org) dataset: <br> oven, person, bus, fire hydrant, chair, fork, backpack, surfboard, umbrella, hot dog, bird, elephant, banana, couch, hair drier, frisbee, toilet, bicycle, clock, train, dining table, suitcase, tennis racket, toaster, bear, kite, remote, traffic light, pizza, teddy bear, bench, cup, book, car, sports ball, baseball bat, bowl, mouse, horse, zebra, spoon, bed, tie, sink, parking meter, donut, orange, scissors, truck, bottle, keyboard, motorcycle, baseball glove, sandwich, laptop, sheep, broccoli, cell phone, dog, snowboard, stop sign, refrigerator, knife, wine glass, handbag, cake, giraffe, boat, vase, potted plant, skateboard, skis, carrot, cow, airplane, toothbrush, apple, cat, microwave, tv. <br> It was prepared during one of our Proof of Concept projects. It is not very accurate however gives quite good results for images with popular scenes. Model was built on top of Inception V1 [provided with Zoo framework](https://github.com/intel-analytics/analytics-zoo/blob/v0.6.0/docs/docs/ProgrammingGuide/image-classification.md#download-link) using Transfer Learning method (freezed all layers up to `pool4/3x3_s2`). Achieved validation accuracy: 97.82%. |
| **MD Labels Mapping** | `69:oven,0:person,5:bus,10:fire hydrant,56:chair,42:fork,24:backpack,37:surfboard,25:umbrella,52:hot dog,14:bird,20:elephant,46:banana,57:couch,78:hair drier,29:frisbee,61:toilet,1:bicycle,74:clock,6:train,60:dining table,28:suitcase,38:tennis racket,70:toaster,21:bear,33:kite,65:remote,9:traffic light,53:pizza,77:teddy bear,13:bench,41:cup,73:book,2:car,32:sports ball,34:baseball bat,45:bowl,64:mouse,17:horse,22:zebra,44:spoon,59:bed,27:tie,71:sink,12:parking meter,54:donut,49:orange,76:scissors,7:truck,39:bottle,66:keyboard,3:motorcycle,35:baseball glove,48:sandwich,63:laptop,18:sheep,50:broccoli,67:cell phone,16:dog,31:snowboard,11:stop sign,72:refrigerator,43:knife,40:wine glass,26:handbag,55:cake,23:giraffe,8:boat,75:vase,58:potted plant,36:skateboard,30:skis,51:carrot,19:cow,4:airplane,79:toothbrush,47:apple,15:cat,68:microwave,62:tv` |

## Custom models

If you need more accurate models or focused on specific area (e.g. military, different types of buildings, groups of people, etc.) please contact us: contact@datahunters.ai. We can train model for you based on your dataset or prepared by us. Cost depends on many things like dataset volume, number of output labels, quality of dataset, etc. 

If you are Open Source contributor and want to build some interesing model with us, just let us know on dev@datahunters.ai!

## Licensing
Licensing of Neural Network models is unfortunately not so obvious thing. Our whole work (presented in this repository) is shipped under liberal license - Apache 2.0 but final license of model could depend also on other things:

* License of based model in case of situation when we used technique called Transfer Learning (it uses other trained model to take advantage of its "knowledge").
* License of dataset that has been used to train model

Opinions are divided but usually the most important and valid license is specified by author of model (in this case - by us, **so it will be Apache 2.0**).
<br/>
<br/>
<br/>

[![DataHunters](http://datahunters.ai/assets/images/logo_full_small.png)](http://datahunters.ai)

