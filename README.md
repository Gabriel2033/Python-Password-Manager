# Python-Password-Manager
 A basic command-line password manager written in Python. Allows users to create accounts and securely log in using SHA-256 password hashing.
### Prerequisites
- Python installed
- PyCharm installed
### Step 1
- We are going to import some libraries and create a password storage dictionary.
 ![image](https://github.com/user-attachments/assets/1bbcf70e-99c8-4e16-8986-5e5aaf449590)

Hashlib brings in Python's built-in library for hashing algorithms, and getpass prompts the user to enter a password without displaying it on the screen. Then we create a dictionary to store the credentials.
### Step 2
- Next, we are going to build a function that lets users create a new account.
  ![image](https://github.com/user-attachments/assets/0d048d52-e277-46ca-a419-2a64857957fd)
  
So what we have done is prompt the user for a username, then prompt for a password using getpass to add extra security. The password is then converted into a hashed string using SHA-256 encryption, and the credentials are stored in the password manager dictionary. We end it off by confirming the account has been created.
### Step 3 
- Now we create a login function.
 ![image](https://github.com/user-attachments/assets/4dd88fae-374c-4e40-9e36-fdb60806d41f)

Once again, we prompt the user for their username and their password, where the password is hashed to match the format stored in the password manager. Next, we check if the username exists in the password manager and if the hashed password matches the stored hashed password for that username. If the credentials match, it prints "Login successful" and if they don't, it prints "Login failed".
### Step 4
- Now we are building the core loop of the program that allows users to choose what they want to do.
 ![image](https://github.com/user-attachments/assets/d8c8895e-ce57-4820-b477-fd22fcfefd79)

Starting the loop, we begin to ask the user to choose what they want to do. If the user enters "1", the create account function is called; if they enter "2", the login function is called; if they enter "0", the loop breaks and the program ends. Any other output prints an "Invalid choice" message. This function acts as the main menu and control center of the password manager.
### Step 5
- Lastly, we are setting the entry point of the program so it runs the main menu when the script is executed directly.

  ![image](https://github.com/user-attachments/assets/b799de87-0b39-4894-8953-cf0832242db8)

What this does is check how the script is being run, whether it is being run directly or being imported and if it is being run directly, it will execute the main function, which boots up the password manager menu. 
