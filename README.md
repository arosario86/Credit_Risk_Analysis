# Credit_Risk_Analysis

## Overview
The overall goal of this analysis was to create a supervised machine learning model that would enable me to predict credit risk from loan applicants based off of the data in the provided csv file.

## Results
The first model was based on resampling techniques.
* Based on the target values, there is a total of 68,470 low-risk applicants, and 347 high-risk applicants.

![Target_Values](https://user-images.githubusercontent.com/104965708/200490375-49fa036e-673e-46c4-8ac7-f90162317903.png)

* When training the model, the train shape is [51612, 95]
* Accuracy score was 0.65
* Imbalanced Classification Report shows the average and totals for high-risk and low-risk applicants.

![Imbalanced](https://user-images.githubusercontent.com/104965708/200490867-877710b4-5f44-44a8-b9d1-1de0b2dd64bb.png)

The second model was based on credit risks using the Balanced Random Forest Classifier.
Note: I kept receiving an error message for the easy ensemble classifier attribute. I looked at many resources, downgraded my scikit-learn to 1.0.1, back to 0.9, and then right back to 1.0.1 and no luck. I still received the error despite upgrading and downgrading it.

![Error_Message](https://user-images.githubusercontent.com/104965708/200489636-8a78ead5-c348-49f0-a85e-945fedbe22d1.png)

* The confusion matrix shows that the actual high risk is 37 and the predicted high risk is 64.
    * The actual low risk is 5 and the predicted low risk is 17,099.
    
![Confusion Matrix](https://user-images.githubusercontent.com/104965708/200491621-97612545-fce2-4462-907c-e75224859509.png)
