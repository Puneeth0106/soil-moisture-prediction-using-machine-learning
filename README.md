# Soil Moisture Prediction Using Machine Learning

Efficient water management is a cornerstone of precision farming. This project utilizes machine learning techniques to predict soil moisture levels, enabling smarter irrigation strategies and reducing dependency on sensors.

## Key Features
- **Soil Moisture Prediction**: Predict moisture levels at unsensed points using data from a small number of sensors.
- **Simulation**: Model moisture behavior over time and distance.
- **Irrigation Planning**: Enable smarter and real-time irrigation strategies.

## How It Works

### Model-1
- **Purpose**: Predicts moisture levels at fixed distances (2.5 and 3.0 units).
- **Algorithm**: Voting Regressor combining Decision Tree, Random Forest, and XGBoost.
- **Performance**: Achieves high accuracy with R-squared scores > 0.99 in most scenarios.

### Model-2
- **Purpose**: Dynamically predicts moisture levels at any user-specified distance.
- **Algorithm**: Random Forest Regressor trained on features like time, initial center moisture, and distance.
- **Capabilities**: Simulates moisture absorption and evaporation over time.

### Simulation
- **Visualization**: Displays moisture trends at the center, two sensor points, or user-defined distances.
- **Inputs**: Time and initial center moisture levels.

## Technologies Used
- **Programming**: Python
- **Libraries**: Scikit-learn, XGBoost, Pandas, NumPy
- **Visualization**: Matplotlib

## Repository Structure
```plaintext
.
├── soil_moisture_summary.md  # Detailed project documentation
├── README.md                 # Project overview and instructions
├── scripts/                  # Python scripts for data preprocessing and modeling
├── plots/                    # Visualizations of predictions and simulations
└── data/                     # Dataset used for training and testing
```

## Getting Started

### Prerequisites
- Python 3.7 or later
- Required Python libraries:
  ```bash
  pip install -r requirements.txt
  ```

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/soil-moisture-prediction.git
   ```
2. Navigate to the project directory:
   ```bash
   cd soil-moisture-prediction
   ```
3. Install the required libraries:
   ```bash
   pip install -r requirements.txt
   ```

### Usage
1. Run the preprocessing and modeling scripts:
   ```bash
   python scripts/preprocess_data.py
   python scripts/train_model.py
   ```
2. Generate predictions or simulate moisture behavior:
   ```bash
   python scripts/predict_moisture.py
   ```
3. Visualize results:
   Check the `plots/` directory for generated visualizations.

## Contributing
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add your message here"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/your-feature-name
   ```
5. Open a pull request.

## License
This project is licensed under the MIT License. See the `LICENSE` file for details.

---

For more details, refer to the `soil_moisture_summary.md` file.
