# GPS Spoofing Detection in Vehicles
This project simulates the movement of vehicles and introduces potential GPS spoofing. It uses a Random Forest classifier to detect spoofing based on the vehicle's speed, direction, altitude, and satellite visibility.

## Overview
- **Vehicle Simulation:** Each vehicle is initialized with random speed, direction, altitude, and satellite visibility. Movement is simulated with environmental noise and randomness.
- **GPS Spoofing:** Randomly introduced to simulate an attack, affecting speed, direction, altitude, and satellite visibility.
- **Data Generation:** Simulated data for multiple vehicles over a number of steps.
- **Model Training:** A Random Forest classifier is trained to detect spoofing.
- **Visualization:** The results are visualized to show the model's predictions.

## Requirements
- Python 3.6+
- NumPy
- Matplotlib
- Scikit-learn

## Code Overview
### Vehicle Class
- **Vehicle:** Simulates vehicle movements and potential GPS spoofing.
- **simulate_movement(step):** Simulates movement with randomness and environmental noise.
- **introduce_spoofing(step):** Introduces GPS spoofing with a certain probability.
### Data Generation
- **generate_vehicle_data(vehicle, steps):** Generates simulated data for a single vehicle over a number of steps.
- **create_dataset(num_vehicles, steps_per_vehicle):** Creates a dataset for multiple vehicles.
### Model Training
- **train_model(X, y):** Trains a Random Forest model to detect spoofing and evaluates its accuracy.
### Visualization
- **visualize_results(X, y_real, y_pred):** Visualizes the model's prediction results.
### Example Output
The script prints the simulated vehicle state at each step and indicates when spoofing is detected. The accuracy of the model is printed, and a visualization of the results is displayed.

## License
This project is licensed under the MIT License.

