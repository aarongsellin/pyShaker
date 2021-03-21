# pyShaker
An easy to use library for encrypting, decrypting and signing data. It can also be used to establish an RSA/AES handshake.

## Installing
Download with ![git](https://git-scm.com/).

```$ git clone https://github.com/mrikea4real/pyShaker```

## Examples
_Client doing a handshake with a server_:

```
>>> from pyShaker import *        # Import shaker library
[ Code for connecting to server ]
>>> shaker = SetupShaker(sock)    # Setup the shaker object
>>> shaker.shake()                # Initate a handshake 
1
>>> shaker.send("testing")        # Send encrypted message to the server
1
```

## Documentation


## Contributing
I would be more than happy to accpet contributions. These can come in the form of bug reports, feature requests and pure code!

## Maintainers
* ![@mrikea4real](https://github.com/mrikea4real) (Aaron Gotthardsson)
