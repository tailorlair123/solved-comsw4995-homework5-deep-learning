Download Link: https://assignmentchef.com/product/solved-comsw4995-homework5-deep-learning
<br>
<h1>Task 1</h1>

Run a multilayer perceptron (feed forward neural network) with two hidden layers and rectified linear nonlinearities on the digits dataset from sklearn using the keras​<a href="https://keras.io/getting-started/sequential-model-guide/"> Sequential interface</a><a href="https://keras.io/getting-started/sequential-model-guide/">.</a><u>​</u>

Include code for selecting L2 regularization strength and number of hidden units using GridSearchCV and evaluation on an independent test-set.

Task 2

Train a multilayer perceptron (fully connected) on the Fashion MNIST dataset using the traditional train/test split as given by fashion_mnist.load_data in keras. Use a separate 10000 samples (from the training set) for model selection and to compute learning curves (accuracy vs epochs, not accuracy vs n_samples). Compare a “vanilla” model with a model using drop-out and evaluate if using drop-out allows you to learn a bigger network. Then, compare to a model using batch normalization. Visualize learning curves for all models.

Task 3

Train a convolutional neural network on the following dataset: <a href="https://lhncbc.nlm.nih.gov/publication/pub9932">https://lhncbc.nlm.nih.gov/publication/pub9932</a>

The goal is to classify cells infected with malaria against those that are not.

<strong>3.1</strong> Start with a convolutional model without residual connections (using batch normalization is​      likely to be helpful and you should try it, whether you use dropout is your choice).

<strong>3.2 </strong>Augment the data using rotations, mirroring and possibly other transformations. How much​     can you improve your original model by data augmentation?

<strong>3.3</strong> Build a deeper model using residual connections. Show that you can build a deep model​          that would not be able to learn if you remove the residual connections (i.e. compare a deep model with and without residual connections while the rest of the architecture is constant). Feel free to reuse existing architectures from the literature or use them as inspiration for your own. You can find commonly used architectures here: <a href="https://keras.io/applications/">https://keras.io/applications/</a>

However, the point of the exercise is to learn the weights from scratch, so please do not reuse the weights shipped with these applications.

3.4 BONUS / Optional: Transfer learning

Reuse an existing architecture from keras (<a href="https://keras.io/applications/">https://keras.io/applications</a>​         <a href="https://keras.io/applications/">/</a>)​ and compare retraining only the densely connected layer with fine-tuning the whole network.

<strong>Hint</strong>:​ Make sure you are doing the reshape for the training set correctly. A direct reshape might​   give you garbled images. Display an image after reshaping to make sure they are correct.

Some additional advice to help you along:

<ul>

 <li>Make sure all your code is running on GPU. You can use debugging.set_log_device_placement(​True​)​to see which device is being used and confirm it is the device you intended.</li>

 <li>Preprocess the images before training a model.</li>

 <li>Test your code on a small part of the data before training the model. You don’t want your code to fail on a print statement after waiting for the network to train.</li>

</ul>


