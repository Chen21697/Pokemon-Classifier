# ML Classification Practice

This project is a practice based on professor Hung-Yi Lee's ML Lecture. Notice that it is a binary classification case.

The output is just a posterior probability, hence if the the posterior probability is greater than 0.5 than it belongs to C1 else C2.

We can get the posterior probability by using Bayes' theorem. For example, given input x, the probability of x belonging C1 is P(C1|x), we then can use Bayes' theorem to find the answer. ![equation](http://www.sciweavers.org/tex2img.php?eq=P%28C_1%7Cx%29%3D%5Cfrac%7BP%28C_1%29P%28x%7CC_1%29%7D%7BP%28C_1%29P%28x%7CC_1%29%2BP%28C_2%29P%28x%7CC_2%29%7D&bc=White&fc=Black&im=jpg&fs=12&ff=arev&edit=)

The prior probability P(C1) P(C2) and distribution probability P(x|C1) P(x|C2) are the parameters of this model. The way we calculate distribution probability
is using Generative Model (assume the training set is generated by a Gaussian Distribution). Therefore, we then use Maximum Likelihood to find the optimal mean and covariance of this Gaussian.

##### Professor Hung-Yi Lee's profile: http://speech.ee.ntu.edu.tw/~tlkagk/courses.html
##### Dataset: https://www.kaggle.com/abcsds/pokemon
