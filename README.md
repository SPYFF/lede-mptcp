# LEDE MPTCP

[![Join the chat at https://gitter.im/SPYFF/lede-mptcp](https://badges.gitter.im/SPYFF/lede-mptcp.svg)](https://gitter.im/SPYFF/lede-mptcp?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

This is the stable branch. Supported MPTCP versions:

![kernel version](https://img.shields.io/badge/kernel%20version-4.4.93-brightgreen.svg)

## About
This is a fork of the [LEDE](https://github.com/lede-project/source) project aims to add proper [MPTCP](https://www.multipath-tcp.org/) support. In this version of LEDE the MPTCP kernel support is enabled by default, also with some other configuration tools to use your router as a transparent MPTCP proxy.

## Goals of this project
* None or minimal configuration to get multipath operation working.
* Keep the source close to the original LEDE project. Only the required kernel [patches](https://www.multipath-tcp.org/patches/) and minimal set of tools for configuration.
* In the near future MPTCP will upstream into the mainline kernel (and into the LEDE kernel as well), when this happens, this project wants to bring the proper tooling for the configuration.

## Building
Just follow the regular [LEDE building process](https://lede-project.org/docs/guide-developer/quickstart-build-images). But before the last `make` command, type `make kernel_menuconfig` and enable the MPTCP support described [here](https://multipath-tcp.org/pmwiki.php/Users/DoItYourself).

Successfully boot on Netgear R7000, Netgear R7800 routers and on a x86_64 VBox virtual machine.

## Example use-case
https://spyff.github.io/mptcp/2017/08/27/transparent-mptcp-proxy/
