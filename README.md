# Simple Weather App 🌦️

A Flutter application that displays current weather information based on your location. The app utilizes **Flutter Bloc** for state management and integrates several packages like **Weather**, **Geolocator**, and **Intl** to fetch and display real-time weather data efficiently.

## Key Features

- 🌍 **Location-based Weather:** Automatically fetches and displays weather for your current location.
- 🔄 **State Management:** Powered by **Flutter Bloc**, ensuring a smooth and organized flow of data.
- 🗓️ **Internationalization:** Using **Intl** for formatted date and time display according to your locale.
- 📍 **Geolocation Services:** Leveraging **Geolocator** to get real-time location updates.

## Packages Used

- **Flutter Bloc:** For managing states and handling complex business logic in an organized way.
- **Weather:** For fetching weather data.
- **Geolocator:** For retrieving the device's current location.
- **Intl:** For formatting dates and times based on the user's locale.


## Problem/Challenges

During the development of the app, the following problems were encountered:

1. **State Management Complexity:** Managing multiple states such as loading, fetching weather data, and handling errors with Flutter Bloc initially posed a challenge. The problem was resolved by structuring the states into logical blocs and ensuring the right event is triggered based on the state.

2. **Geolocation Permission Issues:** Handling permission requests for location services was tricky, especially with different devices having different behaviors. This issue was mitigated by properly checking permissions and handling denied or restricted cases gracefully within the app.

3. **API Error Handling:** Initially, the app had difficulty gracefully managing API failures (like network errors or wrong location inputs). This was fixed by adding error states in the Bloc and showing user-friendly messages when such errors occurred.

4. **Internationalization:** Formatting the date and time according to the device’s locale required fine-tuning. By using **Intl**, we ensured consistent and accurate date-time formatting across different regions.


## Contributing

Contributions are welcome! Feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
