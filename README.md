# Awesome WireGuard with stars

<br />
<div align="center">
  <img width="581" src="https://raw.githubusercontent.com/cedrickchee/awesome-wireguard/master/assets/banner.png">
</div>
<br />

> A curated list of WireGuard tools, projects, and resources.

WireGuard® - fast, modern, secure VPN tunnel.

*You can see the updates on [Twitter](https://twitter.com/awesome-wireguard) (coming soon)*

> Please, help organize these resources so that they are easy to find and understand for newcomers. See how to [Contribute][contributing] for tips!

*If you see a link here that is not (any longer) a good fit, you can fix it by submitting a [pull request][editreadme] to improve this file. Thank you!*

***

## Status Badges

We use emoji to determine repository status.

:green\_circle: **active** repos (last commit date is less than 3 months)

:yellow\_circle: **stale** repos (last commit date is more than 6 months)

:red\_circle: **inactive** repos (last commit date is more than 1 year)

:black\_circle: repos that **were superseded**

:blue\_square: repos that **were code completed**

:grey\_question: repos that **weren't found** (broken link)

***

## Contents

<details>

<summary><b>Expand Table of Contents</b></summary>

* [What is WireGuard](#what-is-wireguard)
* [Official Resources](#official-resources)
* [Where to Start](#where-to-start)
* [Projects](#projects)
  * [Tools](#tools)
  * [Mesh Network](#mesh-network)
  * [Deployment](#deployment)
    * [Container](#container)
  * Monitoring
  * Security
    * Protocol
    * Encryption
  * Runtime
  * [User Interface](#user-interface)
    * [Terminal / CLI](#terminal--cli)
    * [Web](#web)
    * [Desktop](#desktop)
    * [Dashboards](#dashboards)
  * Development
    * Development Environment
    * Testing
    * Boilerplate
  * Homeserver
  * [Services based on WireGuard](#services-based-on-wireguard)
    * [Cloud Service](#cloud-service)
    * [VPN](#vpn)
  * [Extensions / Plugins](#extensions--plugins)
  * Optimization
  * Language Bindings
  * [Alternative Implementations](#alternative-implementations)
* [Useful Resources](#useful-resources)
  * [Blog Posts](#blog-posts)
  * [Articles](#articles)
  * [Demos and Examples](#demos-and-examples)
  * [Good Tips](#good-tips)
  * [Tutorials](#tutorials)
  * [Videos](#videos)
  * [Books](#books)
  * [Podcasts and Interviews](#podcasts-and-interviews)
  * [Presentations](#presentations)
  * [Newsletters](#newsletters)
* Uncategorized
* [Communities and Meetups](#communities-and-meetups)
  * [English](#english)
  * Chinese

</details>

***

## What is WireGuard

> WireGuard® is an extremely simple yet fast and modern VPN that utilizes
> state-of-the-art cryptography. It aims to be faster, simpler, leaner, and more
> useful than IPsec, while avoiding the massive headache. It intends to be
> considerably more performant than OpenVPN. WireGuard is designed as a general
> purpose VPN for running on embedded interfaces and super computers alike,
> fit for many different circumstances. Initially released for the Linux kernel,
> it is now cross-platform (Windows, macOS, BSD, iOS, Android) and widely
> deployable. It is currently under heavy development, but already it might
> be regarded as the most secure, easiest to use, and simplest VPN solution
> in the industry.

*Source: [Official WireGuard project website](https://www.wireguard.com/)*

## Official Resources

* [Next Generation Kernel Network Tunnel](https://www.wireguard.com/papers/wireguard.pdf) \[PDF] - Whitepaper.
* [WireGuard Docs](https://github.com/pirate/wireguard-docs) ⭐ 5,044 | 🐛 0 | 🌐 Shell | 📅 2026-03-21 - Unofficial WireGuard documentation.

## Where to Start

* [Quick Start](https://www.wireguard.com/quickstart/) - Official quick start.

***

## Projects

### Tools

* [wireproxy](https://github.com/octeep/wireproxy) ⭐ 5,753 | 🐛 80 | 🌐 Go | 📅 2026-07-30 - A userspace WireGuard client that connects to a WireGuard peer, and exposes a SOCKS5 proxy. (Use cases: Setting up WG as a VPN requires special privilege. It tells the kernel to create a special network interface to handle WG connection. This can get messy if you do not have any special permission (i.e., root), if you do not have proper firewall configuration, or if you want to connect to multiple WG peers at once. wireproxy static tunneling is basically openssh `-D`, which supports SOCKS5 protocols.)
  ![GitHub last commit](https://img.shields.io/github/last-commit/octeep/wireproxy?style=flat-square\&color=informational) :green\_circle:
* [coder/wush](https://github.com/coder/wush) ⭐ 1,457 | 🐛 22 | 🌐 Go | 📅 2025-07-28 - Simplest and fastest way to transfer files between computers via WireGuard.
  ![GitHub last commit](https://img.shields.io/github/last-commit/coder/wush?style=flat-square\&color=informational) :green\_circle:
* [easy-wg-quick](https://github.com/burghardt/easy-wg-quick) ⭐ 1,118 | 🐛 0 | 🌐 Shell | 📅 2026-08-10 - Creates Wireguard configuration for hub and peers with ease.
  ![GitHub last commit](https://img.shields.io/github/last-commit/burghardt/easy-wg-quick?style=flat-square\&color=informational) :green\_circle:
* [sandialabs/wiretap](https://github.com/sandialabs/wiretap) ⭐ 1,105 | 🐛 12 | 🌐 Go | 📅 2026-07-30 - Wiretap is a transparent, VPN-like proxy server that tunnels traffic via WireGuard and requires no special privileges to run.
  ![GitHub last commit](https://img.shields.io/github/last-commit/sandialabs/wiretap?style=flat-square\&color=informational) :green\_circle:
* [onetun](https://github.com/aramperes/onetun) ⭐ 1,042 | 🐛 17 | 🌐 Rust | 📅 2025-10-20 - A user-space WireGuard port-forwarder -- access ports running on peers in your WireGuard network from any device; without having to install WireGuard locally or without root access (no iptables configs).
  ![GitHub last commit](https://img.shields.io/github/last-commit/aramperes/onetun?style=flat-square\&color=informational) :green\_circle:
* [wgctrl](https://github.com/WireGuard/wgctrl-go) ⭐ 913 | 🐛 26 | 🌐 Go | 📅 2024-12-31 - Package wgctrl enables control of WireGuard interfaces on multiple platforms.
  ![GitHub last commit](https://img.shields.io/github/last-commit/WireGuard/wgctrl-go?style=flat-square\&color=informational) :red\_circle:
* [dsnet](https://github.com/naggie/dsnet/) ⭐ 754 | 🐛 17 | 🌐 Go | 📅 2026-05-17 - Simple command to manage a centralised wireguard VPN. Think wg-quick but quicker: key generation + address allocation.
  ![GitHub last commit](https://img.shields.io/github/last-commit/naggie/dsnet?style=flat-square\&color=informational) :green\_circle:
* [wireguard-manager-and-api](https://github.com/Mawthuq-Software/wireguard-manager-and-api) ⭐ 178 | 🐛 3 | 🌐 Go | 📅 2022-06-23 - A tool for rotating the keys on peers to increase their privacy by removing their IP address from memory.
  ![GitHub last commit](https://img.shields.io/github/last-commit/Mawthuq-Software/wireguard-manager-and-api?style=flat-square\&color=informational) :red\_circle:
* [wgzero](https://github.com/finzzz/wgzero) ⚠️ Archived - Zero overhead wireguard setup.
  ![GitHub last commit](https://img.shields.io/github/last-commit/finzzz/wgzero?style=flat-square\&color=informational) :red\_circle:
* [wg-make](https://github.com/tevino/wg-make) ⭐ 22 | 🐛 0 | 🌐 Go | 📅 2020-06-05 - A tool to help set up WireGuard based networks. Currently, it generates configurations for peers according to a single configuration file.
  ![GitHub last commit](https://img.shields.io/github/last-commit/tevino/wg-make?style=flat-square\&color=informational) :red\_circle:
* [wg-quick](https://git.zx2c4.com/wireguard-tools/about/src/man/wg-quick.8) - Official cross-platform tool to set up a WireGuard interface simply.

### Mesh Network

* [Headscale](https://github.com/juanfont/headscale) ⭐ 42,892 | 🐛 142 | 🌐 Go | 📅 2026-07-30 - An open source implementation of the Tailscale control server.
  ![GitHub last commit](https://img.shields.io/github/last-commit/juanfont/headscale?style=flat-square\&color=informational) :green\_circle:
* [NetBird](https://github.com/netbirdio/netbird) ⭐ 28,415 | 🐛 1,577 | 🌐 Go | 📅 2026-08-16 - (Previously Wiretrustee) NetBird is an open-source VPN management platform built on top of WireGuard® making it easy to create secure private networks for your organization or home. Technically, it creates an overlay network using ICE protocol (WebRTC) to negotiate P2P connections and WG (kernel module, when possible) to create a fast and encrypted tunnel between machines, falling back to relay (TURN) in case a P2P connection isn't possible. Pretty much just a client app is needed, the rest is done by the software. Their vision is to go beyond traditional VPN by bringing advanced NetSec (Zero Trust security model) like OpenZiti.
  ![GitHub last commit](https://img.shields.io/github/last-commit/netbirdio/netbird?style=flat-square\&color=informational) :green\_circle:
* [gravitl/netmaker](https://github.com/gravitl/netmaker) ⭐ 11,754 | 🐛 227 | 🌐 Go | 📅 2026-08-14 - Netmaker is a VPN platform that automates WireGuard from homelab to enterprise. The key distinctions in their solutions are: fast because it can use kernel WireGuard (instead of userspace WireGuard, which is slower), tailored towards the Cloud and Kubernetes, and fully self-hostable.
  ![GitHub last commit](https://img.shields.io/github/last-commit/gravitl/netmaker?style=flat-square\&color=informational) :green\_circle:
* [innernet](https://github.com/tonarino/innernet) ⭐ 5,523 | 🐛 83 | 🌐 Rust | 📅 2026-07-28 - A private network system that uses WireGuard under the hood. It is similar in its goals to Slack's nebula or Tailscale.
  ![GitHub last commit](https://img.shields.io/github/last-commit/tonarino/innernet?style=flat-square\&color=informational) :green\_circle:
* [Kilo](https://github.com/squat/kilo) ⭐ 2,280 | 🐛 94 | 🌐 Go | 📅 2026-08-11 - Kilo is a multi-cloud network overlay built on WireGuard and designed for Kubernetes (k8s + wg = kg).
  ![GitHub last commit](https://img.shields.io/github/last-commit/squat/kilo?style=flat-square\&color=informational) :green\_circle:
* [wesher](https://github.com/costela/wesher) ⭐ 988 | 🐛 19 | 🌐 Go | 📅 2025-02-17 - wesher creates and manages an encrypted mesh overlay network across a group of nodes.
  ![GitHub last commit](https://img.shields.io/github/last-commit/costela/wesher?style=flat-square\&color=informational) :green\_circle:
* [HarvsG/WireGuardMeshes](https://github.com/HarvsG/WireGuardMeshes) ⭐ 651 | 🐛 9 | 📅 2024-12-15 - Compare WireGuard mesh tools.
  ![GitHub last commit](https://img.shields.io/github/last-commit/HarvsG/WireGuardMeshes?style=flat-square\&color=informational) :green\_circle:
* [svenstaro/wiresmith](https://github.com/svenstaro/wiresmith) ⭐ 147 | 🐛 2 | 🌐 Rust | 📅 2026-08-01 - Auto-config WireGuard clients into a mesh ![GitHub last commit](https://img.shields.io/github/last-commit/svenstaro/wiresmith?style=flat-square\&color=informational) :green\_circle:
* [Tailscale](https://tailscale.com/) - Tailscale is a WireGuard-based app that makes secure, private networks easy for teams of any scale.

### Deployment

* [Algo VPN](https://github.com/trailofbits/algo) ⭐ 30,360 | 🐛 77 | 🌐 Python | 📅 2026-08-12 - Set up a DIY/personal VPN in the cloud. It is a set of Ansible scripts that simplify the setup of a personal WireGuard and IPsec VPN, open-sourced by Trail of Bits.
  ![GitHub last commit](https://img.shields.io/github/last-commit/trailofbits/algo?style=flat-square\&color=informational) :green\_circle:
* [Firezone](https://github.com/firezone/firezone) ⭐ 9,032 | 🐛 410 | 🌐 Elixir | 📅 2026-08-16 - An open-source WireGuard-based VPN server alternative to OpenVPN Access Server. You can self-host this.
  ![GitHub last commit](https://img.shields.io/github/last-commit/firezone/firezone?style=flat-square\&color=informational) :green\_circle:
* [WireHole](https://github.com/IAmStoxe/wirehole) ⭐ 4,967 | 🐛 60 | 📅 2026-08-14 - A combination of WireGuard, Pi-hole, and Unbound in a docker-compose project with the intent of enabling users to quickly and easily create a personally managed full or split-tunnel WireGuard VPN with ad blocking capabilities thanks to Pi-hole, and DNS caching, additional privacy options, and upstream providers via Unbound.
  ![GitHub last commit](https://img.shields.io/github/last-commit/IAmStoxe/wirehole?style=flat-square\&color=informational) :red\_circle:
* [seashell/drago](https://github.com/seashell/drago) ⭐ 1,119 | 🐛 34 | 🌐 Go | 📅 2023-10-13 - A self-hosted and flexible configuration manager designed to make it simple to configure secure network overlays spanning heterogeneous nodes via a Web UI.
  ![GitHub last commit](https://img.shields.io/github/last-commit/seashell/drago?style=flat-square\&color=informational) :red\_circle:
* [Cloudblock](https://github.com/chadgeary/cloudblock) ⭐ 860 | 🐛 2 | 🌐 HCL | 📅 2024-07-06 - Deploys WireGuard VPN, Pi-Hole DNS Ad-blocking, and DNS over HTTPS in a cloud provider - or locally - using Terraform and Ansible.
  ![GitHub last commit](https://img.shields.io/github/last-commit/chadgeary/cloudblock?style=flat-square\&color=informational) :green\_circle:
* [ansible-role-wireguard](https://github.com/githubixx/ansible-role-wireguard) ⭐ 693 | 🐛 22 | 🌐 Jinja | 📅 2026-06-15 - Ansible role for installing WireGuard VPN. Supports Ubuntu, Debian, Archlinx, Fedora and CentOS.
  ![GitHub last commit](https://img.shields.io/github/last-commit/githubixx/ansible-role-wireguard?style=flat-square\&color=informational) :green\_circle:
* [freifunkMUC/wg-access-server](https://github.com/freifunkMUC/wg-access-server) ⭐ 687 | 🐛 26 | 🌐 Go | 📅 2026-08-12 - An all-in-one WireGuard VPN solution with a Web UI for connecting devices. This project aims to deliver a simple VPN solution for developers, homelab enthusiasts and anyone else feeling adventurous.
  ![GitHub last commit](https://img.shields.io/github/last-commit/freifunkMUC/wg-access-server?style=flat-square\&color=informational) :green\_circle:
* [WirtBot](https://github.com/b-m-f/WirtBot) ⚠️ Archived - Think of it as a component that will allow you to extend your LAN over the Internet. WirtBot simplifies the process of creating your own private network into 3 steps. No registration, no accounts - Just a network that belongs to you. And it will always be completely free (except for the server/VPS you run it on).
  ![GitHub last commit](https://img.shields.io/github/last-commit/b-m-f/WirtBot?style=flat-square\&color=informational) :red\_circle:
* [Autowire](https://github.com/elghazal-a/autowire) ⭐ 217 | 🐛 2 | 🌐 Go | 📅 2022-02-26 - Automatically configure Wireguard interfaces in distributed system. It supports Consul as backend.
  ![GitHub last commit](https://img.shields.io/github/last-commit/elghazal-a/autowire?style=flat-square\&color=informational) :red\_circle:
* [terraform-aws-wireguard](https://github.com/jmhale/terraform-aws-wireguard) - Terraform module to deploy WireGuard on AWS.
  ![GitHub last commit](https://img.shields.io/github/last-commit/jmhale/terraform-aws-wireguard?style=flat-square\&color=informational) :red\_circle:

#### Container

* [linuxserver/docker-wireguard](https://github.com/linuxserver/docker-wireguard) ⭐ 3,631 | 🐛 2 | 🌐 Dockerfile | 📅 2026-08-06 - A WireGuard container image brought to you by LinuxServer.io. Not all image authors are as great as LinuxServer.io team.
  ![GitHub last commit](https://img.shields.io/github/last-commit/linuxserver/docker-wireguard?style=flat-square\&color=informational) :green\_circle:
* [cmulk/wireguard-docker](https://github.com/cmulk/wireguard-docker) ⚠️ Archived - A Docker image and configuration for a simple personal VPN, used for the goal of security over insecure (public) networks, not necessarily for Internet anonymity. There are currently 3 flavors.
  ![GitHub last commit](https://img.shields.io/github/last-commit/cmulk/wireguard-docker?style=flat-square\&color=informational) :red\_circle:
* [masipcat/wireguard-go-docker](https://github.com/masipcat/wireguard-go-docker) ⭐ 209 | 🐛 6 | 🌐 Go | 📅 2026-03-21 - WireGuard docker image.
  ![GitHub last commit](https://img.shields.io/github/last-commit/masipcat/wireguard-go-docker?style=flat-square\&color=informational) :green\_circle:
* [bitwister/twine](https://github.com/bitwister/twine) ⭐ 14 | 🐛 11 | 🌐 TypeScript | 📅 2025-08-25 - Label based route/port forwarding management tool for Docker that can be used to easily route traffic of containers from/to Wireguard container, while preserving full network isolation. ![GitHub last commit](https://img.shields.io/github/last-commit/bitwister/twine?style=flat-square\&color=informational)

### Monitoring

* [MindFlavor/prometheus\_wireguard\_exporter](https://github.com/MindFlavor/prometheus_wireguard_exporter) ⭐ 601 | 🐛 36 | 🌐 Rust | 📅 2023-10-24 - A Prometheus exporter for WireGuard, very light on your server resources.
  ![GitHub last commit](https://img.shields.io/github/last-commit/MindFlavor/prometheus_wireguard_exporter?style=flat-square\&color=informational) :red\_circle:

### Security

#### Protocol

#### Encryption

### Runtime

### User Interface

#### Terminal / CLI

* [angristan/WireGuard-install](https://github.com/angristan/wireguard-install) ⭐ 11,236 | 🐛 125 | 🌐 Shell | 📅 2026-05-02 - WireGuard VPN installer for Linux servers.
  ![GitHub last commit](https://img.shields.io/github/last-commit/angristan/wireguard-install?style=flat-square\&color=informational) :red\_circle:
* [PiVPN](https://github.com/pivpn/pivpn) ⭐ 8,035 | 🐛 16 | 🌐 Shell | 📅 2026-07-30 - The Simplest VPN installer (scripts), designed for Raspberry Pi.
  ![GitHub last commit](https://img.shields.io/github/last-commit/pivpn/pivpn?style=flat-square\&color=informational) :green\_circle:
* [tun2socks](https://github.com/xjasonlyu/tun2socks) ⭐ 5,445 | 🐛 14 | 🌐 Go | 📅 2026-08-08 - Powered by gVisor TCP/IP stack.
  ![GitHub last commit](https://img.shields.io/github/last-commit/xjasonlyu/tun2socks?style=flat-square\&color=informational) :green\_circle:
* [Nyr/wireguard-install](https://github.com/Nyr/wireguard-install) ⭐ 4,920 | 🐛 0 | 🌐 Shell | 📅 2026-07-02 - WireGuard road warrior installer for Ubuntu, Debian, CentOS and Fedora.
  ![GitHub last commit](https://img.shields.io/github/last-commit/Nyr/wireguard-install?style=flat-square\&color=informational) :green\_circle:
* [WireGuard-Manager](https://github.com/complexorganizations/wireguard-manager) ⭐ 1,857 | 🐛 34 | 🌐 Shell | 📅 2025-12-15 - enables you to build your own vpn under a minute.
  ![GitHub last commit](https://img.shields.io/github/last-commit/complexorganizations/wireguard-manager?style=flat-square\&color=informational) :green\_circle:
* [wg-meshconf](https://github.com/k4yt3x/wg-meshconf) ⭐ 1,048 | 🐛 10 | 🌐 Python | 📅 2024-05-05 - WireGuard full mesh configuration generator.
  ![GitHub last commit](https://img.shields.io/github/last-commit/k4yt3x/wg-meshconf?style=flat-square\&color=informational) :red\_circle:
* [AndrianBdn/wg-cmd](https://github.com/AndrianBdn/wg-cmd) ⭐ 223 | 🐛 2 | 🌐 Go | 📅 2026-07-07 - WG Commander is a TUI for a simple WireGuard VPN setup. UI, QR Codes, Setup Wizard in the terminal.
  ![GitHub last commit](https://img.shields.io/github/last-commit/AndrianBdn/wg-cmd?style=flat-square\&color=informational) :green\_circle:
* [psyhomb/wireguard-tools](https://github.com/psyhomb/wireguard-tools) ⭐ 197 | 🐛 2 | 🌐 Shell | 📅 2023-11-10 - WireGuard helper scripts.
  ![GitHub last commit](https://img.shields.io/github/last-commit/psyhomb/wireguard-tools?style=flat-square\&color=informational) :red\_circle:
* [docker-wireguard-socks-proxy](https://github.com/kizzx2/docker-wireguard-socks-proxy) ⭐ 171 | 🐛 7 | 🌐 Dockerfile | 📅 2019-10-08 - Expose a WireGuard tunnel as a SOCKS5 proxy.
  ![GitHub last commit](https://img.shields.io/github/last-commit/kizzx2/docker-wireguard-socks-proxy?style=flat-square\&color=informational) :red\_circle:
* [guard](https://github.com/stellarproject/guard) ⭐ 84 | 🐛 2 | 🌐 Go | 📅 2021-05-03 - A gRPC server for managing wireguard tunnels.
  ![GitHub last commit](https://img.shields.io/github/last-commit/stellarproject/guard?style=flat-square\&color=informational) :red\_circle:
* [Wiresteward](https://github.com/utilitywarehouse/wiresteward) ⭐ 84 | 🐛 3 | 🌐 Go | 📅 2026-08-11 - A WireGuard peer manager with OAuth2 authentication.
  ![GitHub last commit](https://img.shields.io/github/last-commit/utilitywarehouse/wiresteward?style=flat-square\&color=informational) :green\_circle:
* [wgctl](https://github.com/apognu/wgctl) ⭐ 68 | 🐛 4 | 🌐 Go | 📅 2023-03-06 - Utility to configure and manage your WireGuard tunnels.
  ![GitHub last commit](https://img.shields.io/github/last-commit/apognu/wgctl?style=flat-square\&color=informational) :red\_circle:
* [b-m-f/wired](https://github.com/b-m-f/wired) ⭐ 17 | 🐛 0 | 🌐 Rust | 📅 2026-04-09 - WireGuard network configuration generator with support for multiple topologies written in Rust
  ![GitHub last commit](https://img.shields.io/github/last-commit/b-m-f/wired?style=flat-square\&color=informational) :red\_circle:
* [muiquq/wgcfghelp](https://github.com/muqiuq/wgcfghelp) ⭐ 1 | 🐛 0 | 🌐 C# | 📅 2024-09-09 - Lightweight single binary CLI tool, roadwarrior peer management, config file generator, QR code image generator, MikroTik command generator. ![GitHub last commit](https://img.shields.io/github/last-commit/muqiuq/wgcfghelp?style=flat-square\&color=informational) :green\_circle:
* [WireGuard in NetworkManager](https://blogs.gnome.org/thaller/2019/03/15/wireguard-in-networkmanager/) - Linux NetworkManager has WireGuard support.

#### Web

* [wg-easy/wg-easy](https://github.com/wg-easy/wg-easy) ⭐ 26,672 | 🐛 50 | 🌐 TypeScript | 📅 2026-08-14 - The easiest way to run WireGuard VPN + Web-based Admin UI.
  ![GitHub last commit](https://img.shields.io/github/last-commit/Wg-easy/wg-easy?style=flat-square\&color=informational) :green\_circle:
* [wireguard-ui](https://github.com/ngoduykhanh/wireguard-ui) ⭐ 5,141 | 🐛 210 | 🌐 Go | 📅 2024-08-09 - Simple, have empty interfaces for authentication
  ![GitHub last commit](https://img.shields.io/github/last-commit/ngoduykhanh/wireguard-ui?style=flat-square\&color=informational) :yellow\_circle:
* [Subspace](https://github.com/subspacecommunity/subspace) ⭐ 1,805 | 🐛 65 | 🌐 HTML | 📅 2024-06-13 - A simple WireGuard VPN server GUI.
  ![GitHub last commit](https://img.shields.io/github/last-commit/subspacecommunity/subspace?style=flat-square\&color=informational) :red\_circle:
* [h44z/wg-portal](https://github.com/h44z/wg-portal) ⭐ 1,796 | 🐛 28 | 🌐 Go | 📅 2026-08-11 - Supports LDAP and more
  ![GitHub last commit](https://img.shields.io/github/last-commit/h44z/wg-portal?style=flat-square\&color=informational) :green\_circle:
* [vx3r/wg-gen-web](https://github.com/vx3r/wg-gen-web) ⭐ 1,704 | 🐛 49 | 🌐 Go | 📅 2024-05-07 - Simple Web based configuration generator for WireGuard.
  ![GitHub last commit](https://img.shields.io/github/last-commit/vx3r/wg-gen-web?style=flat-square\&color=informational) :red\_circle:
* [WireGuard UI](https://github.com/EmbarkStudios/wg-ui) ⚠️ Archived - WireGuard Web UI for self-serve client configurations, with optional auth.
  ![GitHub last commit](https://img.shields.io/github/last-commit/EmbarkStudios/wg-ui?style=flat-square\&color=informational) :red\_circle:
* [brsyuksel/wghttp](https://github.com/brsyuksel/wghttp/) ⭐ 23 | 🐛 2 | 🌐 Rust | 📅 2026-07-27 - A http server helps managing wireguard devices and peers on kernel level.
  ![GitHub last commit](https://img.shields.io/github/last-commit/brsyuksel/wghttp?style=flat-square\&color=informational) :green\_circle:

#### Desktop

* [TunnlTo/desktop-app](https://github.com/TunnlTo/desktop-app) ⭐ 1,963 | 🐛 2 | 📅 2026-04-14 - TunnlTo is a lightweight, fast, Windows WireGuard VPN client built for split tunneling.
  ![GitHub last commit](https://img.shields.io/github/last-commit/TunnlTo/desktop-app?style=flat-square\&color=informational) :green\_circle:
* [network-manager-wireguard](https://github.com/max-moser/network-manager-wireguard) ⭐ 468 | 🐛 45 | 🌐 C | 📅 2023-06-14 - Network-Manager VPN Plugin for WireGuard.
  ![GitHub last commit](https://img.shields.io/github/last-commit/max-moser/network-manager-wireguard?style=flat-square\&color=informational) :red\_circle:
* [WireGuardStatusbar](https://github.com/aequitas/macos-menubar-wireguard) ⭐ 271 | 🐛 5 | 🌐 Swift | 📅 2025-05-12 - macOS menubar icon for WireGuard/wg-quick.
  ![GitHub last commit](https://img.shields.io/github/last-commit/aequitas/macos-menubar-wireguard?style=flat-square\&color=informational) :black\_circle:

#### Dashboards

* [Wireguard Dashboard](https://github.com/donaldzou/wireguard-dashboard) ⭐ 3,696 | 🐛 97 | 🌐 Vue | 📅 2026-07-13 - A simple and easy to use WireGuard dashboard written in Python and Flask.
  ![GitHub last commit](https://img.shields.io/github/last-commit/donaldzou/wireguard-dashboard?style=flat-square\&color=informational) :green\_circle:

### Development

#### Development Environment

#### Testing

#### Boilerplate

### Homeserver

### Services based on WireGuard

#### Cloud Service

* [Warp](https://blog.cloudflare.com/1111-warp-better-vpn/) - A free WireGuard VPN from Cloudflare that's trying to fix mobile Internet performance and security.
* [wgcf](https://github.com/ViRb3/wgcf) ⭐ 8,610 | 🐛 25 | 🌐 Go | 📅 2026-07-30 - Cross-platform, unofficial CLI for Cloudflare Warp.
  ![GitHub last commit](https://img.shields.io/github/last-commit/ViRb3/wgcf?style=flat-square\&color=informational) :green\_circle:

#### VPN

* [Mullvad](https://github.com/mullvad/mullvadvpn-app) ⭐ 7,469 | 🐛 139 | 🌐 Rust | 📅 2026-08-16
  ![GitHub last commit](https://img.shields.io/github/last-commit/mullvad/mullvadvpn-app?style=flat-square\&color=informational) :green\_circle:
* [MozWire](https://github.com/NilsIrl/MozWire) ⭐ 634 | 🐛 14 | 🌐 Rust | 📅 2025-01-04 - An unofficial configuration manager giving Linux, macOS users (among others), access to Mozilla VPN.
  ![GitHub last commit](https://img.shields.io/github/last-commit/NilsIrl/MozWire?style=flat-square\&color=informational) :green\_circle:
* [LNVPN](https://github.com/LightRider5/lnvpn) ⭐ 76 | 🐛 12 | 🌐 JavaScript | 📅 2025-03-26 - A wireguard VPN provider with Ligthning only payments, pay as you use.
  ![GitHub last commit](https://img.shields.io/github/last-commit/LightRider5/lnvpn?style=flat-square\&color=informational) :red\_circle:

### Extensions / Plugins

* [wgsd](https://github.com/jwhited/wgsd) ⭐ 899 | 🐛 19 | 🌐 Go | 📅 2023-12-26 - A CoreDNS plugin that serves WireGuard peer information via DNS-SD (RFC6763) semantics. This enables use cases such as mesh networking, NAT-to-NAT connectivity, and dynamic discovery of WireGuard endpoint.
  ![GitHub last commit](https://img.shields.io/github/last-commit/jwhited/wgsd?style=flat-square\&color=informational) :yellow\_circle:

### Optimization

* [nr-wg-mtu-finder](https://github.com/nitred/nr-wg-mtu-finder) ⭐ 365 | 🐛 8 | 🌐 Python | 📅 2025-08-08 - A Python project to help you find the optimal MTU values for WG server and WG peer that maximizes the upload or download speeds between a peer and server.
  ![GitHub last commit](https://img.shields.io/github/last-commit/nitred/nr-wg-mtu-finder?style=flat-square\&color=informational) :yellow\_circle:

### Language Bindings

### Alternative Implementations

Beside Jason Donenfeld's implementation of the WireGuard protocol, written in C and Go, other implementations include:

* [boringtun](https://github.com/cloudflare/boringtun) ⭐ 7,169 | 🐛 107 | 🌐 Rust | 📅 2026-06-29 - Userspace WireGuard implementation in Rust by Cloudflare.
  ![GitHub last commit](https://img.shields.io/github/last-commit/cloudflare/boringtun?style=flat-square\&color=informational) :yellow\_circle:
* [ciniml/WireGuard-ESP32-Arduino](https://github.com/ciniml/WireGuard-ESP32-Arduino) ⭐ 959 | 🐛 33 | 🌐 C | 📅 2024-04-01 - WireGuard implementation for ESP32 Arduino in C.
  ![GitHub last commit](https://img.shields.io/github/last-commit/ciniml/WireGuard-ESP32-Arduino?style=flat-square\&color=informational) :red\_circle:
* [smartalock/wireguard-lwip](https://github.com/smartalock/wireguard-lwip) ⭐ 257 | 🐛 10 | 🌐 C | 📅 2026-08-14 - A C implementation of the WireGuard protocol intended to be used with the lwIP IP stack.
  ![GitHub last commit](https://img.shields.io/github/last-commit/smartalock/wireguard-lwip?style=flat-square\&color=informational) :yellow\_circle:
* [Matt Dunwoodie's implementation for OpenBSD, written in C](https://undeadly.org/cgi?action=article;sid=20200622052207).
* [Ryota Ozaki's wg(4) implementation, for NetBSD, is written in C](https://man.netbsd.org/wg.4).

## Useful Resources

### Blog Posts

* [WireGuard: great protocol, but skip the Mac app](https://rachelbythebay.com/w/2020/12/24/wg/)
* [WireGuard on Kubernetes with Adblocking](https://codingcoffee.dev/blog/wireguard_on_kubernetes_with_adblocking/)
* [SSH and User-mode IP WireGuard](https://fly.io/blog/ssh-and-user-mode-ip-wireguard/)
* [Setup and Adblocking VPN Using WireGuard and NextDNS](https://blog.paramdeo.com/2019/07/03/setup-an-adblocking-vpn-using-wireguard-and-nextdns.html)
* [WireGuard Endpoint Discovery and NAT Traversal using DNS-SD](https://www.jordanwhited.com/posts/wireguard-endpoint-discovery-nat-traversal/)
* [Taildrop was kind of easy, actually](https://tailscale.com/blog/2021-06-taildrop-was-easy/) - Taildrop was the main new feature launched in Tailscale v1.8.
* [Using Tailscale for Authentication of Internal Tools](https://blog.cloud66.com/using-tailscale-for-authentication-of-internal-tools)
* [IPv6 WireGuard Peering at Fly.io](https://fly.io/blog/ipv6-wireguard-peering/)
* [Our User-Mode WireGuard Year](https://fly.io/blog/our-user-mode-wireguard-year/)
* [Tunnel WireGuard via WebSockets](https://kirill888.github.io/notes/wireguard-via-websocket/) - Setting up WireGuard to work in restricted networks that block UDP traffic.
* [Tailscale's human-scale networks are still controlled by Google and Microsoft](https://iliana.fyi/blog/tailscale-auth-and-threat-modeling/)
* [How to access a peer's local network](https://iliasa.eu/wireguard-how-to-access-a-peers-local-network/) - A simple solution. There is no need of any configurations to set split-tunneling. The example shows how Peer B can route to Peer A through a WG server. Peer B can reach a specific network (subnet) behind Peer A.
* [Routing Specific Docker Containers Through WireGuard VPN with systemd-networkd](https://www.eisfunke.com/article/docker-wireguard-systemd.html) - A simple solution for routing specific docker containers through a WireGuard VPN using only two simple systemd-networkd files, no cumbersome `wg` or `ip` calls.
* [Decoding WireGuard with Wireshark](https://blog.salrashid.dev/articles/2022/wireguard_wireshark/) - A simple guide on how to inspect WireGuard packets in Wireshark.

### Articles

* [In-kernel WireGuard is on its way to FreeBSD and the pfSense router](https://arstechnica.com/gadgets/2021/03/in-kernel-wireguard-is-on-its-way-to-freebsd-and-the-pfsense-router/)
* [It's Looking Like Android Could Be Embracing WireGuard - "A Sane VPN"](https://www.phoronix.com/scan.php?page=news_item\&px=WireGuard-Android-GKI-Enabled)
* [Tailscale Raises $100 Million Series B to Fix the Internet with its Zero Trust VPN for Modern DevOps Teams](https://www.businesswire.com/news/home/20220504005325/en)
* [Identity management for WireGuard](https://lwn.net/SubscriberLink/910766/7678f8c4ede60928/)

### Demos and Examples

### Good Tips

* [WireGuard Gotchas with Multiple Tunnels](https://casavant.org/2020/10/10/wireguard-fwmark.html) - WG has a bit of a trap/gotcha when running multiple independent tunnels, one of which has a default route associated with it.

### Tutorials

* [Routing Docker Host And Container Traffic Through WireGuard](https://www.linuxserver.io/blog/routing-docker-host-and-container-traffic-through-wireguard) using [WireGuard Docker image by linuxserver.io](https://github.com/linuxserver/docker-wireguard) ⭐ 3,631 | 🐛 2 | 🌐 Dockerfile | 📅 2026-08-06
* [Fly-Tailscale-Exit](https://github.com/patte/fly-tailscale-exit) ⭐ 1,660 | 🐛 0 | 🌐 Shell | 📅 2026-08-09 - Run your own VPN with global exit nodes with Fly.io, Tailscale and Github.
* [How to easily configure WireGuard](https://www.stavros.io/posts/how-to-configure-wireguard/)
* [Getting Started with WireGuard](https://miguelmota.com/blog/getting-started-with-wireguard/)
* [What They Don’t Tell You About Setting Up A WireGuard VPN](https://dev.to/tangramvision/what-they-don-t-tell-you-about-setting-up-a-wireguard-vpn-1h2g)
* [Building a simple VPN with WireGuard with a Raspberry Pi as Server](https://snikt.net/blog/2020/01/29/building-a-simple-vpn-with-wireguard-with-a-raspberry-pi-as-server/)
* [Setting up a home VPN server with Wireguard (macOS)](https://mikkel.hoegh.org/2019/11/01/home-vpn-server-wireguard/)
* [Creating a VPN Gateway with a Unikernel running WireGuard](https://nanovms.com/dev/tutorials/running-nanos-wireguard-vpn-gateway)
* [Directions for setting up a WireGuard bounce server](https://gitlab.com/ncmncm/wireguard-bounce-server)
  > I find plenty of tutorials online for setting up the most basic Wireguard apparatus.
  > Like most peoples', my machines are stuck behind NATs. To connect between NATted hosts, you need control of a host that is not, to keep up on what external addresses the NATs are presenting.
  > The docs for WireGuard mention bounce servers, but say nothing about how to set one up.
* [WireGuard VPN Road Warrior Setup](https://emanuelduss.ch/2018/09/29/wireguard-vpn-road-warrior-setup/) - The important feature of this setup is, split tunnelling.
  > Either all traffic (default route) or only the traffic desired for the internal network can be routed through the VPN (split tunneling). This can be configured on the client.
* [WireGuard setup with Ansible](https://dev.to/tangramvision/exploring-ansible-via-setting-up-a-wireguard-vpn-3389) - A basic Ansible playbook for deploying a WireGuard server and (local) client.

### Videos

* [WireGuard: Next Generation Abuse-Resistant Kernel Network Tunnel](https://www.youtube.com/watch?v=eYztYCbV_8U)- A good talk from the WireGuard developer and security researcher, Jason Donenfeld explaining what WireGuard can do and how it works. The talk examine both the cryptography and kernel implementation particulars of WireGuard and explore an offensive attack perspective on network tunnels.
* [How To Build Your Own Wireguard VPN Server in The Cloud](https://www.youtube.com/watch?v=7yC-gJtl9mQ) - A good tutorial from Lawerence Systems regarding WireGuard.

### Books

### Podcasts and Interviews

### Presentations

* [Presentations by Jason A. Donenfeld](https://www.wireguard.com/presentations/) - A list of all Jason's presentations.

### Newsletters

## Uncategorized

* [WebVM: Linux Virtualization in WebAssembly with Full Networking via Tailscale](https://leaningtech.com/webvm-virtual-machine-with-networking-via-tailscale/) - Run WireGuard and Tailscale in the browser. wireguard-go code compiled to Wasm. WebVM is proprietary WebAssembly-powered x86 virtualization tech. I'm genuinely curious how it compares to v86/Fabrice Bellard's JSLinux (like WebVM but free and opened-source).

## Communities and Meetups

### English

* [/r/WireGuard](https://www.reddit.com/r/WireGuard/) - Official Reddit WireGuard.
* [#wireguard on Libera](https://web.libera.chat/#wireguard) - Official IRC on Libera Chat.

### Chinese

## Contribute

Contributions welcome! If you would like to contribute, please read the [contribution guidelines][contributing] first. It contains a lot of tips and guidelines to help keep things organized.

*Future: Implement GitHub Actions to monitor and verify all the links with a simple [Node.js script](./scripts/pull_request.js)*

## Copyright

"WireGuard" and the "WireGuard" logo are registered trademarks of Jason A. Donenfeld.

## License

<details>

<summary><b>Expand License</b></summary>

This repository contains a variety of content; some developed by Cedric Chee,
and some from third-parties. The third-party content is distributed under the
license provided by those parties.

*I am providing code and resources in this repository to you under an open
source license. Because this is my personal repository, the license you receive
to my code and resources is from me and not my employer.*

The content developed by Cedric Chee is distributed under the following license:

### Text

The text content is released under the CC-BY-NC-ND license.
Read more at [Creative Commons](https://creativecommons.org/licenses/by-nc-nd/3.0/us/legalcode).

### Code

The code in this repository is released under the [MIT license](LICENSE).

</details>

[editreadme]: https://github.com/cedrickchee/awesome-wireguard/edit/main/README.md

[contributing]: https://github.com/cedrickchee/awesome-wireguard/blob/main/.github/CONTRIBUTING.md

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-16._
