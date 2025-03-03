<br />
![Image of DockServer](/img/logo.png)

[![Website: https://dockserver.io](https://img.shields.io/badge/Website-https%3A%2F%2Fdockserver.io-blue.svg?style=for-the-badge&colorB=177DC1&label=website)](https://dockserver.io)
[![Discord: https://discord.gg/A7h7bKBCVa](https://img.shields.io/badge/Discord-gray.svg?style=for-the-badge)](https://discord.gg/A7h7bKBCVa)
[![License: GPL 3](https://img.shields.io/badge/License-GPL%203-blue.svg?style=for-the-badge&colorB=177DC1&label=license)](LICENSE)
<br />
<br />

<p align="center"><a href="https://github.com/crazy-max/docker-rtorrent-rutorrent" target="_blank"><img height="128" src="https://raw.githubusercontent.com/crazy-max/docker-rtorrent-rutorrent/master/.github/docker-rtorrent-rutorrent.jpg"></a></p>

<p align="center">
  <a href="https://hub.docker.com/r/crazymax/rtorrent-rutorrent/tags?page=1&ordering=last_updated"><img src="https://img.shields.io/github/v/tag/crazy-max/docker-rtorrent-rutorrent?label=version&style=flat-square" alt="Latest Version"></a>
  <a href="https://github.com/crazy-max/docker-rtorrent-rutorrent/actions?workflow=build"><img src="https://img.shields.io/github/workflow/status/crazy-max/docker-rtorrent-rutorrent/build?label=build&logo=github&style=flat-square" alt="Build Status"></a>
  <a href="https://hub.docker.com/r/crazymax/rtorrent-rutorrent/"><img src="https://img.shields.io/docker/stars/crazymax/rtorrent-rutorrent.svg?style=flat-square&logo=docker" alt="Docker Stars"></a>
  <a href="https://hub.docker.com/r/crazymax/rtorrent-rutorrent/"><img src="https://img.shields.io/docker/pulls/crazymax/rtorrent-rutorrent.svg?style=flat-square&logo=docker" alt="Docker Pulls"></a>
  <br /><a href="https://github.com/sponsors/crazy-max"><img src="https://img.shields.io/badge/sponsor-crazy--max-181717.svg?logo=github&style=flat-square" alt="Become a sponsor"></a>
  <a href="https://www.paypal.me/crazyws"><img src="https://img.shields.io/badge/donate-paypal-00457c.svg?logo=paypal&style=flat-square" alt="Donate Paypal"></a>
</p>

## About

[rTorrent](https://github.com/rakshasa/rtorrent) and [ruTorrent](https://github.com/Novik/ruTorrent) Docker image based on Alpine Linux.<br />

## Features

- Run as non-root user
- Multi-platform image
- Latest [rTorrent](https://github.com/rakshasa/rtorrent) / [libTorrent](https://github.com/rakshasa/libtorrent) release compiled from source
- Latest [ruTorrent](https://github.com/Novik/ruTorrent) release
- Name resolving enhancements with [c-ares](https://github.com/rakshasa/rtorrent/wiki/Performance-Tuning#rtrorrent-with-c-ares) for asynchronous DNS requests (including name resolves)
- Enhanced [rTorrent config](rootfs/tpls/.rtorrent.rc) and bootstraping with a [local config](rootfs/tpls/etc/rtorrent/.rtlocal.rc)
- WAN IP address automatically resolved for reporting to the tracker
- XMLRPC through nginx over SCGI socket (basic auth optional)
- WebDAV on completed downloads (basic auth optional)
- Ability to add a custom ruTorrent plugin / theme
- Allow persisting specific configuration for ruTorrent plugins
- ruTorrent [GeoIP2 plugin](https://github.com/Micdu70/geoip2-rutorrent)
- [mktorrent](https://github.com/Rudde/mktorrent) installed for ruTorrent create plugin
- [Traefik](https://github.com/containous/traefik-library-image) Docker image as reverse proxy and creation/renewal of Let's Encrypt certificates (see [this template](examples/traefik))
- [geoip-updater](https://github.com/crazy-max/geoip-updater) Docker image to download MaxMind's GeoIP2 databases on a time-based schedule for geolocation

## Support

Kindly report any issues/broken-parts/bugs on [github](https://github.com/dockserver/dockserver/issues) or [discord](https://discord.gg/A7h7bKBCVa)

- Join our [![Discord: https://discord.gg/A7h7bKBCVa](https://img.shields.io/badge/Discord-gray.svg?style=for-the-badge)](https://discord.gg/A7h7bKBCVa) for Support
