# Password Security Check Tool
This Python script checks if a password has been exposed in data breaches using the "Have I Been Pwned" API. It utilizes the SHA-1 hash function to securely check your password against breach databases without sending your actual password over the network.

Features
- Secure password checking using SHA-1 hash.
- Checks against real breach databases via the "Have I Been Pwned" API.
- Command-line interface for easy use.

Prerequisites
Before running this script, ensure you have Python installed on your system. Additionally, you'll need the requests module, which can be installed via pip:
pip install requests

Run the script from the command line by passing the passwords you want to check as arguments:
python checkmypassword.py password1 password2 password3
Replace password1 password2 password3 with the passwords you wish to check. The script will output whether each password was found in data breaches and the number of times it was exposed.

Example
python checkmypassword.py examplePassword123
Output:
examplePassword123 was found 3 times!

Security Note
This tool uses a range query which only transmits the first 5 characters of the SHA-1 password hash, ensuring that your full passwords are never exposed externally.

Contributions
Contributions are welcome! Please fork the repository and submit a pull request with your suggested changes.




