# Black Hat Python - Chapter 2

**TCP Client**  
The script **tcp_client.py** is an example of using the [socket](https://docs.python.org/3/library/socket.html) module to send and receive data from a host.

There are a couple of assumptions this script makes:
1. The connection will always succeed
2. The server expects us to send some data first (some servers expect to send data to you first)
3. The server will always return data to us in a timely fashion

Here is an example of what the script returns:

![tcp_client.py results](images/tcp_clientresults.png)