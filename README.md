# Potato Disease Analysis with CNN

A deep learning project for analyzing and classifying potato plant diseases using Convolutional Neural Networks (CNN).

## Project Overview

This project uses machine learning to detect and classify potato plant diseases:
- **Potato Early Blight**
- **Potato Late Blight**
- **Healthy Potatoes**

The model is trained using CNN architecture to automatically identify disease patterns from plant images.

## Project Structure

```
potato_analysis_CNN/
├── Potato___Early_blight/      # Dataset: Early blight disease images
├── Potato___Late_blight/       # Dataset: Late blight disease images
├── Potato___healthy/           # Dataset: Healthy potato images
├── venv/                       # Python virtual environment
└── README.md                   # Project documentation
```

## Prerequisites

- Python 3.8 or higher
- pip (Python package manager)
- Git (for cloning the repository)

## Installation & Setup

### 1. Clone the Repository

```bash
git clone <repository-url>
cd potato_analysis_CNN
```

### 2. Create Virtual Environment

Create a Python virtual environment to isolate project dependencies:

```bash
python3 -m venv venv
```

### 3. Activate Virtual Environment

**On Linux/macOS:**
```bash
source venv/bin/activate
```

**On Windows:**
```bash
venv\Scripts\activate
```

### 4. Install Required Packages

Install Jupyter, IPykernel, and other dependencies:

```bash
pip install jupyter ipykernel
```

For machine learning and data processing, you may also need:

```bash
pip install numpy pandas matplotlib scikit-learn tensorflow keras opencv-python pillow
```

### 5. Register Jupyter Kernel

Make the virtual environment available as a Jupyter kernel:

```bash
python -m ipykernel install --user --name=potato-env
```

## Running Jupyter Notebooks

### Option 1: Using VS Code

1. Open the project folder in VS Code
2. Create or open a `.ipynb` notebook file
3. Click the **"Select Kernel"** button (top-right corner)
4. Choose **`potato-env`** from the kernel list
5. Start writing and executing Python code

### Option 2: Using Jupyter Lab/Notebook

Start Jupyter Lab:
```bash
jupyter lab
```

Or start Jupyter Notebook:
```bash
jupyter notebook
```

This will open a browser window where you can create and run notebooks.

## Dataset

The project includes three folders with potato leaf images:

- **Potato___healthy/**: Images of healthy potato plants
- **Potato___Early_blight/**: Images showing early blight disease symptoms
- **Potato___Late_blight/**: Images showing late blight disease symptoms

You can organize your analysis notebooks to:
1. Load and explore the dataset
2. Preprocess images
3. Train the CNN model
4. Evaluate model performance
5. Make predictions on new images

## Typical Workflow

1. **Data Exploration**: Load images and analyze distribution
   ```python
   import os
   from PIL import Image
   import matplotlib.pyplot as plt
   
   # Load and display sample images
   disease_dir = './Potato___Early_blight/'
   images = os.listdir(disease_dir)[:5]
   ```

2. **Data Preprocessing**: Normalize and augment images

3. **Model Building**: Create CNN architecture

4. **Training**: Train the model on your dataset

5. **Evaluation**: Test model accuracy and performance

6. **Prediction**: Use the trained model to classify new images

## Deactivating Virtual Environment

When you're done working, deactivate the virtual environment:

```bash
deactivate
```

## Troubleshooting

### Command 'python' not found
Use `python3` instead on Linux/macOS systems.

### Kernel not showing up in VS Code
Reload VS Code after installing the kernel:
- Close and reopen VS Code, or
- Run the command palette (Ctrl+Shift+P) → "Reload Window"

### Missing packages error
Install the required package:
```bash
pip install <package-name>
```

## Dependencies

Key packages used in this project:

| Package | Purpose |
|---------|---------|
| **jupyter** | Interactive notebook environment |
| **numpy** | Numerical computing |
| **pandas** | Data manipulation and analysis |
| **tensorflow/keras** | Deep learning framework |
| **opencv-python** | Image processing |
| **pillow** | Image handling |
| **matplotlib** | Data visualization |
| **scikit-learn** | Machine learning utilities |

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is open source and available under the MIT License.

## Contact

For questions or suggestions, please open an issue on GitHub.

---

**Last Updated:** December 24, 2025
