# SwiftGeographicLib 🌍

![SwiftGeographicLib](https://img.shields.io/badge/SwiftGeographicLib-v1.0.0-blue.svg)
[![Releases](https://img.shields.io/badge/Releases-latest-orange.svg)](https://github.com/MartinMira24/SwiftGeographicLib/releases)

---

## Overview

Welcome to **SwiftGeographicLib**, a Swift wrapper for geodesic routines from Charles Karney's **GeographicLib**. This library provides a clean and efficient way to perform geodesic calculations in your Swift applications. Whether you're developing for iOS with SwiftUI or UIKit, this library simplifies complex geographic computations.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **Geodesic Calculations**: Easily compute distances and angles between geographic points.
- **Swift Compatibility**: Built entirely in Swift, making it easy to integrate into your projects.
- **High Precision**: Uses proven algorithms to ensure accuracy in geodesic computations.
- **Lightweight**: Minimal dependencies, keeping your app lean and efficient.
- **Comprehensive Documentation**: Detailed guides and examples to help you get started.

## Installation

To get started with **SwiftGeographicLib**, you can download the latest release from our [Releases section](https://github.com/MartinMira24/SwiftGeographicLib/releases). Follow the instructions provided in the release notes to execute the package in your project.

### CocoaPods

If you prefer using CocoaPods, add the following line to your `Podfile`:

```ruby
pod 'SwiftGeographicLib'
```

Then run:

```bash
pod install
```

### Swift Package Manager

To integrate using Swift Package Manager, add the following dependency in your `Package.swift` file:

```swift
dependencies: [
    .package(url: "https://github.com/MartinMira24/SwiftGeographicLib.git", from: "1.0.0")
]
```

## Usage

Once you have installed **SwiftGeographicLib**, you can start using it in your Swift projects. Here’s a simple example to demonstrate its functionality.

### Importing the Library

```swift
import SwiftGeographicLib
```

### Basic Geodesic Calculation

To calculate the distance between two geographic points, use the following code:

```swift
let pointA = GeographicPoint(latitude: 34.0522, longitude: -118.2437) // Los Angeles
let pointB = GeographicPoint(latitude: 40.7128, longitude: -74.0060)   // New York

let distance = Geodesic.distance(from: pointA, to: pointB)
print("Distance: \(distance) meters")
```

## Examples

Here are a few more examples of how to use **SwiftGeographicLib** in your projects.

### Calculate Geodesic Distance

```swift
let point1 = GeographicPoint(latitude: 51.5074, longitude: -0.1278) // London
let point2 = GeographicPoint(latitude: 48.8566, longitude: 2.3522)   // Paris

let distance = Geodesic.distance(from: point1, to: point2)
print("Distance from London to Paris: \(distance) meters")
```

### Calculate Geodesic Angle

```swift
let angle = Geodesic.angle(from: point1, to: point2)
print("Angle from London to Paris: \(angle) degrees")
```

## Contributing

We welcome contributions to **SwiftGeographicLib**! If you have suggestions, improvements, or bug fixes, please follow these steps:

1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Make your changes.
4. Submit a pull request.

Your contributions help improve the library for everyone!

## License

**SwiftGeographicLib** is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or support, please feel free to reach out. You can also check our [Releases section](https://github.com/MartinMira24/SwiftGeographicLib/releases) for the latest updates and versions.

---

Thank you for choosing **SwiftGeographicLib**! We hope this library makes your geodesic calculations straightforward and efficient. Happy coding!