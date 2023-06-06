BruteForcer.py
This repository contains a Python script for a password cracker. The script attempts to brute-force a login page by trying different passwords for a given username. It utilizes the requests library for making HTTP requests and the termcolor library for colored output.

Prerequisites
To run this script, you need to have Python installed on your system. Additionally, you should have the following libraries installed:

requests
termcolor
You can install these libraries using pip with the following command:

Copy code
pip install requests termcolor
Usage
To use the password cracker script, follow these steps:

Clone the repository to your local machine or download the script directly.

Open a terminal or command prompt and navigate to the directory where the script is located.

Execute the script by running the following command:

Copy code
python password_cracker.py
You will be prompted to enter the following information:

Page URL: Enter the URL of the login page you want to brute-force.
Username: Enter the username for the account you want to crack the password for.
Password File: Enter the path to the password file you want to use. Each password should be on a separate line.
Login Failed String: Enter the string that occurs on the page when login fails. This string is used to determine if the login attempt was unsuccessful.
Cookie Value (Optional): If the login page requires a specific cookie value, you can enter it here.
The script will start brute-forcing the login page by trying each password from the provided password file.

If a successful login is found, the username and password will be printed, and the script will exit.

If no successful login is found, the script will display a message indicating that the password was not found in the list.

Notes
The script uses the requests library to send POST or GET requests to the login page with different passwords.
The script checks for the presence of the login failed string in the response content to determine if the login attempt was unsuccessful.
The script will continue trying passwords until it either finds a successful login or exhausts all passwords in the password file.
If a cookie value is provided, it will be included in the requests made by the script.
The script utilizes colored output from the termcolor library to highlight the password being tried in red and display the successful username and password in green.
Make sure to provide the correct information and adjust the script according to the login page's specific requirements.
Feel free to customize and modify the script according to your specific needs. Happy password cracking!




