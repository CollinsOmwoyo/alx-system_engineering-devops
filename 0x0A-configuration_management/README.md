# Puppet: Quick Start

## Install Puppet
### Linux (Ubuntu/Debian)
```sh
wget https://apt.puppet.com/puppet7-release-focal.deb
sudo dpkg -i puppet7-release-focal.deb
sudo apt update && sudo apt install -y puppet-agent
```
### Windows

### Verify
```sh
puppet --version
```

## Basic Usage
### Simple Manifest
Create `example.pp`:
```puppet
file { '/tmp/hello.txt': ensure => present, content => 'Hello, Puppet!'}
```
Run:
```sh
puppet apply example.pp
```

## Next Steps
- Learn Puppet DSL
- Explore Modules
- Use Master-Agent setup