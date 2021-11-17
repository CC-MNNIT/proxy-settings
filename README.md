# MNNIT College internet proxy settings

In the below listed steps you can replace "172.31.100.29" with the proxy of your choice (based on speed/availability).

## For Windows:

- Add proxy in system proxy settings [Settings > Network & Internet > Proxy].
- Use one of the following:
    - [Proxifier](https://www.proxifier.com/)
    - [Psiphon Pro (VPN)](https://psiphon.ca/)
- In Command Prompt, for temporary proxy settings:
    ```bash
    set http_proxy=http://edcguest:edcguest@172.31.100.29:3128
    set https_proxy=https://edcguest:edcguest@172.31.100.29:3128
    ```
- For Lan Configuration Settings, [follow this](lan/README.md).

## For Android:

Use any one of these and enter appropriate settings in them:

- [College Proxy](https://play.google.com/store/apps/details?id=com.cell47.College_Proxy&hl=en_IN&gl=US)
- [Psiphon Pro (VPN)](https://psiphon.ca/)
- [Drony](https://play.google.com/store/apps/details?id=org.sandrob.drony&hl=en_IN&gl=US)

## For Linux/Mac terminal, temporary solution:

Run these:

```bash
export http_proxy="http://edcguest:edcguest@172.31.100.29:3128"
export https_proxy="https://edcguest:edcguest@172.31.100.29:3128"
export ftp_proxy="ftp://edcguest:edcguest@172.31.100.29:3128"
export socks_proxy="socks://edcguest:edcguest@172.31.100.29:3128"
export all_proxy="http://edcguest:edcguest@172.31.100.29:3128"

export HTTP_PROXY="http://edcguest:edcguest@172.31.100.29:3128"
export HTTPS_PROXY="https://edcguest:edcguest@172.31.100.29:3128"
export FTP_PROXY="ftp://edcguest:edcguest@172.31.100.29:3128"
export SOCKS_PROXY="socks://edcguest:edcguest@172.31.100.29:3128"
export ALL_PROXY="http://edcguest:edcguest@172.31.100.29:3128"
```

(Uppercases ones are optional, sometimes lowercases ones don't work). Read answers to [this Stackoverflow question](https://unix.stackexchange.com/questions/212894/whats-the-right-format-for-the-http-proxy-environment-variable-caps-or-no-ca).

You can also add these 6 lines to your `~/.bashrc` (or `~.zshrc` if using `zsh`) or `~/.profile` so that these are exported every time you open a terminal.

## For GNU/Linux, permanent solution:

- Enter proxy port info in System network settings. (not needed if you are using the following script).
- [Use these scripts.](linux-proxy)

## For MacOS:

Try [this](https://support.apple.com/en-in/guide/mac-help/mchlp2591/mac) and [this](https://support.apple.com/en-in/guide/safari/ibrw1053/mac).

## For Android Studio (Gradle):

[Follow link.](https://developer.android.com/studio/intro/studio-config?fbclid=IwAR0AfsH_nW9CUVs4knWtDnvTsdcvXEw4zCquF5AGGQLVxH7xfqomn5EqY0I#proxy)

## For Git:

[Follow link.](https://gist.github.com/evantoli/f8c23a37eb3558ab8765)

## For NPM:
* Applying Proxy (You can change the Proxy according to your needs, this is just an example with Proxy `172.31.100.14`) -
 
    ```bash
    npm config set proxy http://edcguest:edcguest@172.31.100.14:3128
    npm config set https-proxy http://edcguest:edcguest@172.31.100.14:3128
    ```
* Removing Proxy - 

    ```bash
    npm config rm proxy
    npm config rm https-proxy
    ```
    
## List of proxies available:

<a href="Proxies-2022.jpg"><img src="Proxies-2022.jpg"  alt="List of proxies available" height="400"/></a>

<hr>

*Have a suggestion? Create a git issue or contact CC Coordinators!*
