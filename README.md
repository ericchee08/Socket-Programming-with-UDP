# Socket-Programming-with-UDP
UDP allows two or more processes running on different hosts to communicate. UDP is a connectionless service - there is no handshaking to establish a communication pipe because UDP does not have a pipe. When UDP communicates, it attaches the destination address to each batch of data that is being sent  In UDP, the destination address is the IP address of the host and port number.  The host IP address, the port number and the actual data to be transferred are collectively called a ‘packet’. UDP provides an unreliable message-oriented service model, in that it makes a best effort to deliver the packet to the destination in a single operation at the sending side. UDP is a best-effort service; it makes no guarantee that the packet will be delivered. This is in contrast to TCP, which has a reliable service model.

1. The client reads a line from its standard keyboard and sends the line out from its socket to the server.
2. The server reads the line from the socket.
3. The server converts the line to upper case.
4. The server sends the modified line out of its socket to the client.
5. The client reads the modified line from its socket and prints it.

<img width="881" alt="Screenshot 2021-09-13 at 19 34 26" src="https://user-images.githubusercontent.com/58150120/133138000-09cffede-299f-4e05-8e60-16cc67c26776.png">

