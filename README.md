<p align="center">
  <img src="https://user-images.githubusercontent.com/78701055/163567065-86a208ac-d2e5-4dac-96ad-0ecad66649b7.jpg" alt="">
</p>



<h1 align="center"> Handwritten Captcha Recognition </h1>


## Introduction

CAPTCHAs (Completely Automated Public Turing
Tests to Tell Computers and Humans Apart) are
something that almost every internet user has
encountered.They are used to differentiate a human client
and a robot.

This captcha solver has been developed using deep learning and convolutional neural networks along with the help of OpenCv for letter segmentation. It can be used to recognize captchas consisting of different **letters** as well as **emojis**. The model was trained on Google Colab using the EMINST by_class dataset in the form of a csv file. The dataset was modified to remove similar characters such as X and x. 

## Special Features of this model -
The special features of this model include :-  
  1. This model can recognize captchas consisting of letters and emojis.
  2. It can be also used for captchas consisting of lots of noise in the form of lines and dots.
  3. Can detect captchas having letters of variable thickness and size.

## Dataset -

### Letter Dataset:
The letter model is trained on the **EMINST** dataset, which is modified a little bit and hence can detect the followong letters -
**'H','I','J','K','N','T','W','X','Y','Z','f','r','t'**

### Emoji Dataset:
The emoji dataset consists of 7 emojis mapped as:

|<img src="https://user-images.githubusercontent.com/78701055/163564439-fd8aa49a-7604-41c0-9c83-55a2b4c2dac8.jpg" alt="" width="100"/> | <img src="https://user-images.githubusercontent.com/78701055/163565375-cb875b9b-9698-45e1-9c3a-48b3cae8fbd3.jpg" alt="" width="100"/> |  <img src="https://user-images.githubusercontent.com/78701055/163565378-e8e768c1-b9db-410f-a30a-e9f0171d4ec4.jpg" alt="" width="100"/> | <img src="https://user-images.githubusercontent.com/78701055/163565383-34e5dd5a-e40c-4346-8f74-4dfefa261027.jpg" alt="" width="100"/> | <img src="https://user-images.githubusercontent.com/78701055/163565391-5f52a4c5-0ae8-463d-8dfc-6df3958f3eee.jpg" alt="" width="100"/> |  <img src="https://user-images.githubusercontent.com/78701055/163565395-d51900b7-d46e-44d9-b188-0058e1e2c4ce.jpg" alt="" width="100"/> | <img src="https://user-images.githubusercontent.com/78701055/163565402-b88c2d4f-9171-44ab-b5ee-b0ba254a2861.jpg" alt="" width="100"/> |
|--|--|--|--|--|--|--|
|Checkmark : 1 | Cloud: 2 | Croissant: 3 | Heart: 4 | Laugh: 5 | Smile: 6 | Sun: 7 |

## How to Use -


<p align="center">
<img src="https://user-images.githubusercontent.com/78701055/163561542-863fc2c4-2f58-467d-ab4a-f1887db78f0e.png" alt="" width="70%">
<img src="https://user-images.githubusercontent.com/78701055/163562737-e6e29827-aa61-4dd8-804a-906d5abf8ab0.png" alt="" width="25%">
</p>

Upload the [Final_Pipeline.ipynb](https://github.com/SanidhyaTaparia/Mosaic-2022/blob/main/Final_Pipeline.ipynb) file on Google Collab, and then put [Letters_model_final.h5](https://github.com/SanidhyaTaparia/Mosaic-2022/blob/main/Letters%20Detection/Letters_model_final.h5), [Emogis_model_final.h5](https://github.com/SanidhyaTaparia/Mosaic-2022/blob/main/Emojis%20Detection/Emogis_model_final.h5) in the files section (for trained models). Also upload the image of the captcha required to be detected (Examples available in [Testing Images](https://github.com/SanidhyaTaparia/Mosaic-2022/tree/main/Testing%20Images) folder). Now execute the `Final_Pipeline.ipynb` to see the results.

NOTE: The model is trained for the above mentioned letters so give them only in input images for best output.

<br>
