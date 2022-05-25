# Detecting Parkinsons From Geometric Drawings
This is an app that allows for the quick diagnosis of Parkinson's disease based on geometric drawings.

The principle behind it is based on a study by [Zham et.al](https://www.frontiersin.org/articles/10.3389/fneur.2017.00435/full) where they found out that it was possible 
to detect Parkinson’s by asking the patient to draw a spiral and then track

    1.Speed of drawing
  
    2. Pen pressure

The researchers found that the drawing speed and pen pressures were lower among Parkinson’s patients- This was especially pronounced for patients with a more acute/advanced forms of the disease

The classical tremors and muscle rigidity of Parkinson's also directly impact the visual appearance of a hand drawn spiral and wave. 
The current app leverages on this variations by quantifing the visual appearance of these drawings and then trains a machine learning model to classify them.

The data set was curated by Adriano de Oliveira Andrade and Joao Paulo Folado from the NIATS of Federal University of Uberlândia.

The dataset itself consists of 204 images and is pre-split into a training set and a testing set, consisting of:

    1. Spiral: 102 images, 72 training, and 30 testing
    
    2. Wave: 102 images, 72 training, and 30 testing
    
## Parts
    1. detecting_pakinsons.ipynb - Jupyter notebook documenting model creation
    
    2. predicting_parkinsons.py - Helper method that analyzes an image an outputs a prediction based on the saved models
    
    3. app.py - GUI application
    
## Usage
Install python and run the following commands

    pip istall requirements.txt
    
    python app.py or python3 app.py
