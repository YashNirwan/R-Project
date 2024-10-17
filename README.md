# analyzeGPS: A Package for GPS Data Analysis

`analyzeGPS` is an R package designed to perform various calculations on GPS data, including distance, velocity, acceleration, and grade between GPS points. The package is especially useful for analyzing time-series GPS data, such as that collected from GPS tracking devices, and provides key functions to help process, clean, and extract meaningful insights from such data.

## Features

- **Calculate Acceleration**: Compute the acceleration in m/s² between pairs or vectors of GPS points based on time and velocity differences.
- **Distance Calculation**: Calculate the distance in meters between GPS points using the Haversine formula, which takes the Earth's curvature into account.
- **Velocity Calculation**: Compute the speed (velocity) between GPS points based on the time and distance between them.
- **Grade Calculation**: Determine the grade (rise over distance traveled) between pairs or vectors of GPS points.
- **GPS Data Import**: Easily read GPS data from CSV files and sort them into a tidy data frame for further analysis.

## Dataset

The package includes a sample dataset `myGPSData`, containing 7,771 rows of GPS data with the following variables:

- **lon**: Longitude data
- **lat**: Latitude data
- **ele**: Elevation data
- **time**: GPS timestamp (in GMT)
- **tz_CEST**: Timestamp converted to CEST (Central European Summer Time) time zone

## Installation

You can install `analyzeGPS` directly from GitHub (after creating a repo) using `devtools`:

```R
# Install devtools if you don't have it
install.packages("devtools")

# Install analyzeGPS from GitHub
devtools::install_github("your_username/analyzeGPS")
