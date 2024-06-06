# DarkScout

[![Forks][forks-shield]][forks-url][![Stargazers][stars-shield]][stars-url][![Issues][issues-shield]][issues-url]

DarkScout is a simple, nimble subdomain enumeration tool written in Rust language. It is designed to help bug bounty hunters, security professionals and penetration testers discover subdomains of a given target domain.

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->

OSINT sources:
- Alienvault
- Anubis
- Crtsh
- Hackertarget
- Threatminer

<!-- ROADMAP -->
## Usage
```console
$ ./darkscout -t hackthissite.org
```
```console
$ ./darkscout -t hackthissite.org -o hackthesite.txt
```

<!-- ROADMAP -->
## Build
```console
$ git clone https://github.com/DarkSuite/DarkScout
$ cd darkscout
$ cargo build --release
$ cd target/release
$ ./darkscout -t hackthissite.org
```

<!-- ROADMAP -->
## Output
```console
$ ./darkscout -t facebook.com
www.m.facebook.com------------step1-----acc---verify.digi-worx.com
cpanel.the--facebook.com
mail.the--facebook.com
the--facebook.com
webdisk.the--facebook.com
webmail.the--facebook.com
www.the--facebook.com
proxygen_verifier.facebook.com
m.facebook.com-----------n.slickgt.com.br
www.m.facebook.com-----------n.slickgt.com.br
m.facebook.com---------terms-of-service.digi-worx.com
www.m.facebook.com---------terms-of-service.digi-worx.com
m.facebook.com----------step1---confirm.sorgu2.com
www.m.facebook.com----------step1---confirm.sorgu2.com
m.facebook.com------login---step1.akuevi.net
www.m.facebook.com------login---step1.akuevi.net
m.facebook.com-----validate---read---new---tos.yudumay.com
www.m.facebook.com-----validate---read---new---tos.yudumay.com
m.facebook.com----securelogin--confirm.wpthm.ir
www.m.facebook.com----securelogin--confirm.wpthm.ir
news--facebook.com
tihonoff@facebook.com
china--facebook.com
www.china--facebook.com
thefacebook.com

[darkscout]> Successfully scraped 11712 subdomains from facebook.com in 81.238776082s
```

<!-- ROADMAP -->
## Roadmap

* More passive sources for domain reconnaissance
* Builtwith API integration
* HTTP response code checks
* Improved exception handling
* IP validation
* URI parameter parsing
* DB integration via PostgreSQL

See the [open issues](https://github.com/DarkSuite/DarkScout/issues) for a list of proposed features (and known issues).

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to be learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<!-- ISSUES AND REQUESTS -->
## Issues and requests

If you have a problem or a feature request, open an [issue](https://github.com/DarkSuite/DarkScout/issues).

<!-- STARGAZERS -->

## Stargazers over time

[![Stargazers over time](https://starchart.cc/DarkSuite/DarkScout.svg)](https://starchart.cc/DarkSuite/DarkScout)

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/DarkSuite/DarkScout.svg?style=for-the-badge
[contributors-url]: https://github.com/DarkSuite/DarkScout/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/DarkSuite/DarkScout.svg?style=for-the-badge
[forks-url]: https://github.com/DarkSuite/DarkScout/network/members
[stars-shield]: https://img.shields.io/github/stars/DarkSuite/DarkScout.svg?style=for-the-badge
[stars-url]: https://github.com/DarkSuite/DarkScout/stargazers
[issues-shield]: https://img.shields.io/github/issues/DarkSuite/DarkScout.svg?style=for-the-badge
[issues-url]: https://github.com/DarkSuite/DarkScout/issues
[license-shield]: https://img.shields.io/github/license/DarkSuite/DarkScout.svg?style=for-the-badge
[license-url]: https://github.com/DarkSuite/DarkScout/blob/master/LICENSE
