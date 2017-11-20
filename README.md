# browsepy

![](https://raw.githubusercontent.com/wdbm/browsepy/master/media/browsepy.png)

This is a web file browser that uses Flask and is compatible with Python 3.5. It is a fork of [browsepy](https://github.com/ergoithz/browsepy) by Felipe A. Hernandez.

# setup

```Bash
pip install git+https://github.com/wdbm/browsepy.git
```

# usage

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
