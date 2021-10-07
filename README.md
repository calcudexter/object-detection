## Bouding Box Regression  
### Overview  
Here, I have trained two CNN architectures :  
 - One predicts bounding boxes of a single class - Airplanes as shown below  
 Notebook : ```bounding_box_regressor.ipynb```  
 ![Monoclass BB Regression](monoclass_bounding_box_regression.png "Airplanes")

 - The other is fine tuned for predicting class labels as well as boxes for 5 different classes chosen at random from the CALTECH101 dataset.  
 The link to the dataset, necessary preprocessing can be found out in ```multiclass_bounding_box.ipynb```  
 ![Multiclass BB Regression](multiclass_bounding_box_regression.png "Multiclass")  

### Model Architecture  
![Regressor Architecture](regressor.png "Regressor")  <br/><br/>
The two output branches, one for classification and other for bounding box regression, improve the overall efficiency of the task cause being the use of a better loss function.  

Tutorial : [PyImageSearch](https://www.pyimagesearch.com/2020/10/12/multi-class-object-detection-and-bounding-box-regression-with-keras-tensorflow-and-deep-learning/)
