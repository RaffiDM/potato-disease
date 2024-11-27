# Potato Disease Classification

## Project Description
This is a machine learning project for classifying potato plant conditions using deep learning and TensorFlow. The model can identify three categories:
- Healthy Potato
- Early Blight
- Late Blight

## Project Structure
```
potato-disease/
│
├── training/
│   ├── training.ipynb
│   └── PlantVillage/
│       ├── Potato__Early_blight/
│       ├── Potato_Healthy/
│       └── Potato__Late_blight/
│
├── models/
│   └── 
│
└── requirements.txt
```

## Requirements
To run this project, install the dependencies using:
```bash
pip install -r requirements.txt
```

### Key Dependencies:
- TensorFlow
- NumPy
- Matplotlib

## Model Architecture
The model uses a Convolutional Neural Network (CNN) with:
- Image input size: 256x256 pixels
- Data augmentation
- 6 convolutional layers
- Batch size: 32
- Epochs: 50

## Training Process
1. Load dataset from PlantVillage folder
2. Split dataset into training (80%), validation (10%), and testing (10%)
3. Preprocessing:
   - Image resizing
   - Pixel value rescaling
   - Data augmentation

## Model Evaluation
Model is evaluated using:
- Loss function: Sparse Categorical Crossentropy
- Optimizer: Adam
- Metric: Accuracy

## Usage
1. Run the training.ipynb notebook
2. Model will be saved in the `models/` folder
3. Use the model to predict potato leaf conditions

## Performance Visualization
The training process includes visualization of:
- Training and Validation Accuracy
- Training and Validation Loss

## Future Improvements
- Expand dataset
- Fine-tune model hyperparameters
- Add more sophisticated data augmentation techniques

## Acknowledgments
- Dataset sourced from https://www.kaggle.com/datasets/arjuntejaswi/plant-village
