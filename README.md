# Geolocation Project- Task3

Watch the working video of the application from the drive link: https://drive.google.com/file/d/1Mv3SzrS18Ds-QyhSnc6-uhdhscaHAQ_u/view?usp=sharing

## Overview

This Android Geolocation project is designed to track and display the user's current location in real time. The application uses the device’s GPS capabilities to fetch the latitude, longitude, and accuracy, and it integrates Google APIs for enhanced functionality. The app features an intuitive user interface that provides the user with clear location data and control buttons.

## Features

- **Real-time Location Tracking:** The app tracks and displays the user’s current geographic coordinates (latitude and longitude).
- **Location Accuracy:** Shows the accuracy of the location, indicating how precise the GPS data is.
- **Google API Integration:** Utilizes Google Play Services for accurate geolocation data.
- **Control Buttons:** Provides buttons to start and stop location updates.
- **Dynamic UI Updates:** The app dynamically updates the UI with the latest location data.
- **Permissions Handling:** Requests necessary permissions (ACCESS_FINE_LOCATION and ACCESS_COARSE_LOCATION) dynamically.

## User Interface

The app’s user interface is built using a `LinearLayout` to organize the components in a vertical stack. The layout includes:

- **TextViews:** Display real-time information about the current latitude, longitude, and location accuracy.
- **Buttons:** Allow the user to start and stop location updates.

These elements are updated in real time to reflect the user’s current location data.

## Google API Integration

This app uses **Google Play Services** for accessing the device’s geolocation APIs, ensuring accurate and efficient location tracking.

### Google Play Services Location API

- **FusedLocationProviderClient:** This client is used to get the most recent location of the user with high accuracy. It combines data from various sensors (like GPS, Wi-Fi, and cell networks) to provide a more accurate result.

  ```java
  FusedLocationProviderClient fusedLocationClient = LocationServices.getFusedLocationProviderClient(this);
