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

Outcome of classification
* The three model architectures classify the breed of Dog(Dog_01.jpg) as correct breed - Golden retriever.
* The three model architectures classify the breed of dog in Dog_01.jpg to be the same breed of dog as that model architecture classified Dog_02.jpg.
* The three model architectures correctly classify Animal_Name_01.jpg and Object_Name_01.jpg as not dogs.

Results Table

| # Total Images     | 4 |
| ------------------ | - |
| # Dog Images       | 2 |
| # Not-a-Dog Images | 2 |

| CNN Model Architecture | % Not a dog correct | % Dogs correct | % Breeds correct | % Match Labels |
| ---------------------- | ------------------- | -------------- | ---------------- | -------------- |
| Alexnet                |        100.0 %      |      100.0 %   |       100.0 %    |      75.0 %    |
| Resnet                 |        100.0 %      |      100.0 %   |       100.0 %    |     100.0 %    |
| VGG                    |        100.0 %      |      100.0 %   |       100.0 %    |     100.0 %    |

Resnet architecture is best at classsifying uploaded images considering percentage match and runtime performance

## Final results of classifying Dogs

Results Table

| # Total Images     | 40 |
| ------------------ | -- |
| # Dog Images       | 30 |
| # Not-a-Dog Images | 10 |

| CNN Model Architecture | % Not a dog correct | % Dogs correct | % Breeds correct | % Match Labels |
| ---------------------- | ------------------- | -------------- | ---------------- | -------------- |
| Alexnet                |        100.0 %      |      100.0 %   |        50.0 %    |      52.5 %    |
| Resnet                 |         90.0 %      |      100.0 %   |        56.6 %    |      57.5 %    |
| VGG                    |        100.0 %      |      100.0 %   |        60.0 %    |      62.5 %    |

In this project there are 2 main objectives:
* Identifying which pet images are of dogs and which pet images aren't of dogs - VGG and Alexnet correctly identify the images of "dog" and "not-dogs" 100% of the time
* Classifying the breeds of dogs, for the images that are of dogs - VGG provides better solution than other architectures because it classifies the correct breed of dog over 60% of the time.

Based on results, the "best" model architecture is VGG. VGG is able to classify "dogs" and "not-dogs" with 100% accuracy and classifies correct breed of dog with 60% accuracy.
