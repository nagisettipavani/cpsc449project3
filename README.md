# CPSC 449 Web Back-End Engineering - Fall 2020 - Project 3
# Contributors: 
1. Sai Pavani Nagisetti (CWID: 888160793, Email: nagisettipavani@csu.fullerton.edu)
2. Rushabh Shah (CWID: 887456218, Email: rushabhshah@csu.fullerton.edu)


# Project description: 

This project involves making HTTP requests from a Python program and using this ability to store server-side session data in a separate storage service Version 3 database.

The following are the steps to run the project:
1. Clone the github repository https://github.com/nagisettipavani/cpsc449project3.git
2. Install the pip package manager by running the following commands
    > sudo apt update
    >
    > sudo apt install --yes python3-pip
   
3. Install Flask by:
    
    > python3 -m pip install Flask python-dotenv
   
4. Run the following commands to install Foreman and HTTPie:
    > sudo apt update
    
    > sudo apt install --yes ruby-foreman httpie

5. Then cd into the counter folder
    Run the following commands:
    > flask init
    
    > foreman start
    
Now, you will be to see that the two flask applications run on two different ports as configured in the Procfile.

The counter example shows a count value which increments on refresh of page or each visit and maintains a session Id.
The session id is stored in the keys list of the other flask application which can also be viewed on the browser on a different port as mentioned.

Note: Please also examine kv.py because in order to get all keys and values, there is an endpoint called /getAllKeysAndValues in kv.py.
   



