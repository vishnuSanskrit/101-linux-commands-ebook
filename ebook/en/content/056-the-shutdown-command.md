# The `shutdown` command

The `shutdown` command let you bring your system down in a secure way. When `shutdown` is executed the system will notify all logged-in users and disallow further logins.
You habae the option to shut down your system immediatly or after a specific time.

Only users with root (or sudo) privileges can use the `shutdown` command.

### Examples:

1. Shut down your system immediatly:

```
sudo shutdown now
```

2. Shut down you system after 10 minutes:

```
sudo shutdown +10
```

3. Shut down your system with a message after 5 minutes:

```
sudo shutdown +5 "System will shutdown in 5 minutes"
```

### Syntax:

```
shutdown [OPTIONS] [TIME] [MESSAGE]
```

### Additional Flags and their Functionalities:

|**Short Flag**   |**Long Flag**   |**Description**   |
|:---|:---|:---|
|`-r`|<center>-</center>|Reboot the system|
|`-c`|<center>-</center>|Cancel an sheduled shut down|