# MNNIT College internet proxy settings

## For Windows:

- Add proxy in system proxy settings.
- Use one of the following:
    - [Proxifier](https://www.proxifier.com/)
    - [Psiphon Pro (VPN)](https://psiphon.ca/)
- In Command Prompt, for temporary proxy settings:
    ```bash
    set http_proxy=http://edcguest:edcguest@proxy:3128
    set https_proxy=https://edcguest:edcguest@proxy:3128
    ```

## For Android:

- [College Proxy](https://play.google.com/store/apps/details?id=com.cell47.College_Proxy&hl=en_IN&gl=US)
- [Psiphon Pro (VPN)](https://psiphon.ca/)
- [Drony](https://play.google.com/store/apps/details?id=org.sandrob.drony&hl=en_IN&gl=US)

## For Linux/Mac terminal, temporary solution:

Run these:

```bash
export http_proxy="http://edcguest:edcguest@proxy:3128"
export https_proxy="http://edcguest:edcguest@proxy:3128"
export all_proxy="http://edcguest:edcguest@proxy:3128"
```

## For GNU/Linux, permanent solution:

[Use these scripts.](linux-proxy)

## For Android Studio (Gradle):

[Follow link.](https://developer.android.com/studio/intro/studio-config?fbclid=IwAR0AfsH_nW9CUVs4knWtDnvTsdcvXEw4zCquF5AGGQLVxH7xfqomn5EqY0I#proxy)

## For Git:

[Follow link.](https://gist.github.com/evantoli/f8c23a37eb3558ab8765)

## List of proxies available:

<a href="Proxies-2022.jpg"><img src="Proxies-2022.jpg"  alt="List of proxies available" height="400"/></a>

<hr>

*Have a suggestion? Create a git issue or contact CC Coordinators!*
