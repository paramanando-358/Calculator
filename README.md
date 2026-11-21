# Android Calculator App

A simple Android Calculator application developed using Java and XML in Android Studio. The application features a calculator interface designed using LinearLayout with basic arithmetic operations.

## Features

- Clean and simple calculator interface
- Addition (+)
- Subtraction (-)
- Multiplication (×)
- Division (÷)
- Decimal number support
- Delete button to remove the last entered character
- Automatic calculation with operator precedence
- Error handling for invalid expressions and division by zero

## Technologies Used

| Technology | Purpose |
|---|---|
| Java | Application logic |
| XML | User interface design |
| LinearLayout | UI layout structure |
| Android Studio | Development environment |
| Gradle | Project build system |

## UI Preview

The following screenshot shows the calculator interface and its layout structure in Android Studio.

![Calculator UI Preview](screenshots/calculator-ui.png)

## Development Process

### 1. Static UI Design

The initial calculator interface was created using Android XML and LinearLayout.

The layout includes:
- A TextView for displaying expressions and results.
- A DELETE button.
- Four columns of calculator buttons.
- Separate rows for numbers and arithmetic operators.

### 2. UI Alignment Issue and Solution

During UI development, an alignment issue occurred between the DELETE button and the division (÷) button.

**Problem:**
The DELETE button was not properly aligned with the fourth column of the calculator.

**Solution:**
- Divided the DELETE row into four equal-weight columns.
- Used three empty View elements and one DELETE button.
- Applied consistent `layout_weight="1"` values.
- Maintained consistent margins across the rows.

This resolved the horizontal alignment issue.

### 3. Java Functionality

Java was used to implement the calculator's functionality, including number input, arithmetic operations, decimal input, deletion, and result calculation.

## Project Structure

```text
Calculator/
├── app/
│   └── src/
│       └── main/
│           ├── java/
│           │   └── MainActivity.java
│           ├── res/
│           │   └── layout/
│           │       └── activity_main.xml
│           └── AndroidManifest.xml
├── gradle/
├── screenshots/
│   └── calculator-ui.png
├── .gitignore
├── build.gradle.kts
├── gradle.properties
├── gradlew
├── gradlew.bat
└── settings.gradle.kts
```

## Getting Started

### Prerequisites

- Android Studio
- Java Development Kit (JDK)
- Android Emulator or Physical Android Device

### Installation

1. Clone the repository:

```bash
git clone https://github.com/paramanando-358/Calculator.git
```

2. Open the project in Android Studio.
3. Wait for Gradle synchronization to complete.
4. Connect an Android device or start an emulator.
5. Click the Run button to launch the application.

## Developer

**GitHub:** [paramanando-358](https://github.com/paramanando-358)

**Project:** [Android Calculator](https://github.com/paramanando-358/Calculator)

---

*Developed as an Android development learning project.*
