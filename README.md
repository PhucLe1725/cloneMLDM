# Machine learning project about Sign Language Classification using CNN 

## To work on your local computer, you need to:
1, In the terminal, navigate to the directory containing the project and install these packages and libraries:
- pip install -r requirements.txt

2, Download data from these 2 links:
- "https://drive.google.com/file/d/1FOj1n1BoU1U9MDuT0rjww6xI76ON6GlV/view?usp=sharing", this one is our train and validity dataset.
- "https://drive.google.com/drive/folders/1gZ7esm-I1as9vo-rbCKwsFHITHo7z_XV?usp=sharing", this one is our test dataset.

## About our files
1, "model.py" file is used to run our model, you need to change the directories in our code to the data folders you just downloaded: 
- "ROOT_PATH_1" should be "/dataa/asl_alphabet_train";
- "ROOT_PATH_2", "ROOT_PATH_3" and "ROOT_PATH_TEST_1" should be "/dataa".

After running the model, it is saved in "gray_model.h5" file.

2, "gray_model.h5" is used to store our model after training, you can use it direcly in our predicting files "test_for_newdata.py" and "predict_image.py" without training the model again.

3, "predict_image.py" is the fie used for predicting single hand sign image. You need to copy the directory of the picture you want to classify on your computer and paste it as the "image_path"(line 10). It will then rescale the image and predict the letter.

4, "test_for_newdata.py" is used to return model's accuracy for a total new dataset, you only have to change the directory of the folder you want to predict on the code by copy the folder path to "ROOT_PATH_TEST"(line 24).

Caution: You must save your data images in folders name A, B, C, etc. and put those folders in "data" folder, please check the test dataset above as an example.
