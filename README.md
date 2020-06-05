## Identify dog breeds using pre trained image classifier

## Principal Objectives:
* Correctly identify which pet images are of dogs (even if breed is misclassified) and which pet images aren't of dogs.
* Correctly classify the breed of dog, for the images that are of dogs. 
* Determine which CNN model architecture (ResNet, AlexNet, or VGG), "best" achieve the objectives 1 and 2.   
* Consider the time resources required to best achieve objectives 1 and 2, and determine if an alternative solution would have given a "good enough" result, given the amount of time each of the algorithms take to run.

## Development:
* Clone the repository: https://github.com/supreetharoger/ai-programming-identify-dog-breeds.git
* To classify uploaded images, run - sh run_models_batch_uploaded.sh
* To classify dog images, run - sh run_models_batch.sh

## Results of Classifying uploaded images
Shell script outputs the following files for 3 CNN model architecture - Resnet, Alexnet and vgg
* resnet_uploaded-images.txt - that contains the results using CNN model architecture ResNet
* alexnet_uploaded-images.txt - that contains the results using CNN model architecture AlexNet
* vgg_uploaded-images.txt - that contains the results using CNN model architecture VGG

* The three model architectures classify the breed of Dog(Dog_01.jpg) as correct breed - Golden retriever.
* The three model architectures classify the breed of dog in Dog_01.jpg to be the same breed of dog as that model architecture classified Dog_02.jpg.
* The three model architectures correctly classify Animal_Name_01.jpg and Object_Name_01.jpg as not dogs.

| Architecture | 900 | 900 |
| ------------ | --- | --- |
| Alexnet      | 75  | 100 |



