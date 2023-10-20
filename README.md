# USF GlobalProtect VPN
## Installation
Clone this repo and navigate to the local folder:
```
~$ git clone https://github.com/akarez/USF-GlobalProtect.git && cd USF-GlobalProtect/packages/
```
### Ubuntu
For Debian based distributions including Ubuntu, Mint, Kali, Pop!OS etc:

```
~$ sudo dpkg -i GlobalProtect_deb-5.1.1.0-17.deb && sudo apt install -f -y
```
### Fedora
For RHEL based distributions including Fedora, CentOS etc:

```
~$ sudo rpm -i GlobalProtect_rpm-5.1.1.0-17.rpm
```
### Generic
For the rest of distributions such as Arch, Manjaro, Void etc. use the generic installer script:

```
~$ tar xvf GlobalProtect_tar-5.1.1.0-17.tgz && sudo ./install
```
## Setup
Create a new connection and enter your NetID credentials when prompted. You will only run this when setting up the connection to a new portal. After this your credentials and the portal address will be saved for future access:
```
~$ globalprotect connect --portal vpn.usf.edu
```
## Usage
Connecting to the portal:
```
~$ globalprotect connect
```

Show connection status:
```
~$ globalprotect show --status
```

Show connection details:
```
~$ globalprotect show --details
```

Restart connection:
```
~$ globalprotect rediscover-network
```

Disconnecting from the portal:

```
~$ globalprotect disconnect
```
