# LEMP Vagrant Environment

Builds a LEMP environment for development

## Requirements

- Vagrant
- Vagrant Omnibus plugin
- Berkshelf

The Vagrant Berkshelf plugin isn't used at the moment due to build issues on windows.

# Usage

```bash
git clone git@github.com:DanielChalk/vagrant-lemp.git
cd vagrant-lemp
berks install --path=cookbooks
vagrant up --provision
```

## Usage with a frameworks

when using a framework use the ```node['lemp']['root']``` attribute to define your public dir.
The simplest method of doing this is by change the node.json file before you ```vagrant up```

# Author

Author:: Daniel Chalk (<daniel-chalk@hotmail.co.uk>)
