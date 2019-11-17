# internship_assignment


# TASK - 1
     1.Using a 7 layers CNN architecture we get very good results on our test data of over 94% accuracy.

     2.We see that the dataset is unbalanced where letter are dominating the digits by alot and thus to remove this                             biasness we use class_weights.

     3.We penalize out learning rate by 90% if accuracy does not increase for more than 2 epochs.

     4.To prevent overfitting we use dropout > 0.6 and reduce the number of convolutional layers.

     5.Experimented with various learning rate techiniques such as Cyclic learning rates,ReduceonPleatea,and Optimizers                         and got best results with Adadelta.

     6.Use of bactch normalization for smooth training and better results.

   ### RESULTS

                      +-------+---------------------+--------------------+
                      |  Data |         Loss        |   Accuracy In %    |
                      +-------+---------------------+--------------------+
                      |  Test |  0.1251189125623213 | 0.9405819458545247  |
                      | Train | 0.10397172433411961 | 0.9529341713561154 |
                      |   CV  |   127259231002970   | 0.9416774124220932 |
                      +-------+---------------------+--------------------+

# TASK-2

       1.For classifying odd and even digits we use a 5 layered CNN architectures while we use 6 layerd architecture for                          classifying vowel and consonants.

       2.We see that the dataset is unbalanced where consonants are dominating the vowels by alot and thus to remove this                        biasness we use class_weights.

       3.To prevent overfitting we use dropout > 0.6 and reduce the number of convolutional layers.

       4.Experimented with various learning rate techiniques such as Cyclic learning rates,ReduceonPleatea,and Optimizers                        and got best results with Adadelta.

       5.Use of bactch normalization for smooth training and better results.

       6.Introducing Maxpooling layers

       7.Finally we load all the three models model_task_1 for classifying into digit/letter,model_odd_even for classifying                      odd/even and model_vowel_cons for classifying vowel/consonants

   ### INSTRUCTION TO RUN THE PIPELINE - 
      RUN ALL THE CELLS UNDER THE "COMPLETE PIPLELINE" HEADING IN "task_2.ipynb" BY UPLOADING ALL THE RESPECTIVE MODELS GIVEN IN /model/       directory"

 
   ### RESULTS

                    +-----------------------+-------+----------------------+--------------------+
                    |         Model         |  Data |         Loss         |   Accuracy In %    |
                    +-----------------------+-------+----------------------+--------------------+
                    |     model_odd_even    |  Test | 0.019035957532483737 |      0.99475       |
                    |     model_odd_even    | Train | 0.00671219013002788  | 0.9976990049751244 |
                    |     model_odd_even    |   CV  | 0.020536658105508348 | 0.9953282828282828 |
                    | model_vowel_consonant |  Test | 0.07397996356767556  | 0.972362997499831  |
                    | model_vowel_consonant | Train | 0.045407581085349986 | 0.9815614757542651 |
                    | model_vowel_consonant |   CV  | 0.07022251497308078  | 0.9726999726999727 |
                    +-----------------------+-------+----------------------+--------------------+

# TASK-3

       1.Using a 7 layers CNN architecture we get very good results on our test data of over 99% accuracy.

       2.To prevent overfitting we use dropout > 0.5.

       3.We also penalize our learning rate by 90% when accuracy falls for more than 2 epochs

       4.Experimented with various learning rate and Optimizers and got best results with Adadelta.

       5.Use of bactch normalization for smooth training and better results.
       
### RESULTS
         +-------+----------------------+--------------------+
        |  Data |         Loss         |   Accuracy In %    |
        +-------+----------------------+--------------------+
        |  Test | 0.012939076293873178 | 0.9950597385686981 |
        | Train | 0.010478593149658981 | 0.9958001604570761 |
        |   CV  | 0.01249637532158213  | 0.9951398506898305 |
        +-------+----------------------+--------------------+
       
###  INSTRUCTION TO RUN THE PIPELINE - 
      RUN ALL THE CELLS UNDER THE "COMPLETE PIPLELINE" HEADING IN "task_3.ipynb" BY UPLOADING ALL THE RESPECTIVE MODELS GIVEN IN /model/       directory"
