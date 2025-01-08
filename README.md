# Handwritten Equation Solver

This project uses deep learning and computer vision to solve handwritten mathematical equations. It includes data preprocessing, model training and a graphical user interface (GUI) for solving equations.

## File Structure

p1.py: Preprocesses images of handwritten characters and creates a training dataset. It extracts images from different folders, resizes them, and appends the label (digit or symbol) to each image.

p2.py: Defines and trains a Convolutional Neural Network (CNN) model using Keras. The model is used for recognizing the handwritten digits and symbols.

p3.py: A Tkinter-based GUI that allows users to upload images of handwritten equations, processes them, and displays the result of the equation after prediction by the trained model.

## Requirements

Install the necessary dependencies using pip:

`pip install -r requirements.txt`

## Required Libraries:

numpy
pandas
keras
opencv-python
matplotlib
Pillow
tkinter

## Usage

### Data Preparation (p1.py)

Run p1.py to preprocess images of handwritten equations. It loads images from different folders (representing different characters/symbols), resizes them to 28x28 pixels, and saves the resulting dataset as train.csv.

`python p1.py`

### Model Training (p2.py)

Once the dataset is prepared, run p2.py to train the model using the preprocessed data. The model will be saved as create_model_final.json (model architecture) and create_model_final.h5 (model weights).

`python p2.py`

### Solve Equations (p3.py)

Use p3.py to load the trained model and use the GUI to upload an image of a handwritten equation. The system will recognize the equation, solve it, and display the result.

`python p3.py`

The GUI allows you to:

Open an image of a handwritten equation.

Display the equation and its solution.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
