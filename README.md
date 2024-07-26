# Android Auto and Android Automotive Basic Navigation App

This repository contains an app for basic maps navigation and demonstrates how to connect a phone with a head unit and use the Android Automotive emulator.

## Features

- Basic maps navigation
- Integration with Android Auto
- Integration with Android Automotive OS
- Demonstrates connection setup between a phone and a head unit
- Instructions for using the Android Automotive emulator

## Requirements

- Android Studio
- Android SDK
- A physical Android device or an Android Automotive OS emulator
- Google Play Services (latest version)
- Android Auto app (latest version)
## Images
from  Android Automotive OS emulator
![Automotive pic](https://github.com/user-attachments/assets/fab4abb8-c07b-43f5-be1b-cd6cd2c724c1)

from the phone and a head unit
![Screenshot (118)](https://github.com/user-attachments/assets/4bdc4a8d-5edb-49a1-98ec-c8bd17428eb9)
![Screenshot (119)](https://github.com/user-attachments/assets/dac786e8-3c42-4481-bd35-7097c37a9be9)
![Screenshot (120)](https://github.com/user-attachments/assets/b6a9db40-776c-4bce-8980-4e93cafc4f39)
![Screenshot (121)](https://github.com/user-attachments/assets/3592ca22-793d-4479-9ffa-08140d3d77ba)



## Setup Instructions

### Prerequisites

1. **Clone the repository:**
    ```sh
    git clone https://github.com/yourusername/your-repo-name.git
    cd your-repo-name
    ```

2. **Open the project in Android Studio:**
    - Launch Android Studio.
    - Select `Open an existing Android Studio project`.
    - Navigate to the cloned repository directory and open it.

3. **Install dependencies:**
    - Android Studio will prompt you to install the necessary SDK components. Follow the instructions to install them.

### Running on Android Auto

1. **Connect your phone:**
    - Ensure your phone is compatible with Android Auto (Android 6.0 or higher).
    - Connect your phone to your computer via USB.
    - Enable Developer Options and USB Debugging on your phone.

2. **Start the Head Unit Server on your phone:**
    - Go to `Settings > Developer Options > Head Unit Server` and enable it.

3. **Set up ADB port forwarding:**
    ```sh
    adb forward tcp:5277 tcp:5277
    ```

4. **Run the Desktop Head Unit (DHU):**
    - Open Command Prompt.
    - Navigate to the DHU directory:
    - for me was \Users\ISLAM\AppData\Local\Android\Sdk\extras\google\auto\desktop-head-unit.exe
        ```sh
        cd %LOCALAPPDATA%\Android\Sdk\extras\google\auto
        ```
    - Run the DHU executable:
        ```sh
        desktop-head-unit.exe
        ```

5. **Run the app:**
    - In Android Studio, select your connected device and click `Run`.

### Running on Android Automotive Emulator

1. **Set up the Android Automotive OS emulator:**
    - Open Android Studio.
    - Go to `Tools > AVD Manager`.
    - Create a new Virtual Device.
    - Select a car hardware profile.
    - Choose a system image that supports Android Automotive OS.
    - Follow the configuration steps and launch the emulator.

2. **Run the app:**
    - In Android Studio, select the Android Automotive OS emulator and click `Run`.

## Usage

### Using the App

- **Basic Maps Navigation:**
    - Launch the app on your device or emulator.
    - Use the navigation features to explore basic maps functionality.

- **Connecting Phone with Head Unit:**
    - Follow the setup instructions to connect your phone with the head unit using the DHU.
    - Explore the integration with Android Auto.

- **Using the Android Automotive Emulator:**
    - Launch the emulator as described in the setup instructions.
    - Run the app and explore the features specific to Android Automotive OS.


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to the Android Developers community for their continuous support and resources as i used the code labs from google Android Developers.
- [The CodeLab](https://developer.android.com/codelabs/car-app-library-fundamentals?hl=en#0)

