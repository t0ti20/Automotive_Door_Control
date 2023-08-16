# Automotive Door Control System 🚗

In the realm of the automotive industry, Electronic Control Units (ECUs) play a vital role in enhancing safety and ensuring driver comfort. ECUs comprise microcontrollers that interface with both input and output devices. The input devices sense the environmental conditions, while the output devices take actions based on these sensed inputs.

![Automotive_Door_Control_1](https://github.com/t0ti20/Automotive_Door_Control/assets/61616031/a6cc2eb7-f374-4682-9c48-369cdbbde1d5)


## Project Overview 🌟

This project involves the design and implementation of two ECUs that communicate to control car lights based on door state, light switch state, and car speed.

### Main Tasks:

1. **Fully Static Design**
   - Static Design Analysis
2. **Fully Dynamic Design**
   - Dynamic Design Analysis

## Hardware Requirements 🔩

- **Two microcontrollers** connected via CAN bus.
- **Input Devices**:
  - Door Sensor (D)
  - Light Switch (L)
  - Speed Sensor (S)
  - ECU 1 interfaces with D, S, and L.
- **Output Devices**:
  - Right Light (RL)
  - Left Light (LL)
  - Buzzer (B)
  - ECU 2 interfaces with RL, LL, and B.

## Software Requirements 💾

- Periodic status messages from ECU 1 to ECU 2 via the CAN protocol using the Basic Communication Module (BCM):
  - Door state message: Every 10ms
  - Light switch state message: Every 20ms
  - Speed state message: Every 5ms
- Both ECUs possess an OS and application software components.

### Operational Logic:

1. Door opened & car moving → Buzzer ON, Lights OFF
2. Door opened & car stopped → Buzzer OFF, Lights ON
3. Door closed & lights were ON → Lights OFF after 3s
4. Car moving & light switch pressed → Buzzer OFF, Lights ON
5. Car stopped & light switch pressed → Buzzer ON, Lights ON

## Deliverables 📦

- System schematic [Block Diagram](https://github.com/t0ti20/Automotive_Door_Control/tree/master/Block%20Diagram) screenshot.
- PDFs for:
  - Static and Dynamic design analysis
  - State machine diagrams for each ECU component
  - ECU operation diagrams
  - Sequence diagrams
- Video recordings discussing the static design.

https://github.com/t0ti20/Automotive_Door_Control/assets/61616031/804abef1-a713-493f-a024-90e7357af998

- Video recordings discussing the dynamic design.


https://github.com/t0ti20/Automotive_Door_Control/assets/61616031/9fe59f0e-8a9b-4382-9f0c-be0ecc473579


- Pseudocode for each ECU component.
- `.c` and `.h` files for all ECU components.

## Getting Started 🚀

To delve into the intricacies of this project, navigate through the repository. For detailed instructions on each task, refer to the provided documentation and video walkthroughs.

## Contributing 🤝

Suggestions and contributions are always welcome! Please discuss any changes via issues before making a pull request.

## Authors

- [@Khaled El_Sayed](https://github.com/t0ti20)

## Acknowledgements 👏

Grateful to the FWD-EG Embedded Systems Track and everyone who contributed to this project.

