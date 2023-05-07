Download Link: https://assignmentchef.com/product/solved-neural-network-mini-project-number1-what-breast-cancer-will-recur
<br>
This work will require you to download a “real” (i.e. not toy) data set relating to Breast Cancer recurrence prediction.    The data set has values taken from a mass extracted from a patient suffering from breast cancer  and then indicates whether or not the cancer recurs and how long it takes.

There are approximately 151 patients that did not recur; and 47 that recurred.  (This is not a  “balanced” set ;i.e. different amounts of data for each of the two cases,  and you will have to take that into account when considering the quality of your results.  Be sure to explain how you handled this part of the problem.)

Your goal is to implement some of our algorithms and report on how accurate they should be for generalization.

You will implement the following algorithms:

(1)  perceptron algorithm .    (Your own code.   The sets are not linearly separable; but you should indicate how you discover this when running the perceptron.)

(2) <strong>Adaline algorithm</strong> .   (Your own code.   After training the adaline, you can impose a cut-off to decide which class the data point belongs to.  For example, if you try to train the adaline to +1 for Recurring  and -1 for Non-recurring then you can use 0 as a cut-off; i.e. a positive result means recurring and negative non-recurring.)

(3) <strong>Backpropagation algorithm</strong>.    Here you have a <strong>choice</strong> between your own code and the code of a package.      (i)  For your own code, use only one hidden level; and experiment with how many neurons there will be here.    Report on how it worked for each number of neurons and how much time it took.    I suggest you use the same  activation function on all neurons;  but you can experiment on this if you wish.   Be sure to report on the results of all your choices.      (ii)       Alternatively you can use a package on this problem from a package (like MATLAB or (for those who took the course in deep learning (Tensorflow)).  Other packages are also OK probably (I am not sure what is in WEKA, for example.)




The data set can be found at

https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wpbc.data

Explanation regarding the dataset:

<a href="https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wpbc.names">https://archive.ics.uci.edu/ml/machine-learning-databases/breast-cancer-wisconsin/wpbc.names</a>

note: you will need to filter the dataset using field (i.e. column) “2”:

R = recurrent, N = nonrecurrent

Additionally, you need to: leave out the first column (participant’s ID) and the third column (the recurrence time) from the data when implementing your algorithms.




Training and testing.

<ul>

 <li>You should divide the set into two classes;  say 66% for training and 33% for testing.   (You need to think about the balancing problem here, describe what you did …)   Indicate how long you trained and what the results were for the training class and the testing class.</li>

 <li>Having accomplished 1)  if you change the 33% choice 3 times,   you obtain 3 results.   This is called “cross-validation”.   You should report the average of these 3 results and the standard deviation.</li>

</ul>

<strong>Reporting the results:   (The quality of the REPORT will affect your grade significantly.)</strong>

A detailed word/pdf report file along with documented code is expected.  Besides the code I expect about 6 pages or so (not counting code).  <strong><em>You will be graded on completeness and clarity of the report as well as the quality of the implementation</em></strong><em>.</em>

In your report you should refer to the following items (i.e. <strong>I would like to see about 4 sections in your report</strong>):

<ul>

 <li>Time it took to train the final model (in sec or mins on your PC/Laptop) i.e. after all the cross validation processes.</li>

 <li>Ease (are the parameters can be adjusted intuitively or not) of parameter search/adaptation (e.g. learning parameter,  architecture of  feed-forward network (if any)) in order to find the best model for classification</li>

 <li>Performance on the training set and on the testing set (in %) – explain the results</li>

 <li>Summary and discussion of process/ problems.</li>

</ul>

Note: you might meet missing data (features) in some data points – you should think and decide what to do / how to deal with it and of course explain your decision (it doesn’t need to be some “scientific” decision).

The results should be reported clearly.   Be sure to include a tables like the following two ways:




<ul>

 <li>Confusion matrix for each model evaluation</li>

</ul>

<table>

 <tbody>

  <tr>

   <td width="132"> </td>

   <td width="235">Predicted: yes</td>

   <td width="185">Predicted: no</td>

  </tr>

  <tr>

   <td width="132">Actual: yes</td>

   <td width="235">True Positive (mean+/-std)</td>

   <td width="185">False Negative</td>

  </tr>

  <tr>

   <td width="132">Actual: no</td>

   <td width="235">False Positive</td>

   <td width="185">True Negative</td>

  </tr>

 </tbody>

</table>




<strong>Any additional charts and graphs will help</strong>.  (For example, a graph of quality of results over iterations of training data.)




Include an appendix with your codes (i.e. printed out) so we can read it when checking it.


