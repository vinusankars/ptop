# ptop

An awesome task manager written in python. A more awesome top like thing in your terminal !


![ptop-image](https://github.com/darxtrix/ptop/blob/master/docs/ptop.gif)


> Inspired by [vtop](https://github.com/MrRio/vtop)

## Installing

*Note: `ptop` is in active development right now, `pip` registry has the outdated `ptop` version Consider [these](https://github.com/darxtrix/ptop#development) instructions if you want to use the updated and bug free`ptop`.*

```bash
$ pip install ptop
```
**Note:** Python 2.X supported yet, no support for python3.

If **Python3** is your system default:

```bash
pip2.7 install ptop
```

## Usage

```
$ ptop -t <theme>
```


## Supported themes

- `colorful`     
- `elegant`    
- `simple`    
- `dark`   
- `light` etc.

## Changelog [updated on 11 Aug 2017]

- [Fixed] version 0.0.6 fixes index errors.[Issue4](https://github.com/darxtrix/ptop/issues/4)
- [Fixed] A default theme option has been set.[Issue5](https://github.com/darxtrix/ptop/issues/5)
- Though there are some [known issues](https://github.com/darxtrix/ptop#known-issues) still left. :cold_sweat:


## Some Screenshots

![ptop-1](https://github.com/darxtrix/ptop/blob/master/docs/ptop1.png)

![ptop-2](https://github.com/darxtrix/ptop/blob/master/docs/ptop.png)

![ptop-3](https://github.com/darxtrix/ptop/blob/master/docs/ptop2.png)


## Help

```bash
$ ptop -h
```


## Known Issues

- Sometimes garbage text appears on the screen, press `Ctrl` + `L` to **clear**. (Anybody having idea about this ?)
- Though ptop is responsive across various terminal sizes as positioning is done according to terminal sizes, but sometimes things may break. If so, then try in a terminal of bigger size.


## Development

```bash
$ git clone https://github.com/darxtrix/ptop
$ cd ptop   
$ python setup.py develop
```
**Note :** ptop will create a log file called `.ptop.log` in the home directory of the user.


## Main modules :
- `ptop.core` : Defines a basic `Plugin` class that other plugins in the `ptop.plugins` inherit.
- `ptop.interfaces` : The interface to the ptop built using npyscreen.
- `ptop.plugins` : This module contains all the plugin sensors supported i.e `Disk Sensor`,`Memory Sensor`,`Process Sensor`, etc. ( Any new plugin should be added here).
- `ptop.statistics` : Generate continuous statistics using background thread jobs by locating plugins in the plugins directory.
- `ptop.utils` : Custom thread classes.


## Main Dependencies
- [npyscreen](https://pypi.python.org/pypi/npyscreen)
- [psutil](https://pypi.python.org/pypi/psutil)
- [drawille](https://github.com/asciimoo/drawille)


## Contributions

- Pull requests are awesome and always welcome. Please use the [issue tracker](https://github.com/darxtrix/ptop/issues) to report any bugs or file feature requests.
- I really want to move the project forward to the next stable release but I am kind of busy nowadays, so not able to catch up on things quickly. So, contributions are required and moreover if someone wants to be a core contributor, let's have a quick chat on things. Yeah, send me an email. :smiley:


## License 

MIT © [Ankush Sharma](http://github.com/darxtrix)


