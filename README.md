# LEDE MPTCP

## About
This is a fork of the [LEDE](https://github.com/lede-project/source) project aims to add proper [MPTCP](https://www.multipath-tcp.org/) support. In this version of LEDE the MPTCP kernel support is enabled by default, also with some other configuration tools to use your router as a transparent MPTCP proxy.

## Goals of this project
* None or minimal configuration to get multipath operation working.
* Keep the source close to the original LEDE project. Only the required kernel [patches](https://www.multipath-tcp.org/patches/) and minimal set of tools for configuration.
* In the near future MPTCP will upstream into the mainline kernel (and into the LEDE kernel as well), when this happens, this project wants to bring the proper tooling for the configuration.

## Building
*TBD*
