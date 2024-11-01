# Hammer Tool

## Overview

Hammer is a powerful tool designed for testing server robustness through stress testing. Use it responsibly and ensure you have permission before testing any server.

## Table of Contents

- [Installation](#installation)
- [Prerequisites](#prerequisites)
- [Obtaining the Name Server](#obtaining-the-name-server)
- [Usage](#usage)
- [Example Commands](#example-commands)
- [Notes](#notes)
- [License](#license)

## Installation

To install Hammer, follow these steps:

1. Open your terminal.
2. Update your package list and install the necessary software.

## Prerequisites

Ensure your system is up-to-date and has the required packages installed:

```bash
$ sudo apt update
$ sudo apt upgrade
$ sudo apt install python3
$ sudo apt install git
$ sudo apt install dnsutils
```

## Obtaining the Name Server

To perform an operation with Hammer, you’ll need the Name Server of the target website. Use the following command to retrieve this information:

```bash
$ nslookup example.com
```
Make sure to note the IP address returned for the website.

## Usage

Navigate to the Hammer directory and execute the script with the appropriate parameters. Here’s how to do it:

Change to the Hammer directory:

```bash

$ cd Hammer
```
Run the Hammer script using the following syntax:

```bash

$ python3 hammer.py -s [SERVER_IP_ADDRESS] -t [THREAD_COUNT]
```
## Example Commands

For a specific IP address with 135 threads:

```bash

$ python3 hammer.py -s 123.45.67.89 -t 135
```

For a local server on port 8000 with 500 threads:

```bash

$ python3 hammer.py -s 127.0.0.1 -p 8000 -t 500
```
For a specific IP address with a custom port and 5000 threads:

```bash

$ python3 hammer.py -s 216.24.57.4 -p 80 -t 5000
```
## Notes

Replace [IP_ADDRESS] and [THREAD_COUNT] with your target's IP address and the desired number of threads.
Ensure you have permission to test any server you target to avoid legal issues.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
