# IPFS In Web Browsers Working Group
[![#ipfs](https://img.shields.io/badge/irc-%23ipfs-brightgreen.svg)](https://webchat.freenode.net/?channels=ipfs) [![#ipfs-in-web-browsers](https://img.shields.io/badge/irc-%23ipfs--in--web--browsers-brightgreen.svg)](https://webchat.freenode.net/?channels=ipfs-in-web-browsers)

> Tracking the Path to getting IPFS and other Decentralized Protocols Natively Supported in Web Browsers.

## Goals

- **Browser Users** - Browser extension exposes IPFS features in a robust and intuitive form
- **Web Developers** -  Ensure smooth experience for web developers in browser contexts
- **Browser Vendors** - Browser developers are addressing requirements of the distributed web

## Current Status

### Browser Extension

[IPFS Companion](https://github.com/ipfs-shipyard/ipfs-companion#ipfs-companion) is a browser extension that simplifies access to IPFS resources and adds support for the
IPFS protocol.  
It runs in <img src="https://unpkg.com/@browser-logos/firefox@2.0.0/firefox_16x16.png" width="16" height="16">Firefox (desktop and android)
and various Chromium-based browsers such as
<img src="https://unpkg.com/@browser-logos/chrome@1.0.4/chrome_16x16.png" width="16" height="16">Chrome or
<img src="https://unpkg.com/@browser-logos/brave@3.0.0/brave_16x16.png" width="16" height="16">Brave.  
Check [its features](https://github.com/ipfs-shipyard/ipfs-companion#features) and [**install it**](https://github.com/ipfs-shipyard/ipfs-companion#install) today!

Exciting ongoing work: [Exposing IPFS API via `window.ipfs`](https://github.com/ipfs-shipyard/ipfs-companion/blob/master/docs/window.ipfs.md#notes-on-exposing-ipfs-api-as-windowipfs),
[mozilla/libdweb](https://github.com/ipfs-shipyard/ipfs-companion/blob/libdweb/docs/libdweb.md):
[native protocol handler](https://github.com/ipfs-shipyard/ipfs-companion/pull/533),
[local DNS-SD discovery and TCP transport](https://github.com/ipfs-shipyard/ipfs-companion/pull/553)

### JavaScript Libraries
Currently in order to run IPFS in a web browser, you have to either bundle [`js-ipfs`](https://github.com/ipfs/js-ipfs) (**full IPFS node in JS**) with your client-side application
or use [`js-ipfs-api`](https://github.com/ipfs/js-ipfs-api) (**HTTP API client library**) to connect to external daemon running on local or remote machine. Make sure to check `/examples` in both repos.

#### ..in Service Workers

- Tracking related work: [#55](https://github.com/ipfs/in-web-browsers/issues/55)
  - Highlight: IPFS gateway fully running on a Service Worker [service-worker-gateway](https://github.com/ipfs-shipyard/service-worker-gateway)

### IPFS Addressing in Web Browsers

See  [this memo](ADDRESSING.md). It specifies current set of URL conventions for the IPFS community.    
We invite everyone to submit questions and suggestions for improvements via issues/PR.

#### DNSLink

DNSLink is mapping a domain name to an IPFS address by means of DNS TXT record. 

Read [DNSLink guide](https://docs.ipfs.io/guides/concepts/dnslink/) for details such as setting it up on your own website and [DNSLink in IPFS Companion](https://github.com/ipfs-shipyard/ipfs-companion/blob/master/docs/dnslink.md) to see additional benefits of using our browser extension.

## Resources

#### PM
- [Meeting Notes](https://github.com/ipfs/in-web-browsers/tree/master/meeting-notes)
- [ROADMAP](ROADMAP.md)
    - [Quarterly Objectives and Key Results (OKRs)](https://github.com/ipfs/pm/blob/master/OKR/WB.md)
- [![Waffle.io - Columns and their card count](https://badge.waffle.io/ipfs/in-web-browsers.svg?columns=all)](https://waffle.io/ipfs/in-web-browsers)

#### Related Endeavours

- [IPFS Companion](https://github.com/ipfs-shipyard/ipfs-companion) - A Web Extension to give your browser super powers.
- [IPFS WebUI](https://github.com/ipfs-shipyard/ipfs-webui) - The IPFS Dashboard
- [js-ipfs](https://github.com/ipfs/js-ipfs) - IPFS implementation in JavaScript
- [HTTP API Documentation](https://docs.ipfs.io/reference/api/http/) - When an IPFS node (go-ipfs or js-ipfs) is running as a daemon, it exposes an HTTP API that allows you to control the node and run the same commands you can from the command line.
    - [js-ipfs-api](https://github.com/ipfs/js-ipfs) - A client library for the IPFS HTTP API, implemented in JavaScript
- [IPFS GUI Working Group](https://github.com/ipfs-shipyard/pm-ipfs-gui) - Unifying and leveling up IPFS interfaces and the user journey into the Distributed Web
- [Dynamic Data and Capabilities in IPFS Working Group](https://github.com/ipfs/dynamic-data-and-capabilities) -  building blocks that enable collaborative applications, providing solutions for security, identity, access control, concurrency, synchronization, offline and near-real-time collaboration on top of IPFS
