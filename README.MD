# Q-SYS User Components Repository

This repository contains custom Q-SYS User Components (`.quc` files) designed to extend the functionality of Q-SYS Designer. Each `.quc` file provides unique features and capabilities to enhance your Q-SYS system design.

## Table of Contents

- [Components Overview](#components-overview)
- [How to Use](#how-to-use)
- [License](#license)

---

## Components Overview

### APIs

#### 1. **Divoom Pixoo64 Cloud API Control V1.1.quc**

- **Description**: This script gives the user the ability to control a Pixoo64 Pixel wall from a Q-SYS core. Includes automatic device discovery for all devices on the same subnet.
- **Usage**: Place this block into your design.

<!-- ### Audio Components

#### 1. **ComponentName1.quc**
- **Description**: Briefly describe what this component does.
- **Usage**: Explain how to integrate and configure this component in Q-SYS Designer.

*(Add additional components from the "Audio" folder here.)*

--- -->

### Scripting Components

#### 1. **POE Load Calculator v1.1.quc**

- **Description**: This script calculates the Peak PoE load of the design file based on all of the PoE enabled Q-SYS devices in the design.
- **Usage**: Place this block into your design.Emulate or run the design to view the cumulative load.

#### 2. **World Clock Display.quc**

- **Description**: Automatic Scrolling text box to display multiple times in a single UCI element. Allows for selecting specific cities around the world. Automatically tracks DST and time offsets based on on-board Core real-time clock. 
- **Usage**: In Emulate, configure "number of clocks", "clock choices", and "rotation speed". Add "Marquee" element to UCI, and size to taste.

#### 3. **UCI Discovery Tool.quc**

- **Description**: Discover all UCIs attached to the design. This data shows up in a Combo Box on the Text Controller, but the code can be repurposed as a code snippet inside larger code that requires access to the UCI list. **This component requires at least one UCI capable device to be set to Dynamic UCI in the properties tab**
- **Usage**: Set one Touch Panel, UCI Viewer, or MTR component to "Dynamic UCI" in the properties in Design Time. Then, in Emulate, view the UCIs in the Text Controller panel.

#### 4. **Control Script Manager.quc**

- **Description**: Real-Time monitoring and control of any and all Code Access enabled scripts inside of a design. This block gives you access to the current status and memory usage of a script, and gives you the ability to start and stop those scripts remotely. Pair with a status combiner and reflect monitoring proxy to supercharge this block.
- **Usage**: In Design time, set number of controls for each control to how many scripts you would like to monitor. In Emulate, select which scripts you would like to monitor from the drop down list. Selecting "-- DO NOT USE --" disables a row of controls, allowing you to separate out scripts for organizational purposes. 


<!-- *(Add additional components from the "Scripting" folder here.)* -->
### Logic Gates

- **Description**: These are prebuilt logic functions that can be added to the design to quickly create basic logic components.
    - **[1-Of-N].quc**
    - **[AND].quc**
    - **[NAND].quc**
    - **[NOR].quc**
    - **[NOT XOR].quc**
    - **[NOT].quc**
    - **[OR].quc**
    - **[Trigger Combiner].quc**
    - **[XOR].quc**

---

## How to Use

1. **Download the Components**: Fork or Clone this repository to your local machine.
2. **Import into Q-SYS Designer**:
    - Open Q-SYS Designer.
    - Navigate to the "User Components" section.
    - Import the desired `.quc` file(s) from this repository.
3. **Configure the Components**:
    - Drag and drop the imported component into your design.
    - Follow the usage instructions provided in the [Components Overview](#components-overview) section.
4. **Deploy**: Save and deploy your design to the Q-SYS Core processor.
5. **Contribute!**: Make a pull request and add some of your own components to share.

---

## License

Copyright 2025 QSC, LLC

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

---

Feel free to contribute to this repository by submitting pull requests or reporting issues.
