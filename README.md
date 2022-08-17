# Sign-Language-Prediction

## Description of the Sign-Language (American Sign Language)

Sign languages are languages that use the visual-manual modality to convey meaning. Sign languages are expressed through manual articulations in combination with non-manual elements. Sign languages are full-fledged natural languages with their own grammar and lexicon.

American Sign Language (ASL) is a complete, natural language that has the same linguistic properties as spoken languages, with grammar that differs from English. ASL is expressed by movements of the hands and face. It is the primary language of many North Americans who are deaf and hard of hearing, and is used by many hearing people as well. The dataset format is patterned to match closely with the classic MNIST. Each training and test case represents a label (0-25) as a one-to-one map for each alphabetic letter A-Z (and no cases for 9=J or 25=Z because of gesture motions). The training data (27,455 cases) and test data (7172 cases) are approximately half the size of the standard MNIST but otherwise similar with a header row of label, pixel1,pixel2….pixel784 which represent a single 28x28 pixel image with grayscale values between 0-255. The original hand gesture image data represented multiple users repeating the gesture against different backgrounds. The Sign Language MNIST data came from greatly extending the small number (1704) of the color images included as not cropped around the hand region of interest. To create new data, an image pipeline was used based on ImageMagick and included cropping to hands-only, gray-scaling, resizing, and then creating at least 50+ variations to enlarge the quantity.

![amer_sign2](https://user-images.githubusercontent.com/84712492/179519407-ae85400b-7368-4fcb-87ac-25158a0517f8.png)

For this project, I took dataset from kaggle and predicted the outcomes using Convolution Neural Networks (CNN).This dataset section contains two csv files, training set ("sign_mnist_train.csv") and test set ("sign_mnist_test.csv")

### Convolutional Neural network (CNN)

##### Convolutional Layer : detect features from images
##### Non-Linearity Layer :  adding non-linearity to the model
##### Pooling Layer : reduce the spatial size of the input image, so that number of computations in the network are reduced
##### Flattening Layer : convert all the resultant 2-Dimensional arrays from pooled feature maps into a single long continuous linear vector
##### Fully-Connected Layer :  simply, feed forward neural networks
