# PCL1001 – AutoEasy Platform

**PCL-1001 with AutoEasy** is a low-cost programmable platform based on the **PIC16F648A** microcontroller, designed for applications in industrial automation, educational robotics, and rapid prototyping.

This repository contains the firmware developed in Assembly for the microcontroller, the **AutoEasy IDE and compiler** implemented in Visual Basic, documentation, and example programs used to validate the system.

## 📌 Overview

The PCL-1001 integrates dedicated hardware with an interpreted firmware architecture, allowing user programs to be written in a high-level domain-specific language called **AutoEasy**. Programs are compiled into proprietary bytecodes and stored in an external EEPROM memory via serial communication, eliminating the need to reprogram the microcontroller for each application update.

A virtual machine implemented in Assembly executes the bytecodes using a fetch–decode–execute cycle, enabling flexibility, reusability, and rapid iteration, especially in educational and experimental environments.

Main features include:

- Six dry-contact digital inputs  
- Digital outputs for relay control  
- 16×2 alphanumeric LCD display  
- Analog-to-digital and digital-to-analog conversion  
- Full-duplex RS-232 serial communication  
- PWM signal generation  
- Bytecode-based virtual machine architecture  

## 📂 Repository Structure

- **PIC/** – Assembly firmware source code for the PIC16F648A  
- **VB/** – AutoEasy IDE and compiler source code (Visual Basic)  
- **Manual/** – Language reference and system documentation  
- **Tests/** – Example AutoEasy programs used for validation  
- **Install/** – Installation notes and dependencies  

## 📝 Requirements

To build and use this project, the following tools and hardware are required:

- **MPLAB IDE with MPASM** (for firmware compilation)  
- **Visual Basic 6.0 or compatible Visual Studio environment** (for AutoEasy IDE)  
- RS-232 cable or USB-to-RS232 adapter  
- Assembled PCL-1001 hardware platform  

## 🚀 Getting Started

### 💾 Firmware Compilation

1. Open the firmware project in **MPLAB IDE**.  
2. Select **PIC16F648A** as the target device.  
3. Assemble the source code and generate the HEX file.  
4. Program the microcontroller using a compatible programmer (e.g., PICkit).

### 🛠️ AutoEasy IDE

1. Open the AutoEasy project in Visual Basic / Visual Studio.  
2. Build the IDE executable.  
3. Write user programs using the AutoEasy language (`.lpa` files).  
4. Compile the program to generate bytecodes.  
5. Upload the bytecodes to the external EEPROM via serial communication.

### 🧪 Example Applications

The **Tests/** directory contains example programs demonstrating:

- Traffic light control with programmable timing  
- Digital input reading and LCD display  
- Sequential digital output activation  
- PWM-based DC motor control  
- Serial data transmission and reception  

## 📚 Documentation

Detailed documentation, including the AutoEasy language reference, supported commands, and usage examples, is available in the **Manual/** directory. The documentation explains how high-level instructions are translated into bytecodes and executed by the firmware virtual machine.

## 🧑‍🔧 Contributing

Contributions are welcome and encouraged. Possible contributions include:

- New AutoEasy example programs  
- Extensions to the AutoEasy instruction set  
- Improvements to the compiler or IDE  
- Debugging or simulation tools  
- Documentation enhancements  

Please feel free to open **issues** or submit **pull requests**.

## ⚖️ License

This project is distributed under an open-source license (MIT or compatible). Please add or verify the `LICENSE` file according to your preferred licensing model.

## 🙌 Acknowledgments

This project was developed to support low-cost automation and embedded systems education, aiming to reduce technical and economic barriers to learning and experimentation with programmable controllers.
