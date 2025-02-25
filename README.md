# Cisco 2960S HTML Port Viewer

This project provides a web-based interface to visualize the status of ports on a Cisco 2960S switch. It retrieves port status using Netmiko and displays active and inactive ports in a graphical layout.

## Features
- Display 24 GigabitEthernet ports in a 2-row layout (odd ports on top, even on bottom).
- Show VLAN1 and FastEthernet0 separately.
- Ports turn **green** if up, **red** if down.
- Execute **"show"** CLI commands directly from the web interface.
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
<img width="455" alt="Cisco_HTML_View" src="https://github.com/user-attachments/assets/0c798456-191c-4af6-843b-093e137bf040" />


### **Port Status Visualization**
<img width="437" alt="Cisco_Port_Status" src="https://github.com/user-attachments/assets/34af43ec-2cd6-45e8-97a5-1ba7b9d63303" />


### **CLI Command Execution**
<img width="340" alt="Cisco_Show_CLI" src="https://github.com/user-attachments/assets/37d906da-95a1-4e0d-a43d-bee3f291c4ab" />


## Future Enhancements
- Add authentication for security.
- Improve UI styling.
- Extend to support multiple switches.

## License
This project is licensed under the MIT License.

## Author
Developed by **i-tri** ([GitHub Profile](https://github.com/i-tri)).

