# deep-learning-challenge

   
   
    Overview of the analysis: Explain the purpose of this analysis.

    In this exercise, I used the features in the provided dataset to create a binary classifier that can predict whether applicants will be successful if funded by Alphabet Soup.

    The dataset included more than 34,000 organizations that have received funding from Alphabet Soup over the years. Within this dataset are a number of columns that capture metadata about each organization. 
    The notebooks included in this git  detail an attempt to reach 75% predictive accuracy with a neural network. Specifically, the features were used to predict whether or not a charity would be successful. Multiple rounds of both feature tweaking and neural net tuning were used to attempt to reach the accuracy goal. However, it was not reached.


    Results: Using bulleted lists and images to support your answers, address the following questions:

    Data Preprocessing
        What variable(s) are the target(s) for your model? IS_SUCCESSFUL
        What variable(s) are the features for your model? eventually, Application Type, AFfiliation, Classification, Use Case, Status, Income Amount and Ask Amount
        What variable(s) should be removed from the input data because they are neither targets nor features?
        'EIN', 'NAME','SPECIAL_CONSIDERATIONS_N','SPECIAL_CONSIDERATIONS_N','ORGANIZATION_Trust','ORGANIZATION_Corporation','ORGANIZATION_Co-operative','ORGANIZATION_Association'

    Compiling, Training, and Evaluating the Model
        How many neurons, layers, and activation functions did you select for your neural network model, and why?
            For final model I selected 4 hidden layers (100 relu neurons, 100 relu neurons, 50 tanh neurons, 50 tanh neurons and 1 output layer (1 sigmoid neuron)). I also added an ADAM optimizer learning rate to fine tune the  model. Fine tuned from 0.001 to 0.1 in the final model. 
        Were you able to achieve the target model performance? No
        What steps did you take in your attempts to increase model performance?
        in addtion to above, i cut out more application types so only types greater than 1000 were included, to reduce the noise. I also addeda few more classification counts by considering onkly above 700 and not only above 1000 like before. I also reduced the number of features. 

    Summary: Summarize the overall results of the deep learning model. Include a recommendation for how a different model could solve this classification problem, and then explain your recommendation.
