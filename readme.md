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
- https://www.kaggle.com/johnfarrell/dvc-prepare-evalset
- KFold(small, used here)
- stratified(didn't use)
- random 5% split(large, didn't use)
## Preprocessing
- https://www.kaggle.com/johnfarrell/dvc-preprocessing
- [keras.preprocessing.image.ImageDataGenerator][1]
## Basic CNN
- https://www.kaggle.com/johnfarrell/dvc-basic-model
- Augmentation: ImageDataGenerator
- [Simple CNN model][2]
## Pretrained Model Feature Extraction
- https://www.kaggle.com/johnfarrell/dvc-pretrained-model-feature-extract
## Pretrained Model Fine-tune
- https://www.kaggle.com/johnfarrell/dvc-pretrained-model-finetune
## More Tricks
- https://www.kaggle.com/johnfarrell/dvc-advanced-model
- Custom image generator(based on image filepath)
- [Snapshot Ensemble][3] with [Cyclic Learning Rate][4]
- [Test-Time Augmentation][5]

[1]:https://keras.io/preprocessing/image/
[2]:https://blog.keras.io/building-powerful-image-classification-models-using-very-little-data.html
[3]:https://github.com/titu1994/Snapshot-Ensembles
[4]:https://www.jeremyjordan.me/nn-learning-rate/
[5]:https://towardsdatascience.com/augmentation-for-image-classification-24ffcbc38833