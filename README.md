PROCEDURE:  
  
•	We first need to install the pyautogui module to control the cursor and keyboard. 
 
•	We now need to download server.py onto one of the computers and client.py to the rest. 
 
•	Now run server.py on and note the IP address as well as the port that comes as an alert. 
 
•	On the other computers, run client.py. When it asks for the Host IP Address and the Port, type the details that you saw in the alert. 
 
•	On the computer running server.py, you should now see a tkinter window. This window is your virtual touchpad. Click inside the window, and as your cursor moves inside that window, the cursor will move simultaneously on the client computers! 
 
•	You can adjust the window so that the touchpad can reach each end of the client computer. You can use Control + l for left click, Control + r for right click and Control + d for the double click. I am working on adding dragging functionality to the touchpad too! 
 
•	To type text, click on the 'Text' button from the menu of the touchpad. This should bring up a window. Use the text field to enter your text, and click on the 'Type Text' button to type the text on the clients, 'Delete' for 'backspace' and 'Enter' for a new line. 

 
 *Import Socket Library  
	To use a socket object in your program, start off by importing the socket library. No need to install it with a package manager, it comes out of the box with Python.  

To establish a connection between client and server, we need to create socket objects. In Python, we can do this using the socket module.

# Create a socket object for the client
client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
2. Opening and Closing Connections
Once we have initialized socket objects, we can proceed to open a connection, send and receive data, and finally, close the connection.

# Connect to a specified IP and port
client_socket.connect(('0.0.0.0', 8080))

# Sending data (this method can be called multiple times)
client_socket.sendall(b'Hello, server!')

# Close the socket connection to stop data transmission
client_socket.close()
