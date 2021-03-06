# ML Classification Practice

This project is a practice based on professor Hung-Yi Lee's ML Lecture. Notice that it is a binary classification case.

The output is just a posterior probability, hence if the the posterior probability is greater than 0.5 than it belongs to C1 else C2.

We can get the posterior probability by using Bayes' theorem. For example, given input x, the probability of x belonging C1 is P(C1|x), we then can use Bayes' theorem to find the answer. <img src="https://latex.codecogs.com/svg.latex?P(C_1|x)=\frac{P(C_1)P(x|C_1)}{P(C_1)P(x|C_1)&plus;P(C_2)P(x|C_2)}" title="P(C_1|x)=\frac{P(C_1)P(x|C_1)}{P(C_1)P(x|C_1)+P(C_2)P(x|C_2)}" />

The prior probability P(C1) P(C2) and distribution probability P(x|C1) P(x|C2) are the parameters of this model. The way we calculate distribution probability
is using Generative Model (assume the training set is generated by a Gaussian Distribution). Therefore, we then use Maximum Likelihood to find the optimal mean and covariance of this Gaussian.

##### Professor Hung-Yi Lee's profile: http://speech.ee.ntu.edu.tw/~tlkagk/courses.html
##### Dataset: https://www.kaggle.com/abcsds/pokemon
