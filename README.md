# Binwalk

![Build Status](https://github.com/OSPG/binwalk/actions/workflows/test.yml/badge.svg)
[![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://GitHub.com/ReFirmLabs/binwalk/graphs/commit-activity)
[![GitHub license](https://img.shields.io/github/license/ReFirmLabs/binwalk.svg)](https://github.com/ReFirmLabs/binwalk/blob/master/LICENSE)
[![GitHub stars](https://img.shields.io/github/stars/badges/shields.svg?style=social&label=Stars)](https://github.com/ReFirmLabs/binwalk/stargazers)

Binwalk is a fast, easy to use tool for analyzing, reverse engineering, and extracting firmware images.


### *** Extraction Security Notice ***

Prior to Binwalk v2.3.3, extracted archives could create symlinks which point anywhere on the file system, potentially resulting in a directory traversal attack if subsequent extraction utilties blindly follow these symlinks. More generically, Binwalk makes use of many third-party extraction utilties which may have unpatched security issues; Binwalk v2.3.3 and later allows external extraction tools to be run as an unprivileged user using the `run-as` command line option (this requires Binwalk itself to be run with root privileges). Additionally, Binwalk v2.3.3 and later will refuse to perform extraction as root unless `--run-as=root` is specified.

### Installation and Usage

* [Installation](./INSTALL.md)
* [API](./API.md)
* [Supported Platforms](https://github.com/ReFirmLabs/binwalk/wiki/Supported-Platforms)
* [Getting Started](https://github.com/ReFirmLabs/binwalk/wiki/Quick-Start-Guide)
* [Binwalk Command Line Usage](https://github.com/ReFirmLabs/binwalk/wiki/Usage)
* [Binwalk IDA Plugin Usage](https://github.com/ReFirmLabs/binwalk/wiki/Creating-Custom-Plugins)

More information on [Wiki](https://github.com/ReFirmLabs/binwalk/wiki)

# Binwalk Professional Edition

After years of developing and supporting binwalk as an open source project we have finally sold out to the man and released a cloud-based firmware extraction engine called *Binwalk Enterprise*. After all someone needs to pay devttys0 so he can buy more milling equipment and feed his children (in that order). Please consider subscribing and reap the benefits of getting actual customer support for all your firmware extraction and analysis needs. Please visit https://www.refirmlabs.com/binwalk-enterprise/ for more information. 
