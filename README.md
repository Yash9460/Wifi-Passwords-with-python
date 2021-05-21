## Wifi-Passwords-with-python

# How to Get Wifi Passwords with python?

Sometimes we forget our own connected wifi password. And when someone asks for the password to connect with the same network we decline. In this repository, we are going to learn how we can see wifi passwords with python.

In order to get wifi passwords, we are going to use the subprocess module of Python which makes it easy to check the connected wifi passwords by allowing us to run (cmd)command prompt commands inside our program. We have two netsh commands using them we can easily see wifi passwords.

Logic is very simple, we will run cmd commands to check wifi passwords inside our program with the help of the subprocess module as mentioned above.

- The two cmd commands to check connected wifi passwords are as follows:
    
      netsh wlan show profile
      netsh wlan show profile PROFILE-NAME key=clear
    
    
The first command is used to show the profiles of the connected wifi while 2nd is used to show the password of the wifi which you want to know.

Here we will use these two commands in our own way to Get WiFi Passwords With Python.

# Run cmd commands for wifi passwords in python

As mentioned earlier, we are going to use the subprocess module to run cmd commands in our python program. We will use a method from the subprocess module called check_output to run both cmd commands.

# Stepwise flow of code

- Import subprocess module.

- Run the 1st cmd command using subprocess.check_output method and store the profiles data in a variable.

- Convert the profile data into a list.

- Iterate over the list and run the second command to check the passwords.

- Store the paswords and print

# Output

![Screenshot 2021-05-21 221724](https://user-images.githubusercontent.com/73324896/119171541-589b0000-ba82-11eb-96a2-b6801c8eecdb.png)
