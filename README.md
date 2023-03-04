# Overview
Alphabet Soup is looking for a tool that can help select funding for applicants with the best chance of success in their ventures.

## Results
After 3 trials the best accuracy score: 0.7287463545799255 (Module 3)

### Files
* AlphabetSoupCharity_Optimization.ipynb (Jupyter Notebook - Google Colaboratory)
* AlphabetSoupCharity_Optimization1.h5 (Trial 1)
* AlphabetSoupCharity_Optimization2.h5 (Trial 2)
* AlphabetSoupCharity_Optimization3.h5 (Trial 3)
### Data Processing
* I used the X_train_scaled[5] (APPLICATION_TYPE_T12) for my feautres
* No variables were removed except for what was required in the module
### Compiling, Training, and Evaluating the Model
#### Trial 1
Model: "sequential"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 dense (Dense)               (None, 70)                3640      
                                                                 
 dense_1 (Dense)             (None, 30)                2130      
                                                                 
 dense_2 (Dense)             (None, 1)                 31        
                                                                 
=================================================================
Total params: 5,801
Trainable params: 5,801
Non-trainable params: 0
_________________________________________________________________

#### Trial 2
Model: "sequential_2"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 dense_6 (Dense)             (None, 65)                3380      
                                                                 
 dense_7 (Dense)             (None, 15)                990       
                                                                 
 dense_8 (Dense)             (None, 1)                 16        
                                                                 
=================================================================
Total params: 4,386
Trainable params: 4,386
Non-trainable params: 0
_________________________________________________________________

#### Trial 3
Model: "sequential_6"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 dense_18 (Dense)            (None, 100)               5200      
                                                                 
 dense_19 (Dense)            (None, 100)               10100     
                                                                 
 dense_20 (Dense)            (None, 1)                 101       
                                                                 
=================================================================
Total params: 15,401
Trainable params: 15,401
Non-trainable params: 0
_________________________________________________________________

### Summary
Based on the three trials, trial 3 preformed slightly better with more total params.  Before I could make a recommendation I would need to spend more time understanding the data.  I feel with more knowledge about the data I would have more insight into which columns should be included/excluded from the training models.