# aggioggia
Updater script for apt and apt-get. <br />
Because I'm too lazy to simply apt update+upgrade.

## Usage
```
$ aggioggia
[sudo] password for dpdani:
 ⇒  Pre-update cleaning...
 ⇒  Fetching updates...
 ⇒  Available updates:
Listing... Done
linux-generic/xenial-proposed 4.4.0.70.76 amd64 [upgradable from: 4.4.0.67.72]
linux-headers-generic/xenial-proposed 4.4.0.70.76 amd64 [upgradable from: 4.4.0.67.72]
linux-image-generic/xenial-proposed 4.4.0.70.76 amd64 [upgradable from: 4.4.0.67.72]
 ⇒  Running upgrade...
 ⇒  Cleaning up...
 ⇒  System updated
$ _
```
## What does this do for me?
Basically aggioggia is running the following apt commands:
1. `apt autoremove`
2. `apt update`
3. `apt list`
4. `apt upgrade`
5. `apt autoremove`

## Installation
Copy the file `aggioggia` to `/usr/bin/`. You'll be able to use aggioggia from the command line.

## Dependencies
- `apt-get`
- `apt`
- `sudo` <br />
Basically, a Debian system with sudo installed (Ubuntu).
