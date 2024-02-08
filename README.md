# High-Level Approach
My high-level approach was to first implement basic command line parsing functionality before I did anything else. This was to make sure that the correct data was being passed to all functions I write to avoid any future mistakes. Then, I created a class to represent my TCP client. I felt that this was best to centralize the functionality of the client into one object, holding important things such as the host, port, control socket, and the data socket. Then, I implemented each command from lowest difficulty to highest difficulty. MKD and RMD were not dependent on a data socket, so I was able to implement those first. I handled each operation individually on the command line with conditional statements (ideally would be switch-case, but that's only available in Python 3.10+) to call on the appropriate functions for each operation.

# Challenges
Challenges I faced in this project were:
- Using 2 sockets simultaneously
- Command line parsing
- Response parsing (like the TCP response codes)
- Handling multiple different operations individually
- Calling on the correct commands in the correct order to fulfill a request

# Testing
For testing I:
- Utilized print statements throughout my code while debugging
- Used try/catch statements
- Checked error codes to catch when my client would fail
- Used 'ls' frequently to check updates to the server