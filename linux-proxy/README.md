# PROXY APPLIER FOR GNU/LINUX (MNNIT)

**Please read this thoroughly, at least once.**


*NOTE: first create a backup of /etc/environment file before using this script (it'll help if something unexpected happens).*

*ALSO: NEVER EVER use `sudo` to run this script.	<-follow strictly*

<hr>

## TO USE:

Open terminal in the directory in which [`apply_proxy`](apply_proxy), [`remove_proxy`](remove_proxy) are present.

To set proxy enter the command:

```bash
./apply_proxy
```

and enter the proxy host name you want to use.

To unset enter the command:

```bash
./remove_proxy
```

**NOTE:** If you are using KDE Plasma desktop, turn on "System Settings > Network > Settings > Proxy > Use system proxy configuration" for easy proxyfication.

<hr>

## TO USE THE SCRIPT FROM ANYWHERE:

If you want the flexibility to use the script from anywhere and not only the directory in which it is kept, put the scripts in `~/.local/bin/` directory.

You can use:

```bash
curl https://raw.githubusercontent.com/cc-mnnit/proxy-settings/main/linux-proxy/apply_proxy > ~/.local/bin/apply_proxy && chmod +x ~/.local/bin/apply_proxy

curl https://raw.githubusercontent.com/cc-mnnit/proxy-settings/main/linux-proxy/remove_proxy > ~/.local/bin/remove_proxy && chmod +x ~/.local/bin/remove_proxy

```

<hr>

## WHAT THE SCRIPT DOES:

`apply_proxy` adds (or applies) proxy related lines (or settings) in 1. `/etc/environment`, 2. `snap`, 3. `/apt/apt.conf`, 3. `dconf` (org.gnome.system.proxy) and 4. `git`.

You are using this shell script on your sole responsibility. Do keep a backup of `/etc/environment` as a safety measure. If anything wrong happens or you system bricks, don't blame it on me.

I would suggest you to first understand what is in the scripts before executing them.

(All these warnings are due to the fact that /etc/environment file is being edited, which uses root access)

<br>

Have a suggestion? Create a git issue or contact CC Coordinators!

*Thank You!*
