Merge-conflicter


Om nama shivaya 
===
# Merge-conflicter



i have created a new line

and a second line here

import socket

# 1. Create a TCP/IP socket
client_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)

# 2. Connect to the server
client_socket.connect(("127.0.0.1", 65432))

# 3. Send data (must be encoded as bytes)
client_socket.sendall(b"Hello from the client!")

# 4. Wait for a response
response = client_socket.recv(1024)
print(f"Server replied: {response.decode()}")

# 5. Close the socket
client_socket.close()
