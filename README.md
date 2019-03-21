# GATEmachineLearnDemo
This repository include demo for GATE learning framework

## Rquirement
GATE 8.5.1 or above


## Classification
Classification demo is a sentence level sentiment classification 
### Train model:
    1. Open GATE developer
    2. Click File -> Restore Application from File
    3. Select classificationTrain.xgapp
    *. (The application and training corpus will loded automaticly)
    *. (If you inspect data in GATE developer, the training instances are labeled "Sentence" with feature "class" )
    4. Double click loaded application (classificationTrain)
    5. In the application tab, click "Run this application" at bottom of the window.
    
### Test model:
    1. Open GATE developer
    2. Click File -> Restore Application from File
    3. Select classificationTest.xgapp
    *. (The application and testing corpus will loded automaticly)
    4. Double click loaded application (classificationTest)
    5. In the application tab, click "Run this application" at bottom of the window.    
    *. (If you inspect the data after run the application, you should see a new annotation set called "LearningFramework")
    *. (The "LearningFramework" should contain annotation type "Sentence" with predicted feature "class")


## Chunking
Chunking demo is a Disease entiry recognition task. 
### Train model:
    1. Open GATE developer
    2. Click File -> Restore Application from File
    3. Select train.xgapp
    *. (The application and training corpus will loded automaticly)
    *. (If you inspect data in GATE developer, the training instances are labeled "Disease" in "ConsensusAuto" set )
    4. Double click loaded application (Training)
    5. In the application tab, click "Run this application" at bottom of the window.
    
### Test model:
    1. Open GATE developer
    2. Click File -> Restore Application from File
    3. Select testing.xgapp
    *. (The application and testing corpus will loded automaticly)
    4. Double click loaded application (testing)
    5. In the application tab, click "Run this application" at bottom of the window.    
    *. (If you inspect the data after run the application, you should see a new annotation set called "LearningFramework")
    *. (The "LearningFramework" should contain predicted annotation type "Disease" )
    
## Topic Modelling
Topic Modelling demo is unsupervised topic model clustering task
### Train and Apply model:
    1. Open GATE developer
    2. Click File -> Restore Application from File
    3. Select trainLda.xgapp
    *. (The application and training corpus will loded automaticly)
    *. (Using same data as chunking demo)
    4. Double click loaded application (TrainLDA)
    5. In the application tab, click "Run this application" at bottom of the window.
    *. (This takes much longer time than previous tasks)
    6. After training, you should find 4 file under the folder "machineLearnModels/lda/"
    *. topWordsPerTopic.txt - top 10 topic words words for each topics 
    *. topDocsPerTopic.txt - top 5 documents contains each topic
    *. topTopicPerDoc.txt - topic proportion for each document
    *. topicWordWeights.txt - topic word weights in each topic
    



