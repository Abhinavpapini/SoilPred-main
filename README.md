# 🌱 Soil Prediction System

A machine learning-based crop prediction application that determines the most suitable plant type based on soil parameters using K-Nearest Neighbors (KNN) algorithm.

## 📋 Table of Contents
- [Features](#features)
- [Screenshots](#screenshots)
- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Technology Stack](#technology-stack)
- [Project Structure](#project-structure)
- [How It Works](#how-it-works)
- [Model Performance](#model-performance)
- [Contact](#contact)

## ✨ Features

- **Machine Learning Prediction**: Uses KNN algorithm for crop recommendation
- **User-Friendly GUI**: Built with Tkinter for easy interaction
- **Real-time Predictions**: Instant crop recommendations based on soil parameters
- **Data Validation**: Input validation to ensure proper parameter values
- **Comprehensive Dataset**: Trained on extensive plant parameter data
- **Jupyter Notebook Analysis**: Complete data analysis and model development workflow

## 📸 Screenshots

The application includes visual elements and a user-friendly interface:
- Background image for enhanced UI experience
- Input fields for all 9 soil parameters
- Clear result display with color-coded feedback
- Menu system for navigation and information

## 🔧 Installation

### Prerequisites
- Python 3.7+
- Required Python packages (see requirements below)

### Setup
1. Clone or download this repository
2. Navigate to the project directory
3. Install required packages:

```bash
pip install pandas scikit-learn tkinter
```

### Required Files
Ensure these files are in your project directory:
- `soilprd.py` - Main application file
- `Plant_Parameters.csv` - Dataset file
- `crop_prediction_bg 1.png` - Background image
- `soilPred.ipynb` - Jupyter notebook for analysis

## 🚀 Usage

### Running the Application
```bash
python soilprd.py
```

### Input Parameters
The application requires the following soil parameters:

1. **pH** - Soil acidity/alkalinity level
2. **Soil EC** - Electrical conductivity of soil
3. **Phosphorus** - Phosphorus content in soil
4. **Potassium** - Potassium content in soil
5. **Urea** - Urea fertilizer amount
6. **T.S.P** - Triple Super Phosphate fertilizer
7. **M.O.P** - Muriate of Potash fertilizer
8. **Moisture** - Soil moisture percentage
9. **Temperature** - Soil temperature

### Steps to Use:
1. Launch the application
2. Enter values for all 9 soil parameters
3. Click "Display Data" button
4. View the predicted suitable crop type

### Menu Options:
- **File Menu**: New entry, Exit application
- **Options Menu**: Home, About Us, Contact Us

## 📊 Dataset

The `Plant_Parameters.csv` contains:
- **100,000+ records** of plant data
- **9 soil parameter features**
- **Multiple plant types** including Carrots and other crops
- **Normalized data** for better model performance

### Sample Data Structure:
```
pH, Soil EC, Phosphorus, Potassium, Urea, T.S.P, M.O.P, Moisture, Temperature, Plant Type
6.02, 0.24, 15.99, 133.21, 45.63, 16.95, 23.36, 79.23, 52.09, Carrots
```

## 💻 Technology Stack

- **Language**: Python 3.x
- **Machine Learning**: scikit-learn (KNN Algorithm)
- **GUI Framework**: Tkinter
- **Data Processing**: Pandas
- **Development Environment**: Jupyter Notebook
- **Data Analysis**: NumPy, Matplotlib (in notebook)

## 📁 Project Structure

```
SoilPred-main/
├── soilprd.py                 # Main application file
├── soilPred.ipynb            # Jupyter notebook for analysis
├── Plant_Parameters.csv       # Training dataset
├── crop_prediction_bg 1.png  # Background image
├── s1.png                    # Screenshot 1
├── s2.png                    # Screenshot 2
├── s3.png                    # Screenshot 3
├── s4.png                    # Screenshot 4
└── README.md                 # This file
```

## 🔬 How It Works

### Algorithm: K-Nearest Neighbors (KNN)
- **K-value**: 10 neighbors
- **Training Split**: 20% training, 80% testing
- **Data Processing**: Features are normalized using standard scaling
- **Prediction**: Based on similarity to k-nearest training samples

### Workflow:
1. **Data Loading**: Reads plant parameters from CSV
2. **Preprocessing**: Normalizes features and encodes plant types
3. **Model Training**: Trains KNN classifier on soil parameters
4. **Prediction**: Takes user input and predicts suitable crop
5. **Display**: Shows prediction with color-coded feedback

### Key Functions:
- `Normalise(X)`: Data normalization
- `getPredictions(datalist)`: Generate crop predictions
- `display_data()`: Process input and show results

## 📈 Model Performance

- **Algorithm**: K-Nearest Neighbors
- **Test Size**: 80% of data used for testing
- **Features**: 9 soil parameter inputs
- **Output**: Plant type classification
- **Validation**: Built-in input validation for data integrity

## 🚧 Future Enhancements

- Add more plant types to the dataset
- Implement additional ML algorithms for comparison
- Include seasonal recommendations
- Add data visualization features
- Implement database connectivity for larger datasets
- Add export functionality for predictions

## 📝 License

This project is developed for educational and research purposes.

---

**Note**: Make sure all required files are in the same directory as the main application file for proper functionality.
