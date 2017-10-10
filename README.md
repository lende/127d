# Idea: "127 daemon"

**Note:** This is just an *idea* for someone to steal, as I'm not an active user
of macOS. The thought came to me when developing the [127]-tool, and testing it
on a Mac.

`127d` is a macOS daemon that automates aliasing of [loopback addresses] based
on entries in the local [hosts-file]. Aliasing is neccessary since loopback
addresses, except for 127.0.0.1, are not routed to the local host by default.
See this [Super User question] for details.

The deamon reads the hosts-file on startup (aliases must be recreated after each
reboot), and whenever the file changes.

[127]: https://github.com/lende/127
[loopback addresses]: https://en.wikipedia.org/wiki/Localhost#Name_resolution
[hosts-file]: https://en.wikipedia.org/wiki/Hosts_(file)
[Super User question]: https://superuser.com/questions/458875/
