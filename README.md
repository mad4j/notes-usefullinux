Useful Linux
============
Same useful terminal commands that may save your week-ends!!


## :repeat: Do not repeat yourself.

```$ sudo !!```

Forget to sudo? Don't worry is not needed to re-type to whole command.

![sudo](gifs/sudo.gif)


## :movie_camera: Bash, the Director's cut!!

```$  ttystudio output.gif --log```

Use ```^Q``` to terminate recording session and generate animation.

## System information

Get brief system description:

```$ uname -a```

How long since last boot:

```$ uptime```

System host name:

```$ hostname```

Host IP address:

```$ hostname -I```


![sysinfo](gifs/sysinfo.gif)


## Continously watch

Repeat a command coninuosly:

```$ watch -n 1 -d ifconfig eth0```


![watch](gifs/watch.gif)


## :envelope: Please, tell me my address

``` $ curl ifconfig.me ```

What is my external IP address? or more detailed information:

``` $ curl ipinfo.io ```

![sudo](gifs/ipinfo.gif)


## :mag: Performing historical researches

Search in bash history in interactive mode by pressing ``` CTRL-R```.

Type part of your command and the most recent match will be suggested. Then press ```ENTER``` to execute the command or ```CTRL-R``` again to search the next match.
Use ```CTRL-C``` to cancel the operation and return back to the shell.

![sudo](gifs/ctrl-r.gif)


## References

* [51 Useful Lesser Known Commands for Linux Users](https://www.tecmint.com/51-useful-lesser-known-commands-for-linux-users/)
* [Best tips and triks for bash](https://linuxacademy.com/blog/linux/tutorial-the-best-tips-tricks-for-bash-explained/)
