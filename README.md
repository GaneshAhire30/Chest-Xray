# Chest-Xray Project
# AI PROJECT ON PNEUMONIA CHEST X-RAY CLASSIFICATION
# BUSINESS CASE:- Based on the image data we need to predict the X-ray is normal or pneumonia. 
## INTRODUCTION :- 
* Pneumonia is a lung inflammation caused by a viral or bacterial infection that can range from mild to severe cases. This inflammation makes the patient unable to breathe enough oxygen to reach the bloodstream. It happens when an infection makes the air sacs (alveoli) in the lungs fill with fluid or pus that might affect either one or both lungs. If your doctor thinks you might have pneumonia, a chest X-ray will be performed to find the infection in the patient's lungs and how far it’s spread.
  ![image](https://github.com/user-attachments/assets/5fd1a841-9960-4e2c-be9a-bfee8a425ced)

### How can you tell pneumonia from an X-ray ?
* When interpreting the x-ray, the radiologist will look for white spots in the lungs (called infiltrates) that identify an infection. This exam will also help determine if you have any complications related to pneumonia such as abscesses or pleural effusions (fluid surrounding the lungs).

## DATA SUMMARY :- 
**The Data set is contain total 8,546 images of Pneumonia patient chest x-ray , include three class [Normal,pneumonia]**

**Classes :-**

1. NORMAL
2. PNEUMONIA

## TASK: BINARY CLASSIFICATION :-

## WE DEVICE THIS PROJECT INTO MULTIPLE STEPS :-
* Importing library
* Make subset of training,testing & validation
* Data Processing [Prepare training and testing data]
* Visualise Training Images
* Build Arcitecture
* Model Compilation
* Training
* Evaluation
* Model saving
* Prediction
* Testing
* Visualise Test Images
* Deploy model using flask framework

## LODING DATA / PREPARING DATA :-
* Make a subset of data into three parts train, test, and validation with the help of split folder library.

## DATA PROCESSING :-
**[PREPARE TRAINING, TESTING, VALIDATION DATA]**
* Training: 7546 images belonging to 2 classes.
* Validation: 500 images belonging to 2 classes.
* Testing: 500 images belonging to 2 classes.

## VISUALISE TRAINING IMAGES FROM BOTH CLASSES:-
### 1. NORMAL:-
![image](https://github.com/user-attachments/assets/35932c50-5bb0-4f98-8493-5e84703ace49)

### 2. PNEUMONIA :-
![image](https://github.com/user-attachments/assets/af2cbc3f-c027-4248-bbd7-0938de869253)

## BUILD ARCHITECTURE:-
**Use VGG16 transfer learning technique to build a architecture for detect the X-ray.**

1. Total params: 14,978,370
2. Trainable params: 263,682
3. Non-trainable params: 14,714,688
* Use flatten layer to convert output into 1D array
* Use sigmoid activation function at last FCNN layer because only 2 classes are present.

### MODEL COMPILATION & TRAINING & EVALUATION :-
* Use binary cross_entropy and adam optimaizer to compile a model.
* Train model on  30 epochs, and plot training, validation accuracy as well as loss and validation loss.
* **After evaluating the model**
 * 118/118 [==============================] - 223s 2s/step - loss: 0.1529 - accuracy: 0.9434 
   Train Accuracy & Loss: [0.15292632579803467,0.9434137344360352]
 * 8/8 [==============================] - 332s 47s/step - loss: 0.3201 - accuracy: 0.8580
   Testing Accuracy & Loss [0.3200925290584564, 0.8579999804496765]

## MODEL SAVING :-
* Save the model using h5.

## PREDICTION & TESTING:-
* Select the image from testing data for prediction after that convert this image into array, and expand the diamension of image then Select the maxarg and last making the prediction using if elase condition.

## VISUALISE SOME PREDICTION:-

![image](https://github.com/user-attachments/assets/e623ed12-3928-47d6-87e9-b7bc8c45ebde)

## DEPLOY MODEL USING FLASK FRAMWORK .

## LIBRARY USED:-
* Tensorflow
* Keras
* Matplotlib
* Glob
* Numpy
* Splifolder
* Open CV
* OS

## TOOL USED:-
* Jupyter Notebook





