# General Steps of Image Classification (with Keras)
---
#### by **Jiazhen Xi**

- Sources are in repository
- Completed visualizations/results are in url
- directory
    - input
        - dogs-vs-cats-redux-kernels-edition/[raw_data_folders]
        - dvc-prepare-evalset
    - notebook_sources
        - *.ipynb

## Prepare evaluation datasets (train/valid/test)
- **Source**: https://www.kaggle.com/johnfarrell/dvc-prepare-evalset
- KFold(small, used here)
- stratified(didn't use)
- random 5% split(large, didn't use)
## Preprocessing
- **Source**: https://www.kaggle.com/johnfarrell/dvc-preprocessing
- [keras.preprocessing.image.ImageDataGenerator][1]
## Basic CNN
- https://www.kaggle.com/johnfarrell/dvc-basic-model
- Augmentation: ImageDataGenerator
- [Simple CNN model][2] (arranged with [Model class with functional API][3])
## Pretrained Model Feature Extraction
- **Source**: https://www.kaggle.com/johnfarrell/dvc-pretrained-model-feature-extract
## Pretrained Model Fine-tune
- **Source**: https://www.kaggle.com/johnfarrell/dvc-pretrained-model-finetune
## More Tricks
- **Source**: https://www.kaggle.com/johnfarrell/dvc-advanced-model
- Custom image generator(based on image filepath)
- [Snapshot Ensemble][4] with [Cyclic Learning Rate][5]
- [Test-Time Augmentation][6]

[1]:https://keras.io/preprocessing/image/
[2]:https://blog.keras.io/building-powerful-image-classification-models-using-very-little-data.html
[3]:https://keras.io/models/about-keras-models/
[4]:https://github.com/titu1994/Snapshot-Ensembles
[5]:https://www.jeremyjordan.me/nn-learning-rate/
[6]:https://towardsdatascience.com/augmentation-for-image-classification-24ffcbc38833