# Drug Reporting App

A Flutter app designed for anonymously reporting drug users. This app helps raise awareness and provides a secure platform for reporting drug-related activities in the community.

## Features

- **Anonymous Reporting**: Users can report drug-related activities without revealing their identity.
- **Location Data**: Each report includes the location from where the report is being submitted.
- **Photo Attachment**: Users can attach photos with their reports (optional).
- **Real-time Synchronization**: The app syncs data with the backend in real-time for accurate and timely reporting.
- **Secure Data**: Data is hashed using SHA-256 for privacy and security.

## Prerequisites

Before you begin, make sure you have the following installed:

1. **Flutter**:  
   Install Flutter by following the [official Flutter installation guide](https://flutter.dev/docs/get-started/install) for your operating system.
   
   - Flutter SDK
   - Dart SDK (comes with Flutter)

2. **Android Studio**:
   Download and install [Android Studio](https://developer.android.com/studio). This will provide the necessary SDKs and emulators for Android development.

3. **Set Up Android Emulator**:
   - Open Android Studio, go to **AVD Manager**, and create an emulator.
   - Alternatively, you can use a physical Android device connected via USB for testing.

4. **Flutter Dependencies**:
   You may need to install additional dependencies. Run this in your terminal:
   ```bash
   flutter doctor
   ```

### Setting Up the Project

1. **Clone the Repository**:
   First, clone the project repository to your local machine:
   ```bash
   git clone https://github.com/NikithaSNair/App.git
   cd App
   ```

2. **Install Flutter Dependencies**:
   Once inside the project directory, run the following to install necessary dependencies:
   ```bash
   flutter pub get
   ```

3. **Run the Application**:
   Make sure an Android emulator or a physical Android device is running. Then, execute:
   ```bash
   flutter run
   ```

   This will launch the app on your device or emulator.

### Folder Structure

The project is organized as follows:

```
/lib               # Contains the main Flutter application code
  /screens         # Different UI screens for user interaction
  /models          # Data models (e.g., Report Model)
  /services        # Services for data fetching, API calls, etc.
/assets            # Images, icons, and other media files
  /images          # Image assets like icons and screenshots
  /icons           # App-specific icons
/pubspec.yaml      # Project dependencies and configurations
README.md          # Project documentation
```

### Core Features

- **UI Screens**: The UI screens contain all the views where users can interact with the app, including reporting drug-related activities, capturing photos, and adding location data.
  
- **Models**: The app utilizes a data model for managing report data, including location and photo. You will find files that define the structures for these models.

- **Services**: A `services/` folder handles interactions with external APIs or your backend (in this case, fetching and submitting reports).

### Running the App

1. **Ensure Android Device/Emulator is Running**:
   - Open Android Studio and either start an emulator or connect a physical Android device.
   
2. **Build and Run the App**:
   - Once the setup is complete, execute:
   ```bash
   flutter run
   ```

   - This command will build the app and deploy it to your running emulator or physical device.

### App Permissions

- **Location Access**: The app will ask for permission to access the user's location to accurately submit reports based on the user's geographic location. Make sure to grant the location permission when prompted.

- **Camera Access**: Users can optionally attach images with their reports. The app will request access to the device’s camera.

### Additional Notes

- **Testing**: You can test the app using either physical devices or Android emulators. Ensure that location services are enabled for accurate testing.

- **Future Updates**: This app is currently a frontend implementation. Future versions may include more advanced features such as user authentication and blockchain-based data storage.

---

### License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---
