# Splunk Blocklist Integration App

The Splunk Blocklist Integration App is designed to fetch blacklisted IP addresses from `blocklist.de` on an hourly basis and ingest this data into Splunk. This automation aids security and IT professionals in monitoring and analyzing potentially malicious IP addresses.

![Снимок экрана 2023-08-22 151031](https://github.com/DamikoMu/splunk_app_blocklist/assets/48206331/f86fca10-f0a7-4e9b-afa2-2ffbb4d08a79)


## Features

- **Automated Data Collection**: Fetches blacklisted IP addresses every hour.
- **Data Deduplication**: Ensures only new IP addresses are ingested into Splunk.
- **Python Script**: Cross-platform compatibility and easy integration with Splunk.


## Table of Contents

- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)
- [Support](#support)

## Prerequisites

- Splunk instance up and running.
- Python 3.x installed on the machine where Splunk is running.
- Appropriate permissions to create and manage Splunk apps and data inputs.

## Installation

1. **Clone the Repository**:  
    ```bash
    git clone https://github.com/your_username/splunk-blocklist-app.git
    ```

2. **Move to Splunk Apps Directory**:  
    Navigate to your Splunk installation directory and place the cloned repository in the `apps` folder.

3. **Restart Splunk**:  
    This ensures Splunk recognizes and integrates the new app.

## Usage

1. **Configure Data Input**:  
    In Splunk, navigate to "Settings" > "Data inputs", and set up a new script-based data input pointing to the `blocklist_puller.py` script. Set the interval to 3600 seconds (1 hour).



## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Support

For support, bug reports, or feature requests, please open an issue on our [issues page](link_to_issues_page) or reach out via email at [support@example.com](mailto:support@example.com).
