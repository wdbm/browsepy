# browsepy

![](https://raw.githubusercontent.com/wdbm/browsepy/master/media/browsepy.png)

This is a web file browser that uses Flask and is compatible with Python 3.5. It is a fork of [browsepy](https://github.com/ergoithz/browsepy) by Felipe A. Hernandez.

# setup

```Bash
pip install git+https://github.com/wdbm/browsepy.git
```

# HTTP usage with Flask

Installed, browsepy can be run in the following way:

```Bash
browsepy 127.0.0.1 8080 --directory="${HOME}/share"
```

As a cloned repository, browsepy can be run in the following way:

```Bash
python -m browsepy 127.0.0.1 8080 --directory="${HOME}/share"
```

As a cloned repository, browsepy can be hosted in the following way:

```Bash
sudo python -m browsepy 0.0.0.0 80 --directory="${HOME}/share"
```

# HTTPS usage with Gunicorn

Installed, browsepy can be run with Gunicorn via HTTPS. Run with Gunicorn, command line arguments and options should be expressed as an argv list argument for the function `browsepy.__main__:WSGI`, in a way like the following:

```Bash
sudo gunicorn --workers=4 "browsepy.__main__:WSGI(argv=['0.0.0.0', '8080', '--directory=/home/user/share'])" --bind=0.0.0.0:8080 --certfile=/home/user/certificates/fullchain.pem --keyfile=/home/user/certificates/privkey.pem
```
