
[![GitHub issues](https://img.shields.io/github/issues/Bypass-Network/BypassIB)](https://github.com/Bypass-Network/BypassIB/issues)
[![GitHub license](https://img.shields.io/github/license/Bypass-Network/BypassIB)](https://github.com/Bypass-Network/BypassIB/blob/main/LICENSE)


## Documentation

- [Overview](#overview)
  - [Supported Sites](#supported-sites)
  - [Features](#features)
  - [Pages](#pages)
- [Setup](#setup)
  - [Locally](#locally)
  - [Deploy](#deploy)
  - [Proxies](#proxies)
  - [Configuration](#configuration)
- [Support](#support)
  - [FAQ](#faq)
  - [Contact](#contact)
- [More](#more)
  - [Proxy Sources](#proxy-sources)
  - [Credits](#credits)
  - [Contributing](#contributing)

## Overview

### Supported Sites

- google.com
- discord.com (might work)
- youtube.com
- invidio.us
- reddit.com
- 1v1.lol

### Features

- All the best proxies
- Nice game library
- Tab cloaking and other cool features
- Basic auth
- Customizable CSS
- Installable PWA
- Build in youtube downloader


## Setup

**Please Note: Aero needs to be on a subdomain, see [proxies](#proxies) for more info**



### Proxies

Some of the proxies on Tsunami are hosted on subdomains, deploy the correct proxy for Tsunami to work

Palladium and Corrosion are hosted locally, so you don't need a subdomain

[a.example.com (Aero)](https://github.com/titaniumnetwork-dev/aero)

[Locally (Palladium)](https://github.com/FogNetwork/Palladium)

[Locally (Corrosion)](https://github.com/titaniumnetwork-dev/Corrosion)

### Configuration

**config.json**

```json
{
    "port": "8080",
    "auth": "false",
    "username": "user",
    "password": "secret"
}
```

`"port": "8080"` Changes the port 

`"auth": "false"` Basic authentication, set to true or false

`"username"` Username for authentication

`"password"` Password for authentication

**/public/js/go.js**

```js
var palladiumproxy = window.location.protocol + "//" + window.location.hostname + "/palladium/gateway?url="

var corrosionproxy = window.location.protocol + "//" + window.location.hostname + "/corrosion/gateway?url="

var aeroproxy = window.location.protocol + "//" + "a." + window.location.hostname + "/http/"
```
`palladiumproxy` Location for Palladium proxy

`corrosionproxy` Location for Corrosion proxy

`aeroproxy` Location for Aero proxy

Custom Proxy Example:

```js
var palladiumproxy = "https://example.com/palladium/"
```

## Support

### FAQ


**Captcha not working/issues**

Captcha is only supported on Womginx, though the support is limited

**Why is Discord not working properly?**

Try using Palladium or Corrosion. Refreshing the page might help



## More


### Proxy Sources

[Palladium](https://github.com/FogNetwork/Palladium)

[Corrosion](https://github.com/titaniumnetwork-dev/Corrosion)

[Modified Corrosion](https://github.com/BinBashBanana/Corrosion-Heroku)

[Aero](https://github.com/titaniumnetwork-dev/aero)

[Womginx](https://github.com/binary-person/womginx) (Not Used)

[PyDodge](https://github.com/BinBashBanana/PyDodge) (Not Used)

[Alloy](https://github.com/titaniumnetwork-dev/alloy) (Not Used)

[SystemYA](https://github.com/sysce/proxy) (Not Used)

[Via](https://github.com/hypothesis/via) (Not Used)

[Node Unblocker](https://github.com/nfriedly/node-unblocker) (Not Used)

[Powermouse](https://github.com/titaniumnetwork-dev/powermouse) (Not Used)

### Credits

[Jackson Development](https://github.com/JacksonDevelopment) - Owner and Main Developer

[Nebelung](https://github.com/Nebelung-Dev) - Owner Of Tsunami And Main Developer

[EnderKingJ](https://github.com/EnderKingJ) - Proxy Developer

[Quite A Fancy Emerald](https://github.com/QuiteAFancyEmerald) - Holy Unblocker King

[Caracal.js](https://github.com/caracal-js) - Proxy Developer

[Avad3](https://github.com/Avad3) - Developer

[BinBashBanana](https://github.com/BinBashBanana) - Game Library and PyDodge 

[Binary Person](https://github.com/binary-person) - Creator of Womginx

[Divide](https://github.com/vibedivide) - SystemYA and Chatbox Creator

[Shirt](https://github.com/shirt-dev) - Proxy Developer

### Contributing

See [CONTRIBUTING.md](https://github.com/FogNetwork/Tsunami/blob/main/CONTRIBUTING.md)

Special Thanks To Quite A Fancy Emerald, Inspiration for Tsunami
