# Layers_creation

Here I impelment my own custom layer. The layer is already available in Keras. I implemented Leaky ReLU using basic tf libraries, which is available in tf also. The data is popular mnist data, which is available with tf. The utils file will import the data and do the preprocessing for us, that consists some helper function.      

I used the formula of leaky-ReLU `tf.maximum(0., x) + self.alpha * tf.minimum(0., x)`, which is the equation of the activation. After training model(50k parameter) with our layer, on 5 epochs only, I compared my result with ReLU, which gives a good result with overall 97% acc on val set. Source code for python is available in the notebook. The helper function is also avilable as `utlis.py`.
