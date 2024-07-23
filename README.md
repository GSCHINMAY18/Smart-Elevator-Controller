# Elevator Control System with System Verilog FSM

## Introduction

Elevators are a critical component of modern urban infrastructure, transforming vertical transportation in multi-story buildings. This project focuses on implementing a System Verilog Finite State Machine (FSM) to manage an elevator control system. The system addresses complex requirements such as user floor selections, priority handling, emergency stops, and safety through limit sensors.

## Assumptions Made

To understand the elevator control system's operation, several assumptions are considered:

1. **Direction Persistence**: The elevator continues in its current direction until all requests in that direction are serviced.
   
2. **Idle State**: After fulfilling all requests at the latest destination, the elevator stops and becomes idle.
   
3. **Door Control Signal**: Arrival sensors trigger door opening for a set time upon reaching a floor, ensuring safe passenger entry and exit.

These assumptions guide the system's behavior, state transitions, and logic design, aligning with industry standards for efficiency and safety.

## Modified Priority Algorithm Implementation and Functionality

### 1. Priority Algorithm Overview

The system implements a modified priority algorithm to optimize elevator operations:

- **Proximity-Based Prioritization**: Prioritizes requests based on proximity and direction of travel.
  
- **Efficient Movement Planning**: Dynamically adjusts movement direction to optimize response to high-priority requests.
  
- **Handling Multiple Requests**: Orders requests to minimize travel distance, reducing overall energy consumption and travel time.

### 2. Emergency System Integration

- **Emergency Stop**: Includes a button for passengers to halt the elevator safely, preserving current status and direction.

## Repository Contents

- **src/**: Contains the System Verilog FSM code for the elevator control system.
  
- **testbenches/**: Includes testbenches for simulating and verifying the system's behavior.
  
- **docs/**: Additional documentation files, including this README.

## Usage

1. **Simulation**: Use a System Verilog simulator (e.g., ModelSim, Xilinx Vivado) to simulate the FSM implementation.
   
2. **Testing**: Execute testbenches provided in the `testbenches/` directory to validate system functionality against expected behaviors.

## Contributors

- [Your Name]
- [Other Contributors (if applicable)]

## License

This project is licensed under the [License Name] License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- [Mention any acknowledgments or references here]
