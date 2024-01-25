# OCPP Simulator

## Overview

This project is a simple Electric Vehicle (EV) Charger Simulator that follows the Open Charge Point Protocol (OCPP) standards. It provides a graphical user interface (GUI) built using tkinter to simulate the behavior of an EV charging station. The simulator supports basic OCPP 1.6 functionalities, including boot notification, authorization, start and stop transactions, status notifications, and sending meter values.

## Features

- **Boot Notification:** The simulator can send a boot notification to a central system, establishing a connection and receiving an interval for sending heartbeats.

- **Authorization:** It supports authorizing RFID tags, allowing or denying access to the charging station.

- **Start Transaction:** The simulator can initiate a charging transaction with specified parameters such as connector ID, RFID tag, and meter start value.

- **Stop Transaction:** It simulates stopping a transaction with details like meter stop value and reason.

- **Heartbeat:** The simulator sends periodic heartbeats to the central system.

- **Meter Values:** It can send meter values, including energy consumption, during a charging session.

- **Status Notification:** The simulator can send status notifications to update the central system about the charging station's status.

## Getting Started

### Prerequisites

- Python 3.7 or higher
- `websockets` library
- `ocpp` library

### Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/ocpp-simulator.git
    cd ocpp-simulator
    ```

2. Install dependencies:

    ```bash
    pip install -r requirements.txt
    ```

### Usage

1. Run the simulator:

    ```bash
    python ocpp_simulator.py
    ```

2. Fill in the required information in the GUI, such as the central station WebSocket URL, charge station serial number, RFID tag, etc.

3. Use the provided buttons to perform actions like connecting to the central system, authorizing RFID tags, starting and stopping transactions, and more.

4. View the console output for detailed logs and simulation information.

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/my-feature`.
3. Commit your changes: `git commit -m 'Add my feature'`.
4. Push to the branch: `git push origin feature/my-feature`.
5. Submit a pull request.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- Thanks to the OCPP community for the protocol standards.
- Inspired by the need for a simple OCPP simulator for testing purposes.
