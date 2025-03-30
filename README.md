🌱 Vegetable Image Classification

This project focuses on classifying vegetable images using a Convolutional Neural Network (CNN) trained on the Vegetable Image Dataset. The dataset consists of 15 vegetable classes and contains a total of 21,000 images, which are preprocessed and augmented to enhance model performance.

📂 Dataset Structure

The dataset is divided into three subsets:

Train: 15,000 images (70%)

Validation: 3,000 images (15%)

Test: 3,000 images (15%)

Each subset contains subfolders representing different vegetable categories:

Bean ,Bitter Gourd ,Bottle Gourd ,Brinjal ,Broccoli ,Cabbage ,Capsicum ,Carrot ,Cauliflower ,Cucumber ,Papaya ,Potato ,Pumpkin ,Radish ,Tomato

🚀 Model Architecture

The CNN model consists of:

Input Layer: (224, 224, 3) for RGB images

Convolutional Layers with ReLU activation

MaxPooling Layers to reduce spatial dimensions

Flatten Layer to convert feature maps into a 1D vector

Fully Connected Layers (Dense Layers) with dropout for regularization

Output Layer with softmax activation for 15-class classification

🛠️ Preprocessing & Augmentation

We use ImageDataGenerator from Keras for:

Rescaling pixel values to [0,1] range

Rotation (20°)

Zooming (20%)

Horizontal Flipping for better generalization

📊 Training & Evaluation

The model is trained using:

Loss Function: Categorical Crossentropy

Optimizer: Adam

Metric: Accuracy
