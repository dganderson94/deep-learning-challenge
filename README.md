# Overview
The purpose of this analysis is to develop a neural network that can reliably predict which ventures are likely to be successful with the aid of a loan from Alphabet Soup.

# Results

* ## Data Preprocessing
  * Target: Whether or not the venture was a success

  * Features:
    * Application Type
    * Affiliation
    * Classification
    * Use Case
    * Type of Organization
    * Active Status
    * Income Amount
    * Special Considerations
    * Ask Amount

  * Removed Variables:
    * EIN
    * Name of Organization

* ## Compiling, Training, and Evaluating
  * Parameters:
    * Neurons: 1,757
    * Layers: 7, including the output layer
    * Activation Functions: ReLu, Sigmoid
  * Rationale:
    * These parameters were selected more or less arbitrarily. Trying different combinations yielded no discernible pattern that could be followed to maximize performance.
    * I was not able to achieve the target model performance.
    * In my attempts to increase performance, I fiddled with the configuration of the model itself, as well as the ways in which the training data was binned.

# Summary
Overall, the model was not particularly successful in predicting the success of ventures funded by Alphabet Soup. Accuracy topped out at around 73%, just short of the target of 75%. A different model might be able to achieve higher accuracy in the following ways:
* By ignoring features that have little impact on success rate
* By utilizing different binning techniques for continuous features
* By reconfiguring the model with different activation functions and other parameters
* By training for more iterations

These changes would allow the model to more effectively hone in on what truly matters for predicting the success rate of a funded venture, both by narrowing the number of potential considerations and by creating a more nuanced model.
