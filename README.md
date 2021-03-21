# pyShaker
pyShaker is an easy to use library that sets up an encrypted tunnel for sending and receiving data between two endpoints. 

## Installing
Download with ![git](https://git-scm.com/).

```$ git clone https://github.com/mrikea4real/pyShaker```

## Examples
_Client doing a handshake with a server_:

```
>>> from pyShaker import * # Import shaker library
>>> import socket          # Import socket library
>>> 
>>> shaker = pyShaker.SetupShaker("10.10.10.10",8888) # Setup the shaker object
                                                      # This single command connects and exchanges encryption keys with the server.
1
>>> shaker.send("testing") # Send encrypted message to the server
1
>>> shaker.close() # Close connection to server
```

## Documentation
_Default RSA encryption strength is set at 1024_

```SetupShaker(ip,port)``` - Returns shaker object and connects to server through TCP.

```send(data)``` - Sends and encrypts data.

```receive(size)``` - Receives and decrypts data.

```close()``` - Close session and disconnect from the server.

## Contributing
I would be more than happy to accpet contributions. These can come in the form of bug reports, feature requests and pure code!

## Maintainers
* ![@mrikea4real](https://github.com/mrikea4real) (Aaron Gotthardsson)
