# iris-flower-classification
Machine Learning project using Weka to classify iris flowers with 96% accuracy. No-code ML for botanical garden visitor app.


# Dataset

## Iris Dataset (iris.arff)

**Source:** UCI Machine Learning Repository  
**Original Author:** R.A. Fisher (1936)  
**Format:** ARFF (Weka format)

### Contents:
- 150 instances (50 per class)
- 4 numeric features + 1 class label
- No missing values
- Perfectly balanced classes

### Features:
1. Sepal Length (cm)
2. Sepal Width (cm)
3. Petal Length (cm)
4. Petal Width (cm)
5. Class (Setosa, Versicolor, Virginica)

### Usage:
Load this file in Weka Explorer:
`Preprocess → Open file → iris.arff`





# Trained Models

## iris_j48_model.model

**Algorithm:** J48 Decision Tree (C4.5)  
**Accuracy:** 96.0%  
**Training:** 10-fold cross-validation  
**Features:** All 4 measurements (full model)

### Configuration:
- Confidence factor: 0.25
- Min instances per leaf: 2
- Pruning: Enabled

### How to Use:
1. Open Weka Explorer
2. Load iris.arff
3. Classify tab → Right-click → Load model
4. Select this model
5. Re-evaluate on test set

### Performance:
- Setosa: 98% accuracy
- Versicolor: 94% accuracy
- Virginica: 96% accuracy




# Source Code

## iris_prototype.html

Interactive web-based prototype for iris flower identification.

### Features:
- 2-field input (petal length & width)
- Instant classification (<100ms)
- Mobile-responsive design
- No server required

### How to Use:
1. Open `iris_prototype.html` in any modern browser
2. Enter petal measurements in cm
3. Click "Identify Flower"

### Test Inputs:
- **Setosa:** Length=1.4, Width=0.2
- **Versicolor:** Length=4.5, Width=1.3
- **Virginica:** Length=5.5, Width=2.0

### Technology:
- HTML5
- CSS3 (responsive design)
- Vanilla JavaScript (no dependencies)
