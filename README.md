# Slowloris.py - a low bandwidth DOS tool
Proof of concept code in python3 of the [slowloris](https://en.wikipedia.org/wiki/Slowloris_(computer_security)) attack invented by RSnake.


## Note

It's recommended you run the script on a Linux host rather than Windows, this is due to a limitation set by Windows OS which limits the amount of sockets you can use at once.

If the remote server is vulnerable you're usually able to successfully DOS the remote server, continue to raise the number of connections until you've accomplished your test.

## Usage

```
slowloris.py [-h] [-p PORT] [-c COUNT] [-f FREQ] [-v] [-s] [RHOST]

Slowloris PoC demonstration in python3

positional arguments:
  RHOST                     Remote host, the victim webserver in 
                            either domain or IPv4 format

optional arguments:
  -h, --help                Show a help message and exit
  -p PORT, --port PORT      Port of the remote webserver
  -c COUNT, --count COUNT   Number of connections to fire up
  -f FREQ, --freq FREQ      Frequency to message the web server
  -v, --verbose             Enables debug verbosity
  -s, --https               Secure the attacker connections with HTTPS
```

## License
This project is licensed under the MIT License - see the [LICENSE](https://github.com/Zatrac/slowloris.py/blob/master/LICENSE) file for details
