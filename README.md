# Let's Keep It Short And Simple
# Introduction to Saving And Loading Model in Tensorflow
As we know that deep learning model really takes a lot of time to training and once we achieved a better performance, we do not want to try it further in future for our new data prediction, So it is always recommended to save the model to your disk so as to load it for future use.
In this Colab,
1. You will first load the infamous Cats/Dogs Classification dataset 
2. You will build a model for the classification task using Transfer Learning (using pre-trained model)
3. Check the model by predicition
4. Save the model {In Keras, models are saved with the extension of HDF5 (.h5)}
5. Loading the model to your working file
6. How to train the reloaded model again
7. How to use Tensorflow SavedModel format -
                    1. SavedModel is a standalone serialization format for Tensorflow objects, supported by TensorFlow serving as well as TensorFlow implementations other than                        Python. 
                    2. A SavedModel contains a complete TensorFlow program, including weights and computation. It does not require the original model building code to run,                            which makes it useful for sharing or deploying (with TFLite, TensorFlow.js, TensorFlow Serving, or TFHub).
                    3. The SavedModel files that were created contain:
                       - A Tensorflow checkpoint containing the model weights.
                       - A SavedModel proto containing the underlying Tensorflow graph. Separate graphs are saved for predictions (serving), train, and evaluation. If the model                          wasn't compiled before, then only the inference graph gets exported.
                       - The model's architecture config, if available.
