# RProxy2

## Introduction

A simple magisk module to archive local reverse proxy,so you can access discord&steam community pixiv etc .It use [caddy2](https://github.com/caddyserver/caddy/releases) as a local reverse proxy to  transfer data to specified server
<div display="block">
<img src="https://altonhe.github.io/medias/RProxy/1.jpeg" width="30%" height="30%" >
<img src="https://altonhe.github.io/medias/RProxy/2.jpeg" width="30%" height="30%">
<img src="https://altonhe.github.io/medias/RProxy/3.jpeg" width="30%" height="30%">
</div>

### Requirements
* [TrustmeAlready](https://github.com/ViRb3/TrustMeAlready)

## Support

- [x] Pixiv
- [x] Steam Community
- [x] Discord
- [ ] ~~reCAPTCHA~~
- [x] Medium
- [x] Githubusercontent

## Install

This module is still on development,You can download it in release

**make sure you have installed** **[edxposed](https://github.com/ElderDrivers/EdXposed) and [magisk](https://github.com/topjohnwu/Magisk/releases)**

1.install [TrustmeAlready](https://github.com/ViRb3/TrustMeAlready)  to disable SSL verification 

2.flash this mod via magisk

3.add fellow hosts to `/system/etc/hosts`

> if you use adaway to manage hosts, you may add this to rule
> ` https://raw.githubusercontent.com/Altonhe/RProxy2/master/hosts.txt`

```hosts
223.119.248.19 steamuserimages-a.akamaihd.net #UHE_
223.119.248.19 steamcdn-a.akamaihd.net #UHE_
223.119.248.19 steamstore-a.akamaihd.net #UHE_
223.119.248.19 steamcommunity-a.akamaihd.net #UHE_
223.119.248.19 steampipe.akamaized.net #UHE_
223.119.248.19 eaassets-a.akamaihd.net #UHE_
223.119.248.19 humblebundle-a.akamaihd.net #UHE_
223.119.248.19 steamcommunity-a.akamaihd.net #UHE_
127.0.0.1 steamcdn-a.akamaihd.net
127.0.0.1 origin-a.akamaihd.net
127.0.0.1 steam-chat.com
127.0.0.1 steamcommunity.com
127.0.0.1 www.steamcommunity.com
127.0.0.1 discordapp.com
127.0.0.1 dl.discordapp.net
127.0.0.1 media.discordapp.net
127.0.0.1 images-ext-2.discordapp.net
127.0.0.1 images-ext-1.discordapp.net
127.0.0.1 support.discordapp.com
127.0.0.1 url9177.discordapp.com
127.0.0.1 canary-api.discordapp.com
127.0.0.1 cdn-ptb.discordapp.com
127.0.0.1 ptb.discordapp.com
127.0.0.1 status.discordapp.com
127.0.0.1 cdn-canary.discordapp.com
127.0.0.1 cdn.discordapp.com
127.0.0.1 streamkit.discordapp.com
127.0.0.1 i18n.discordapp.com
127.0.0.1 url9624.discordapp.com
127.0.0.1 url7195.discordapp.com
127.0.0.1 merch.discordapp.com
127.0.0.1 printer.discordapp.com
127.0.0.1 canary.discordapp.com
127.0.0.1 apps.discordapp.com
127.0.0.1 pax.discordapp.com
127.0.0.1 www.pixiv.net
127.0.0.1 pixiv.net 
127.0.0.1 ssl.pixiv.net
127.0.0.1 accounts.pixiv.net 
127.0.0.1 touch.pixiv.net
127.0.0.1 oauth.secure.pixiv.net
127.0.0.1 dic.pixiv.net
127.0.0.1 en-dic.pixiv.net 
127.0.0.1 sketch.pixiv.net
127.0.0.1 payment.pixiv.net
127.0.0.1 factory.pixiv.net 
127.0.0.1 comic.pixiv.net  
127.0.0.1 novel.pixiv.net 
127.0.0.1 imgaz.pixiv.net 
127.0.0.1 sensei.pixiv.net
127.0.0.1 fanbox.pixiv.net
127.0.0.1 i.pximg.net
127.0.0.1 source.pixiv.net
127.0.0.1 i1.pixiv.net 
127.0.0.1 i2.pixiv.net 
127.0.0.1 i3.pixiv.net 
127.0.0.1 i4.pixiv.net 
210.129.120.50 app-api.pixiv.net  
74.120.148.207 g-client-proxy.pixiv.net 
210.140.131.159 d.pixiv.org 
210.140.92.135 pixiv.pximg.net  
210.140.92.134 s.pximg.net
127.0.0.1 medium.com
127.0.0.1 cdn-client.medium.com
127.0.0.1 miro.medium.com
127.0.0.1 glyph.medium.com
127.0.0.1 api.medium.com
127.0.0.1 cdn-static-1.medium.com
127.0.0.1 cdn-images-1.medium.com
127.0.0.1 cdn-images-2.medium.com
127.0.0.1 raw.githubusercontent.com
```

4.reboot

Normally you can access [steam](steamcommunity.com) now,**for** **some ROMS you should add additional steps**

```bash 
su -c "/data/local/caddy2/start.sh"
```

## Credits

[Dogfight360](https://www.dogfight360.com/blog/):he's  [steam community 302](https://www.dogfight360.com/blog/686/) inspire this program

[Magisk](https://github.com/topjohnwu/Magisk/releases):make this a module

[Pixiv-Nginx](https://github.com/mashirozx/Pixiv-Nginx):for support rules to proxy pixiv

[TrustmeAlready](https://github.com/ViRb3/TrustMeAlready):solve SSL verification 

[Caddy2](https://github.com/caddyserver/caddy/releases) :A light&speed server to archive local reverse proxy

[newtrek](https://www.jianshu.com/u/a8649c5c66fe):support medium hosts rule

## Thanks

[@Royz](https://github.com/RoyZ-CSGO):for add additional features
