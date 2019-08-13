# IPMI Exporter

[![GoDoc](https://godoc.org/github.com/lovoo/ipmi_exporter?status.svg)](https://godoc.org/github.com/lovoo/ipmi_exporter) [![Build Status](https://travis-ci.org/lovoo/ipmi_exporter.svg?branch=master)](https://travis-ci.org/lovoo/ipmi_exporter)

IPMI Exporter for prometheus.io, written in Go.

**THIS IS A FORK** of the original repository, which is available [here](https://github.com/lovoo/ipmi_exporter).

This repo has:
* merged two additional pull requests;
* a fix for the [issue 31](https://github.com/lovoo/ipmi_exporter/issues/31).

## Requirements

* ipmitool

## Docker Usage

    docker run --device=/dev/ipmi0 -d --name ipmi_exporter -p 9289:9289 lovoo/ipmi_exporter:latest

## Building

    make build

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -am 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request

## Package repositories

Debian repo quick install:

    curl -s https://packagecloud.io/install/repositories/LovooOS/prometheus-exporters/script.deb.sh | sudo bash

You can find package repositories for other systems and how to add it to the system on [packagecloud.io/LovooOS/](https://packagecloud.io/LovooOS/prometheus-exporters/install)

Special thanks to [packagecloud.io](https://packagecloud.io/) for hosting our packages.
