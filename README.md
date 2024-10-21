# Tic-Tac-Toe Android App

An aesthetically pleasing Tic-Tac-Toe game for Android, built with Kotlin. This application allows users to play a classic Tic-Tac-Toe game against each other. The game maintains a record of the outcomes of the last five games, displaying the results on a dedicated results activity page.


![image](https://github.com/user-attachments/assets/f0156844-5ca8-4fd3-8764-a257d931d422) ![image](https://github.com/user-attachments/assets/7ac7e6a6-41b0-4d3a-aa19-5029da73b4b1)


![image](https://github.com/user-attachments/assets/e172301f-55f8-40a6-a2c3-cab970fe42b5)


## Table of Contents

- [Features](#features)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Usage](#usage)
  - [Playing the Game](#playing-the-game)
  - [Viewing Results](#viewing-results)
- [App Architecture](#app-architecture)
- [Customization](#customization)
- [Contributing](#contributing)
- [License](#license)

## Features

- **Classic Gameplay**: Experience the traditional Tic-Tac-Toe game with a modern interface.
- **Aesthetic Design**: Designed with a focus on aesthetics to deliver a pleasant user experience.
- **Results Tracking**: Displays the outcomes of the last five games in a results activity page.
- **Multiplayer Support**: Allows two players to take turns playing against each other.
- **Responsive Design**: Optimized for different screen sizes and orientations.

## Getting Started

### Prerequisites

To build and run the Tic-Tac-Toe Android app, you need:

- [Android Studio](https://developer.android.com/studio) (version 4.0 or later)
- Android device or emulator running Android 5.0 (Lollipop) or higher

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/tictactoe-android-app.git
   cd tictactoe-android-app
## Open the Project in Android Studio

1. **Launch Android Studio** and select **Open an existing project**.
2. **Navigate** to the directory where the project was cloned and open it.

## Build the Project

1. **Allow Android Studio** to download all necessary dependencies.
2. **Click on Run** or use `Shift + F10` to build and deploy the app on your device or emulator.

## Usage

### Playing the Game

1. **Launch the app** on your Android device.
2. The **game board** will be displayed, showing a **3x3 grid**.
3. **Player 1 (X)** starts the game, followed by **Player 2 (O)**.
4. Players **take turns** tapping on an empty cell to place their mark.
5. The game **automatically checks** for a win or a draw after each turn.
6. Once the game ends, the **outcome is saved** and displayed in the **results page**.

### Viewing Results

- The **results activity** shows the outcomes of the **last five games**, indicating whether **Player 1 won**, **Player 2 won**, or if there was a **draw**.
- **Results are updated** after each game, with the **oldest result being removed** when the list exceeds five games.

## App Architecture

The app follows the **Model-View-ViewModel (MVVM)** architecture pattern, ensuring **separation of concerns** and maintainability:

- **Model**: Represents the game's logic, including player turns, win conditions, and results tracking.
- **View**: Composed of XML layouts for the main game screen and the results screen.
- **ViewModel**: Acts as an intermediary between the Model and the View, handling user inputs and updating the UI accordingly.

### Package Structure

com.example.tictactoe ├── model │ ├── Game.kt │ ├── Player.kt ├── view │ ├── MainActivity.kt │ ├── ResultsActivity.kt │ ├── activity_main.xml │ ├── activity_results.xml ├── viewmodel │ ├── GameViewModel.kt │ ├── ResultsViewModel.kt └── utils ├── Constants.kt


- **model**: Contains data classes for game logic and player representation.
- **view**: Includes activity classes and XML layouts for the user interface.
- **viewmodel**: Manages the UI-related data in a lifecycle-conscious way.
- **utils**: Utility classes for shared constants and functions.

## Customization

You can customize various aspects of the app, such as:

- **Theme and Colors**: Modify the app's colors in `res/values/colors.xml` to match your desired aesthetic.
- **Icons and Images**: Update the icons and images in the `res/drawable` folder to personalize the look.
- **Game Rules**: Adjust the win conditions or add new features like score tracking across multiple sessions in `Game.kt`.

## Contributing

We welcome contributions to enhance the Tic-Tac-Toe app. Here’s how you can contribute:

1. **Fork the repository**.
2. **Create a new branch**:
   ```bash
    git checkout -b feature-branch
    git commit -m 'Add new feature'
    git push origin feature-branch
    This formatting follows the typical structure of a GitHub README, with clear sections, bullet points, and code formatting for commands. Let me know if you need any further modifications!




