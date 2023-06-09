# Keystroke-based Identification
Python code for collecting and authenticating a user based on their keystroke patterns.


## Running

* Using Python(Make sure you are using python 3.6 or above):
    ```
    pip install -r requirements.txt  
    python app.py  
    ```

Either way, the web page is accessible from localhost:5000
## Project explanation
The code consists of the following parts
### Data collection
To collect data a web interface was implemented using Flask and keystrokes timing were sampled with the aid of Javascript event handlers.
### Feature Extraction
[feature_extractor](model_code/feature_extractor.py) the takes raw data and produces 3 different feature data set
### Training
[Training](/model_code/trainer.py) was done using two major algorithms
* Classic Machine-Learning
  * KNN
  * SVM
* Neural Network (Pytorch)
### Testing
The web platform also uses the model and performs a authentication using previous mentioned methods

