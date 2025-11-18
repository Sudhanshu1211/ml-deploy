# WellPredict ML-Deploy

A Flask web app that predicts water quality suitability for well-digging using a trained machine learning model.

## Features
- Simple web form for user input
- Predicts if water quality is suitable for well-digging
- Uses a pre-trained scikit-learn model (`mahatva3.pkl`)

## Requirements
- Python 3.9+
- Flask
- pandas
- numpy
- scikit-learn (ideally same version as used for training the model)

## Setup & Usage

1. **Clone or Download** this repository.
2. **Open a terminal** in the `ml-deploy` folder.
3. **Create and activate a virtual environment:**
    ```bash
    python -m venv venv
    venv\Scripts\activate  # On Windows
    # source venv/bin/activate  # On macOS/Linux
    ```
4. **Install dependencies:**
    ```bash
    pip install flask pandas scikit-learn numpy
    ```
5. **Run the app:**
    ```bash
    python app.py
    ```
6. **Open your browser:**
    Go to [http://127.0.0.1:5000/](http://127.0.0.1:5000/)

## Input Parameters
- LATITUDE
- LONGITUDE
- pH
- HCO3
- Cl
- SO4
- NO3
- Total Hardness (TH)
- Ca
- Mg
- Na
- K
- F
- SiO2

## Notes
- If you see version warnings, try to match the scikit-learn version to the one used to train `mahatva3.pkl`.
- For best results, retrain the model in your local environment if possible.

## License
MIT
