**Swift-Arduino** is an Xcode framework designed to simplify Arduino control using Swift.  
Its syntax reads like plain English, making it approachable for beginners while powerful enough for advanced projects.

---

## Key Features

- Intuitive, English-like commands for Arduino pin control.  
- Automatic board connection—no manual setup required.  
- Cross-project friendly: works in any Xcode project with minimal configuration.  
- Flexible enough for advanced IoT, robotics, and electronics projects.  

---

## Installation

### Swift Package Manager
```swift
dependencies: [
    .package(url: "https://github.com/Mr-Stickman1/Swift-Arduino.git", from: "1.0.0")
]



Manual Installation

Download swiftarduino.framework.zip
.

Drag the framework into your Xcode project.

Import the module:

import SwiftArduino

Quick Start

Turn a pin on/off:

make pin "13" on
make pin "12" off


Read a digital pin:

let pinState = read pin "7"
print("Pin 7 state: \(pinState)")


Set PWM value for analog pins:

set pin "9" to 128  // 0-255


Control a servo:

move servo "10" to 90
move servo "10" to 0


Blink an LED:

repeat 5 times {
    make pin "13" on
    wait 1
    make pin "13" off
    wait 1
}

Example Projects

LED Patterns: Blink LEDs in Morse code or sequences.

Temperature Sensor: Read analog sensor values and display in Xcode console.

Servo Control: Move servos in smooth animations for robotics arms.

IoT Projects: Control Arduino from Mac for home automation.

Games & Interaction: Use buttons and sensors to create interactive mini-games.

Contributing

Contributions welcome!

Fork the repository.

Test your ideas or add new examples.

Submit pull requests with improvements, bug fixes, or new features.

Whether you are a beginner or experienced developer, your contributions help grow this framework.

License

This project is licensed under the MIT License
.

⭐ Star this repo if you find it useful and share it with other Swift developers!
