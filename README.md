# 🌞 Solar PV Cleaning System

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Arduino](https://img.shields.io/badge/Arduino-ESP32-00979D?logo=arduino&logoColor=white)](https://www.arduino.cc/)
[![Platform](https://img.shields.io/badge/Platform-ESP32-red)](https://www.espressif.com/en/products/socs/esp32)
[![Version](https://img.shields.io/badge/Version-1.0.0-blue)](https://github.com/HorizonHnk/solar-pv-cleaning-system)
[![Website](https://img.shields.io/badge/Website-Live-brightgreen)](https://glowing-granita-8fe486.netlify.app/)
[![YouTube](https://img.shields.io/badge/YouTube-Tutorials-red?logo=youtube)](https://www.youtube.com/playlist?list=PLrZbkNpNVSwxkeTpdWLuhH0i63HLL73QL)

> **An autonomous ESP32-based solar panel cleaning robot with WiFi control, ultrasonic sensors, and coordinated motor movement for maintaining optimal solar panel efficiency.**

## 🌐 **Project Website & Tutorials**

📱 **Live Website:** [https://glowing-granita-8fe486.netlify.app/](https://glowing-granita-8fe486.netlify.app/)

🎥 **Video Tutorials:** [YouTube Playlist - Complete Build Guide](https://www.youtube.com/playlist?list=PLrZbkNpNVSwxkeTpdWLuhH0i63HLL73QL)

---

## 📋 Table of Contents

- [🌞 Solar PV Cleaning System](#-solar-pv-cleaning-system)
  - [🌐 Project Website & Tutorials](#-project-website--tutorials)
  - [📋 Table of Contents](#-table-of-contents)
  - [✨ Features](#-features)
  - [🎥 Video Tutorial Series](#-video-tutorial-series)
  - [🛠️ Hardware Components](#️-hardware-components)
  - [🏗️ System Architecture](#️-system-architecture)
  - [📷 System Images](#-system-images)
  - [⚙️ Installation Overview](#️-installation-overview)
    - [Hardware Setup](#hardware-setup)
    - [Software Requirements](#software-requirements)
  - [🚀 Usage](#-usage)
    - [Quick Start](#quick-start)
    - [Web Interface](#web-interface)
    - [Manual Control](#manual-control)
  - [🔌 Circuit Diagram](#-circuit-diagram)
  - [📁 Project Structure](#-project-structure)
  - [🔧 Configuration](#-configuration)
  - [🐛 Troubleshooting](#-troubleshooting)
  - [🤝 Contributing](#-contributing)
  - [📄 License](#-license)
  - [👥 Authors](#-authors)
  - [🙏 Acknowledgments](#-acknowledgments)
  - [🔗 Additional Resources](#-additional-resources)

---

## ✨ Features

- **🤖 Autonomous Operation**: Fully automated cleaning cycles with obstacle detection
- **📡 WiFi Control**: Remote monitoring and control via web interface
- **🔍 Smart Navigation**: Ultrasonic sensors prevent falls and collisions
- **💧 Water Management**: Precision water spray system with automated flow control
- **⚡ Multi-Motor Coordination**: Synchronized movement and brush rotation
- **🔋 Power Management**: Multiple power rails for optimal efficiency
- **🌐 Real-time Monitoring**: Live status updates and sensor readings
- **🛡️ Safety Features**: Emergency stop and edge detection
- **📱 Mobile Friendly**: Responsive web interface for smartphone control
- **🔧 Modular Design**: Easy component replacement and upgrades

> **🌐 For detailed feature descriptions and technical specifications, visit our [complete project website](https://glowing-granita-8fe486.netlify.app/)**

---

## 🎥 Video Tutorial Series

Follow our comprehensive YouTube playlist covering every aspect of building and programming the Solar PV Cleaner:

**📺 [Complete Tutorial Playlist](https://www.youtube.com/playlist?list=PLrZbkNpNVSwxkeTpdWLuhH0i63HLL73QL)**

### **Tutorial Episodes:**
1. **Project Overview & Demonstration** - System capabilities and introduction
2. **ESP32 Arduino IDE Setup** - Programming environment configuration 
3. **Sensor Integration Tutorial** - HC-SR04 ultrasonic sensor implementation
4. **Motor Control System** - L298N driver and multi-motor coordination
5. **Water Management System** - Pump control and TIP120 transistor circuit
6. **Web Interface Development** - WiFi setup and control panel
7. **Mechanical Assembly** - Frame construction and component mounting
8. **Testing & Calibration** - Real-world performance optimization
9. **Troubleshooting Guide** - Common issues and solutions
10. **Advanced Features** - Customizations and enhancements

---

## 🛠️ Hardware Components

### **Main Controller**
| Component | Description | Function |
|-----------|-------------|----------|
| **ESP32 Development Board** | WiFi/Bluetooth microcontroller | Controls entire cleaning system, hosts web interface |
| **Arduino (Alternative)** | Basic microcontroller | Alternative controller option, less features than ESP32 |

### **Sensors**
| Component | Description | Function |
|-----------|-------------|----------|
| **HC-SR04 Ultrasonic (Forward)** | Distance sensor (2cm-400cm) | Detects obstacles and panel edges ahead |
| **HC-SR04 Ultrasonic (Backward)** | Distance sensor (2cm-400cm) | Monitors rear clearance during movement |

### **Motors & Actuators**
| Component | Description | Function |
|-----------|-------------|----------|
| **DC Gear Motor (Left)** | High-torque motor | Drives left-side movement mechanism |
| **DC Gear Motor (Right)** | High-torque motor | Drives right-side movement mechanism |
| **DC Gear Motor (Brush)** | Rotational motor | Rotates cylindrical cleaning brushes |
| **DC Gear Motor (Additional)** | Auxiliary motor | Backup movement or secondary cleaning |
| **DC Water Pump** | Electric liquid pump | Pumps cleaning water through spray nozzles |

### **Motor Control**
| Component | Description | Function |
|-----------|-------------|----------|
| **L298N Motor Driver Board** | Dual H-bridge controller | Controls speed and direction of motors |
| **TIP120 Darlington Transistor** | High-current switch | Switches water pump with isolation |
| **Arduino Relay Module** | Electronic switch | Controls high-power devices safely |
| **Flyback Diode (1N4007)** | Motor protection diode | Protects from voltage spikes |
| **Current Limiting Resistor (1kΩ)** | Current control resistor | Limits base current to transistor |

### **Power Supply**
| Component | Description | Function |
|-----------|-------------|----------|
| **5V DC Battery/Power Bank** | Low voltage power | Powers ESP32 and sensors |
| **9V DC Battery** | Medium voltage power | Intermediate voltage requirements |
| **12V DC Battery/Pack** | Motor power battery | Powers motors and pump |

### **Cleaning Mechanism**
| Component | Description | Function |
|-----------|-------------|----------|
| **Cylinder Cleaning Brushes** | Rotating brush roller | Main cleaning element |
| **Water Spray Nozzle** | Pressurized water outlet | Sprays water for cleaning |
| **Water Tap (Solenoid Valve)** | Electronic water control | Automated water flow control |
| **Water Supply Tubing** | Flexible water hose | Carries water to nozzles |
| **Water Distribution System** | Pipe network with valves | Manages water flow distribution |
| **Water Reservoir/Tank** | Water storage container | Holds cleaning water supply |

> **🛍️ For complete parts list with suppliers and pricing, visit the [hardware section](https://glowing-granita-8fe486.netlify.app/#hardware) on our website**

---

## 🏗️ System Architecture

```
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│   Web Interface │────│   ESP32 Core    │────│  Motor Control  │
│   (WiFi Access) │    │   Controller    │    │   (L298N + PWM) │
└─────────────────┘    └─────────────────┘    └─────────────────┘
                              │                        │
                              │                        ▼
┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
│ Ultrasonic      │────│   Sensor Data   │    │   DC Motors     │
│ Sensors (2x)    │    │   Processing    │    │   (4x + Pump)   │
└─────────────────┘    └─────────────────┘    └─────────────────┘
                              │
                              ▼
                    ┌─────────────────┐
                    │ Cleaning System │
                    │ (Brush + Water) │
                    └─────────────────┘
```

> **🏗️ For detailed system architecture and design principles, visit the [architecture section](https://glowing-granita-8fe486.netlify.app/#architecture) on our website**

---

## 📷 System Images

### System Overview
![Solar Cleaning System Overview](https://github.com/HorizonHnk/Solar-PV-Cleaning-System/blob/main/Block%20diagram.png?raw=true)
*Complete solar panel cleaning robot with ESP32 controller, ultrasonic sensors, and cleaning mechanisms*

### Electronic Components Layout
![Electronic Components](https://github.com/HorizonHnk/Solar-PV-Cleaning-System/blob/main/Arduino%20Components.png?raw=true)
*ESP32 development board with motor drivers, sensors, and power management circuits*

### Mechanical Structure
![Mechanical Design](https://github.com/HorizonHnk/Solar-PV-Cleaning-System/blob/main/Untitled.png?raw=true)
*Frame, rails, brushes, and water distribution system for effective panel cleaning*

### Circuit Connections
![Circuit Diagram](https://github.com/HorizonHnk/Solar-PV-Cleaning-System/blob/main/new.png?raw=true)
*Detailed wiring diagram showing ESP32 connections to motors, sensors, and pump control*

### Web Interface
![Web Control Interface](https://github.com/HorizonHnk/Solar-PV-Cleaning-System/blob/main/website.png?raw=true)
*Responsive web interface for remote monitoring and control via WiFi*

> **🖼️ View more images and interactive gallery at [glowing-granita-8fe486.netlify.app/#gallery](https://glowing-granita-8fe486.netlify.app/#gallery)**

---

## ⚙️ Installation Overview

### Hardware Setup

1. **🔌 Power System Setup**:
   - Connect 5V supply for ESP32 and sensors
   - Connect 12V supply for motors and water pump
   - Install voltage regulators for stable operation

2. **🤖 Controller Installation**:
   - Mount ESP32 development board
   - Connect to breadboard/PCB for organized wiring
   - Install heat sinks if needed for continuous operation

3. **📡 Sensor Mounting**:
   ```
   Forward Sensor:  Front edge detection
   Backward Sensor: Rear clearance monitoring
   ```

4. **⚙️ Motor System**:
   - Install 4x DC gear motors for movement and cleaning
   - Mount L298N motor driver board
   - Connect water pump with TIP120 transistor control

5. **💧 Water System**:
   - Install spray nozzles and tubing
   - Mount water reservoir/tank
   - Connect solenoid valve for automated flow control

6. **🏗️ Mechanical Assembly**:
   - Assemble frame and guide rails
   - Install cleaning brushes
   - Mount all components securely

### Software Requirements

- **Arduino IDE** with ESP32 board package
- **Required Libraries**: WiFi, WebServer, NewPing
- **Development Environment**: Compatible with Windows, macOS, Linux
- **Programming Language**: C++ (Arduino Framework)

> **📁 Note**: Complete installation guides and code are available on our [project website](https://glowing-granita-8fe486.netlify.app/#docs) and [YouTube tutorials](https://www.youtube.com/playlist?list=PLrZbkNpNVSwxkeTpdWLuhH0i63HLL73QL)

---

## 🚀 Usage

### Quick Start

1. **Power On**: Connect 5V and 12V power supplies
2. **Connect to WiFi**: 
   - Look for AP: `SolarCleaner_XXXX`
   - Password: `cleanpanel123`
   - Navigate to: `192.168.4.1`
3. **Start Cleaning**: Click "Auto Clean" in web interface

### Web Interface

The system creates a WiFi access point with a responsive web interface:

- **📊 Dashboard**: Real-time sensor readings and status
- **🎮 Manual Control**: Direct motor and pump control
- **⚙️ Settings**: Cleaning parameters and schedules
- **📈 Monitoring**: Historical data and maintenance logs

### Manual Control

> **Safety First**: Always ensure the cleaning area is clear before operation

**Emergency Stop**: Press the physical button or use web interface

**Manual Movement**:
- Forward/Backward arrows
- Speed adjustment slider
- Individual motor control

> **📱 For detailed usage instructions and interface guide, visit our [website documentation](https://glowing-granita-8fe486.netlify.app/#docs)**

---

## 🔌 Circuit Diagram

![Complete Circuit Diagram](https://github.com/HorizonHnk/Solar-PV-Cleaning-System/blob/main/new%20Untitled.png?raw=true)
*Comprehensive wiring diagram showing all connections*

### Connection Summary
- **ESP32 Controller**: Central processing and WiFi communication
- **Ultrasonic Sensors**: Distance measurement and obstacle detection
- **Motor Drivers**: Speed and direction control for movement
- **Water System**: Pump control and flow management
- **Power Management**: Multiple voltage rails and regulation

> **⚠️ Important**: Refer to the detailed circuit images and our [website circuit section](https://glowing-granita-8fe486.netlify.app/#gallery) for exact pin connections and component values

---

## 📁 Project Structure

```
solar-pv-cleaning-system/
│
├── 📁 images/
│   ├── 🖼️ system-overview.png         # Complete system photos
│   ├── 🖼️ electronics-layout.png      # Circuit board layouts
│   ├── 🖼️ mechanical-structure.png    # Frame and mechanical parts
│   ├── 🖼️ circuit-diagram.png         # Wiring diagrams
│   ├── 🖼️ web-interface.png          # Control interface screenshots
│   ├── 🖼️ esp32-pinout.png           # Controller pinout reference
│   ├── 🖼️ motor-driver-wiring.png    # Motor connections
│   └── 🖼️ power-distribution.png     # Power system layout
│
├── 📁 diagrams/
│   ├── 📊 system-architecture.svg     # System block diagram
│   ├── 📊 component-layout.svg        # Component organization
│   └── 📊 flow-diagram.svg           # Process flow charts
│
├── 📁 documentation/
│   ├── 📖 hardware-components.md      # Complete parts list
│   ├── 📖 assembly-guide.md          # Build instructions
│   ├── 📖 troubleshooting.md         # Common issues & solutions
│   └── 📖 specifications.md          # Technical specifications
│
├── 📁 3d-models/
│   ├── 🔧 frame-design.stl           # 3D printable frame parts
│   ├── 🔧 motor-mounts.stl           # Motor mounting brackets
│   └── 🔧 sensor-housing.stl         # Protective sensor cases
│
├── 📄 README.md                      # This documentation file
├── 📄 LICENSE                        # MIT License
└── 📄 HARDWARE_LIST.md               # Complete component list
```

> **📝 Note**: This repository contains project documentation, images, and design files. Source code and detailed guides are available on our [project website](https://glowing-granita-8fe486.netlify.app/) and [YouTube channel](https://www.youtube.com/playlist?list=PLrZbkNpNVSwxkeTpdWLuhH0i63HLL73QL)

---

## 🔧 Configuration

### System Parameters

**📡 WiFi Settings**
- Default SSID: `SolarCleaner_XXXX`
- Default Password: `cleanpanel123`
- Access Point Mode: Enabled by default
- Web Interface Port: 80

**⚙️ Motor Configuration**
- Motor Speed Range: 0-255 (PWM)
- Default Cleaning Speed: 150
- Safety Speed Limit: 200
- Brush Rotation: 60 RPM

**🔍 Sensor Settings**
- Obstacle Detection Distance: 15cm
- Edge Detection Distance: 5cm
- Sensor Update Frequency: 10Hz
- Maximum Range: 400cm

**💧 Water System**
- Pump Flow Rate: Adjustable via PWM
- Default Water Pressure: 50% 
- Cleaning Cycles: Configurable
- Auto-shutoff Timer: 30 minutes

### Customization Options

- **Cleaning Patterns**: Horizontal, vertical, or custom paths
- **Speed Profiles**: Gentle, normal, or intensive cleaning
- **Water Usage**: Conservation mode or thorough cleaning
- **Safety Margins**: Adjustable edge detection sensitivity
- **Scheduling**: Automatic cleaning cycles (future feature)

> **📋 Complete configuration guide**: Visit our [technical specifications](https://glowing-granita-8fe486.netlify.app/#specifications) page for detailed parameter explanations

---

## 🐛 Troubleshooting

### Common Issues

**❌ ESP32 Connection Problems**
- ✅ Check WiFi credentials and network settings
- ✅ Verify power supply stability (5V)
- ✅ Reset ESP32 and reconnect
- ✅ Check antenna positioning

**❌ Motor Operation Issues**
- ✅ Verify 12V power supply for motors
- ✅ Check L298N driver board connections
- ✅ Inspect motor wiring and terminals
- ✅ Test individual motors separately

**❌ Sensor Reading Errors**
- ✅ Ensure proper 5V power to sensors
- ✅ Check trigger and echo pin connections
- ✅ Verify sensor mounting and alignment
- ✅ Test in open area without obstacles

**❌ Water System Malfunction**
- ✅ Check water pump power connections
- ✅ Verify TIP120 transistor wiring
- ✅ Inspect tubing for blockages
- ✅ Test pump operation manually

**❌ Web Interface Not Loading**
- ✅ Confirm ESP32 access point is active
- ✅ Check device connection to WiFi network
- ✅ Try accessing via IP address directly
- ✅ Clear browser cache and cookies

### Performance Optimization

- **🔋 Power Management**: Use efficient power supplies and check voltage levels
- **🌐 WiFi Range**: Position ESP32 for optimal signal strength
- **⚙️ Mechanical Maintenance**: Regular cleaning of brushes and rails
- **💧 Water Quality**: Use clean water to prevent nozzle blockages
- **🔧 Component Check**: Periodic inspection of all connections

### Support Resources

- 📖 [Complete troubleshooting guide](https://glowing-granita-8fe486.netlify.app/#docs)
- 🎥 [Video troubleshooting tutorials](https://www.youtube.com/playlist?list=PLrZbkNpNVSwxkeTpdWLuhH0i63HLL73QL)
- 🖼️ Reference circuit diagrams in `/images` folder
- 🔧 Review 3D models for mechanical issues
- 📧 Contact support for additional assistance

---

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. **🍴 Fork** the repository from [github.com/HorizonHnk/solar-pv-cleaning-system](https://github.com/HorizonHnk/solar-pv-cleaning-system)
2. **🌿 Create** a feature branch (`git checkout -b feature/amazing-feature`)
3. **💾 Commit** your changes (`git commit -m 'Add amazing feature'`)
4. **📤 Push** to the branch (`git push origin feature/amazing-feature`)
5. **🔀 Open** a Pull Request

### Contribution Guidelines

- 📸 Include high-quality images for hardware modifications
- 📝 Update documentation for design changes
- 🔍 Provide detailed descriptions of improvements
- 📐 Include accurate measurements and specifications
- ⚡ Focus on efficiency and reliability improvements
- 🧪 Test all hardware changes thoroughly

### Areas for Contribution

- **📷 Photography**: Better system images and documentation photos
- **🎨 3D Modeling**: Improved mechanical parts and enclosures
- **📖 Documentation**: Enhanced assembly guides and tutorials
- **⚙️ Hardware Design**: Component optimization and cost reduction
- **🔧 Mechanical Engineering**: Structural improvements and efficiency
- **💡 Feature Ideas**: New functionality and system enhancements

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

```
MIT License

Copyright (c) 2025 Solar PV Cleaning Project

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software...
```

---

## 👥 Authors

- **HorizonHnk** - *Project Creator & Lead Developer* - [@HorizonHnk](https://github.com/HorizonHnk)
- **Contributors Welcome** - *Join the project* - [Contributors](https://github.com/HorizonHnk/solar-pv-cleaning-system/contributors)

See also the list of [contributors](https://github.com/HorizonHnk/solar-pv-cleaning-system/contributors) who participated in this project.

---

## 🙏 Acknowledgments

- **🏗️ Espressif Systems** for the amazing ESP32 platform
- **🤖 Arduino Community** for extensive libraries and support
- **🔧 DIY Electronics Community** for hardware inspiration
- **🌞 Solar Industry** for highlighting the need for automated cleaning
- **📚 Open Source Contributors** worldwide

---

## 🔗 Additional Resources

### **🌐 Project Links**
- **📱 Complete Project Website**: [https://glowing-granita-8fe486.netlify.app/](https://glowing-granita-8fe486.netlify.app/)
- **🎥 Video Tutorial Series**: [YouTube Playlist](https://www.youtube.com/playlist?list=PLrZbkNpNVSwxkeTpdWLuhH0i63HLL73QL)
- **📁 GitHub Repository**: [Solar PV Cleaning System](https://github.com/HorizonHnk/solar-pv-cleaning-system)

### **📞 Support & Contact**
- **📧 Email**: hhnk3693@gmail.com
- **🐛 Issues**: [GitHub Issues](https://github.com/HorizonHnk/solar-pv-cleaning-system/issues)
- **📖 Wiki**: [Project Wiki](https://github.com/HorizonHnk/solar-pv-cleaning-system/wiki)
- **💬 Discussions**: [GitHub Discussions](https://github.com/HorizonHnk/solar-pv-cleaning-system/discussions)

### **📚 Documentation Sections**
- [Introduction & Overview](https://glowing-granita-8fe486.netlify.app/#introduction)
- [Complete Feature List](https://glowing-granita-8fe486.netlify.app/#features)
- [System Architecture](https://glowing-granita-8fe486.netlify.app/#architecture)
- [Hardware Components](https://glowing-granita-8fe486.netlify.app/#hardware)
- [Project Gallery](https://glowing-granita-8fe486.netlify.app/#gallery)
- [Technical Specifications](https://glowing-granita-8fe486.netlify.app/#specifications)
- [Documentation & Guides](https://glowing-granita-8fe486.netlify.app/#docs)

---

### 🌟 Star this repository if you found it helpful!

**Made with ❤️ for cleaner, more efficient solar panels**

---

> **⚠️ Safety Notice**: This project involves electrical components and water. Always follow proper safety procedures, disconnect power when making connections, and test in a safe environment before deployment. For detailed safety guidelines, visit our [website documentation](https://glowing-granita-8fe486.netlify.app/#docs).

---

**🚀 Ready to build your own Solar PV Cleaner? Start with our [complete tutorial series](https://www.youtube.com/playlist?list=PLrZbkNpNVSwxkeTpdWLuhH0i63HLL73QL) and visit our [project website](https://glowing-granita-8fe486.netlify.app/) for comprehensive guides!**
