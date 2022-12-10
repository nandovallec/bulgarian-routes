# Scalable ML Lab 2
## Alexander Yonchev
## Fernando Vallecillos Ruiz

### Possible improvements
#### Model centric approaches
There are multiple ways to achieve improvements in the model. First and foremost the lack of computational resources is significant. We tried to train the 'small' model multiple times however, we could not get GPU sessions in Google Collab even trying at different days and hours. We also tried to use Modal however, the limitations of space and not being able to import libraries inside dataclasses made it impossible. As last resort, we trained it locally. However, the big size of the input made only possible this training reducing the batch size to 2, making the process incredibely long. In this folder, there are some of the examples and checkpoints of these tries.
Besides of the lack of resources, there are some other ways to achieve an improved version. Adding more layers to the beginning or the end before hypertuning the model could achieve better results even if it could also mean some overfitting. 

#### Data Centric approaches
There are also multiple ways to improve the model based on the data. There is a lot of labelled data with audio and transcriptions since it is essential for deaf users in multituple environments. 
On the other hands, different transformations of the data are also possible as part of the preprocessing step. Transformations to increase the quality of the audio (reducing background noise, increase some frequencies, etc.).


### Refactoring
The refactoring is pretty simple. We add pickle files to zip the data in a compress form. It then can be unpickled and used for the training with the GPU.


### Interface
https://huggingface.co/spaces/nandovallec/bulgarian-route
