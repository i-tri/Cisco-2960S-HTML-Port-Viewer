# Cisco 2960S HTML Port Viewer

This project provides a web-based interface to visualize the status of ports on a Cisco 2960S switch. It retrieves port status using Netmiko and displays active and inactive ports in a graphical layout.

## Features
- Display 24 GigabitEthernet ports in a 2-row layout (odd ports on top, even on bottom).
- Show VLAN1 and FastEthernet0 separately.
- Ports turn **green** if up, **red** if down.
- Execute "show" CLI commands directly from the web interface.
- Auto-refresh every 5 seconds to keep the status updated.

## Technologies Used
- **Flask** (Python-based web framework)
- **Netmiko** (For SSH communication with the switch)
- **HTML, CSS, JavaScript** (Frontend)

## Installation & Setup
### Prerequisites
- Python 3 installed
- Required libraries: Flask, Netmiko
- A Cisco 2960S switch with SSH access enabled

### Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/i-tri/Cisco_2960s_HTML_Port_Viewer.git
   cd Cisco_2960s_HTML_Port_Viewer
   ```
2. Install dependencies:
   ```sh
   pip install flask netmiko
   ```
3. Run the Flask application:
   ```sh
   python cisco.py
   ```
4. Open a browser and go to:
   ```
   http://127.0.0.1:5000
   ```

## Usage
1. The main interface will display the switch port status.
2. Use the CLI input box to send commands directly to the switch and view output.

## Screenshots
### **Main Interface**
![Main Interface](screenshots/main_interface.png)

### **Port Status Visualization**
![Port Status](screenshots/port_status.png)

### **CLI Command Execution**
![CLI Execution](screenshots/cli_execution.png)

## Future Enhancements
- Add authentication for security.
- Improve UI styling.
- Extend to support multiple switches.

## License
This project is licensed under the MIT License.

## Author
Developed by **i-tri** ([GitHub Profile](https://github.com/i-tri)).

