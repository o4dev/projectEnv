ProjectEnv
==========

Sets up and manages projects

> PLEASE NOTE: This does not manage packages inside the environment such as what virtualenv does

Install
=======
projectEnv comes with a install script which deals with most of the installation. However it
does require `apt-get` to satisfy its dependancys. If this is not an option for your system
it can be avoided by installing:
* `make`
* `npm`
* `python-pip`
then just remove the `sudo apt-get install make npm python-pip` line from your install.sh


1. ```git clone https://github.com/o4dev/projectEnv.git projectEnv```
3. ```chmod +x projectEnv/install.sh```
4. ```projectEnv/install.sh```

> [sudo] password for user: [enter password]<br>
> ... <br>
> Where do you want the development directory ?: [enter directory]


load settings after install
```
user@host:~/projectEnv$ cd ~
user@host:~$ source .bashrc
```

Usage - see the tutorial [here](https://github.com/o4dev/projectEnv/wiki/Tutorial)
=====

New Project:
```newproject [template] [optional: name] [if entered name and is gae: appid]```

```
user@host:~$ newproject gae/webapp2_jinja2_less_coffee_bootstrap
> What is the projects name? test # enter a name
> What is the appid for appengine for the project? test123 # enter Google app engine's appid
```

Activate Project:
```activate [project name]```

```
user@host:~$ activate test
user@test: $
```