# Image-Segmentation-Using-U-Net

This is a work-in-progress notebook.

This notebook demonstrates the implementation of a U-Net architecture for image segmentation using TensorFlow and Keras. The U-Net model is a popular deep learning architecture for biomedical image segmentation tasks.

The notebook begins by defining the input and output shapes of the U-Net model. The model consists of a contracting path and an expansive path. The contracting path consists of four max pooling layers and four convolutional blocks. Each convolutional block includes two convolutional layers with a dropout layer in between. The expansive path consists of four upsampling layers and four convolutional blocks. Each upsampling layer is followed by a concatenation with the corresponding layer in the contracting path. The final layer is a 1x1 convolution layer with a sigmoid activation function to predict the segmentation mask.

The model is compiled with the Adam optimizer and the binary cross-entropy loss function. The model summary is printed to show the number of parameters and the shapes of the layers.

The notebook also defines a checkpoint callback to save the model with the best validation loss. 
