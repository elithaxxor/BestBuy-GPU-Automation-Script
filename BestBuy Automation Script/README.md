BestBuy Automation (GPU) Script

This project automates interactions with BestBuy’s website using Selenium WebDriver. The script can automate processes such as logging into a BestBuy account, adding a product to the cart, and placing an order. It also includes methods to handle installation of required dependencies and display status messages.

Features

	•	Automates the login process on BestBuy’s website.
	•	Navigates through BestBuy product pages (e.g., GPUs) and adds items to the cart.
	•	Handles interactions with web elements like banners, buttons, and form inputs.
	•	Implements waiting mechanisms to ensure proper timing for web page loading.
	•	Includes colorful terminal output to show the status of various steps.
	•	Supports installing necessary dependencies through Python’s subprocess.

Requirements

To run this project, you need the following Python packages:

	•	selenium
	•	webdriver-manager
	•	tqdm

To install these dependencies, you can run the following command:
```pip install selenium webdriver-manager tqdm```   

Additional Requirements:

	•	Chrome browser
	•	ChromeDriver (installed automatically using webdriver-manager)

Installation

	1.	Clone the repository:
```git clone
    2.	Change to the project directory:
 ```
```cd bestbuy-automation-script
    3.	Install the required dependencies:
```
``` pip install -r requirements.txt
    4.	Run the script:
```
```python bestbuy_automation.py
    5.	Follow the on-screen instructions to interact with the BestBuy website.
```

Usage: 
Step 1: Set Up ChromeDriver

The script uses webdriver-manager to manage the ChromeDriver for Selenium. Ensure you have Chrome installed on your system, and the appropriate version of ChromeDriver will be installed automatically.

Step 2: Run the Script

To run the script, execute the following command:
```python bestbuy_automation.py
```
Step 3: Interact with the Script
Methods Overview

	1.	BestBuy_ripper Class:
	•	Manages the interaction with BestBuy’s website, including login, navigating to product pages, and handling the cart checkout process.
	•	Methods:
	•	login_info: Automates the login process to the BestBuy account.
	•	first_page: Navigates to a specific product page (e.g., NVIDIA GPU).
	•	iterate: Attempts to add an item to the cart.
	•	click_thru_page: Moves to the cart page and initiates the checkout process.
	•	parse_login: Handles the login by filling email and password fields.
	2.	Prettify Class:
	•	Provides utility methods for displaying colorful messages and spinners in the terminal.
	•	Methods:
	•	spinner: Shows a loading spinner.
	•	display_header: Displays a header with usage instructions and system details.
	•	period_wait: Simulates a waiting period with dots.
	3.	install_dependants Class:
	•	Installs necessary dependencies for the project using Python’s subprocess module.
	•	Methods:
	•	install_plugins: Installs plugins such as threading, tqdm, datetime, etc.
