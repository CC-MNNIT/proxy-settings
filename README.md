# MNNIT College internet proxy settings

In the below listed steps you can replace "172.31.102.29" with the proxy of your choice (based on speed/availability).

## For Windows:

- Add proxy in system proxy settings [Settings > Network & Internet > Proxy].
- Use one of the following:
  - [Proxifier](https://www.proxifier.com/). Configuration [details here](proxifier).
  - [Psiphon Pro (VPN)](https://psiphon.ca/)
- In Command Prompt, for temporary proxy settings:
  ```bash
  set http_proxy=http://edcguest:edcguest@172.31.102.29:3128
  set https_proxy=http://edcguest:edcguest@172.31.102.29:3128
  ```
- For LAN Configuration Settings, [follow this](lan/README.md).

## For Android:

Use any one of these and enter appropriate settings in them:

- [College Proxy](https://play.google.com/store/apps/details?id=com.cell47.College_Proxy&hl=en_IN&gl=US)
- [Drony](https://play.google.com/store/apps/details?id=org.sandrob.drony&hl=en_IN&gl=US)
- [Psiphon Pro (VPN)](https://psiphon.ca/)

## For GNU/Linux, permanent solution:

- Enter proxy port info in System network settings, only web browsers will work. (not needed if you are using the following script).

  and;

- **[Use these scripts](linux-proxy)**. Read the README present at the link.

## For Linux/Mac terminal, temporary solution:

Run these:

```bash
export http_proxy="http://edcguest:edcguest@172.31.102.29:3128"
export https_proxy="http://edcguest:edcguest@172.31.102.29:3128"
export ftp_proxy="http://edcguest:edcguest@172.31.102.29:3128"

export HTTP_PROXY="http://edcguest:edcguest@172.31.102.29:3128"
export HTTPS_PROXY="http://edcguest:edcguest@172.31.102.29:3128"
export FTP_PROXY="http://edcguest:edcguest@172.31.102.29:3128"
```

(Uppercases ones are optional, sometimes lowercases ones don't work). Read answers to [this Stackoverflow question](https://unix.stackexchange.com/questions/212894/whats-the-right-format-for-the-http-proxy-environment-variable-caps-or-no-ca).

You can also add these 6 lines to your `~/.bashrc` (or `~.zshrc` if using `zsh`) or `~/.profile` so that these are exported every time you open a terminal.

## For MacOS:

Try [this](https://support.apple.com/en-in/guide/mac-help/mchlp2591/mac) and [this](https://support.apple.com/en-in/guide/safari/ibrw1053/mac).

## For Android Studio (Gradle):

[Follow link.](https://developer.android.com/studio/intro/studio-config?fbclid=IwAR0AfsH_nW9CUVs4knWtDnvTsdcvXEw4zCquF5AGGQLVxH7xfqomn5EqY0I#proxy)

## For Git:

[Follow link.](https://gist.github.com/evantoli/f8c23a37eb3558ab8765)

```bash
add Proxy in GIT Bash
git config --global http.proxy http://edcguest:edcguest@172.31.102.29:3128

Unset Proxy from Git Bash

git config --global --unset http.proxy
git config --global --unset http.https://domain.com.proxy

git config --global --unset http.sslVerify
git config --global --unset http.https://domain.com.sslVerify

```

## For NPM:

- Applying Proxy:

  ```bash
  npm config set proxy http://edcguest:edcguest@172.31.102.29:3128
  npm config set https-proxy http://edcguest:edcguest@172.31.102.29:3128
  ```

- Removing Proxy:

  ```bash
  npm config rm proxy
  npm config rm https-proxy
  ```
## For Docker

[Follow link.](https://docs.docker.com/network/proxy/)

## List of proxies available:

<a href="Proxies-2022.jpg"><img src="Proxies-2022.jpg"  alt="List of proxies available" height="400"/></a>

<hr>

_Have a suggestion? Create a GitHub issue or [contact CC Coordinators](https://cc-mnnit.github.io/#current-representatives)!_
