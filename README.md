# Cisco ISE-PIC Identity Manager

This script provides a Python interface to manage user identity events for Passive Identity services with Cisco ISE-PIC.

## Requirements

- Python 3.x
- `requests` library (install via `pip install requests`)

## Usage

1. Clone or download the script to your local machine.
2. Install the required libraries if not already installed: `pip install requests`.
3. Run the script with the necessary arguments:

```bash
python3 passive_id.py <ise_ip> <pic_user> <pic_pwd> <agent_id>
```

* `<ise_ip>`: IP address of the Cisco ISE-PIC.
* `<pic_user>`: Username for authentication.
* `<pic_pwd>`: Password for authentication.
* `<agent_id>`: Agent ID.


## Functionality

#### Generate Authentication Token: 
Creates an authentication token to be used for subsequent requests.

#### Add Identity Mapping: 
Adds a user identity mapping with provided details.

#### Delete Identity Mapping by ID: 
Deletes a user identity mapping by its ID.

#### Delete All Identity Mappings by Agent ID: 
Deletes all user identity mappings associated with a specific agent ID.

## Script Details
The script initializes a CiscoISEPICManager class instance with the provided Cisco ISE-PIC details.
It then demonstrates adding a user, removing a user, and deleting all identity mappings by agent ID.

## Testing

* To test the functionality of the script, ensure that the Cisco ISE-PIC instance is accessible from your network and that the provided authentication credentials are correct.
* Run the script with the required arguments, and verify that the expected operations are performed successfully.
* Check the console output for any error messages or confirmation of successful operations.

## License
This project is licensed under the MIT License - see the LICENSE file for details.