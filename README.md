# Linear Kalman Filter Project

## Table of Contents
- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
- [Implementation Details](#implementation-details)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction
This project implements a Linear Kalman Filter to estimate the state of a dynamic system from noisy measurements. The Kalman Filter is widely used in control systems, navigation, and robotics for estimating hidden states in linear systems.

## Project Overview
The project uses a dataset of noisy measurements and applies the Kalman Filter algorithm to predict and update the state estimates based on the observed data. The implementation includes both the prediction and update steps of the Kalman Filter.

## Getting Started

### Prerequisites
- Python 3.6 or higher
- Necessary Python libraries:
  - NumPy
  - Pandas
  - Matplotlib

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/kalman-filter-project.git
 
2. Install the required libraries:
   ```bash
   pip install - requirements.txt

## Usage
1. Place your dataset (`dataset.csv`) in the project directory.
2. Open the Jupyter Notebook `Kalman_filter.ipynb`.
3. Run the cells sequentially to execute the Kalman Filter implementation.
4. Adjust the parameters of the Kalman Filter as needed to optimize the state estimates.

## Implementation Details
The implementation consists of the following key components:
- **Data Loading**: Load and preprocess the dataset to extract relevant measurements and control inputs.
- **Kalman Filter Functions**:
  - `kalman_predict(A, B, x, P, u, Q)`: Implements the prediction step of the Kalman Filter.
  - `kalman_update(x_pred, P_pred, z, H, R)`: Implements the update step to correct the predictions based on measurements.
- **Main Loop**: Iterates over the time steps, applying the prediction and update steps for each measurement.
- **Visualization**: Plots the estimated states against the noisy measurements to assess the performance of the filter.

## Results
The results of the Kalman Filter implementation are visualized through a plot comparing the estimated states (positions) with the noisy measurements. The estimated states should ideally converge closely to the true states, demonstrating the effectiveness of the Kalman Filter.

## Contributing
Contributions are welcome! Please feel free to submit a pull request or open an issue for any suggestions or improvements.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
