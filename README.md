# Superlumic

Superlumic is a light utility wrapper around Ansible to ease the automated install of OSX 10.10 and higher. It uses several roles distilled over years of use in the Chef based predecessor, Kitchenplan.

This, however, is a fork of superlumic which uses the convenience of superlumic to bootstrap the machine with ansible but uses mac-dev-playbook for the actual installation.  This fork loses some of the ability of superlumic to set different usernames, but that funcationality might get added back in soon.

## Configuration

This used to use superlumic's [superlumic-config](https://github.com/superlumic/superlumic-config) repo.  Instead, this version of superlumic actually uses geerlinguy's mac-dev-playbook for the actual config.  My fork of mac-dev-playbook merely includes my config.yml and a little fix for pip: [my mac-dev-playbook fork](https://github.com/stackedsax/mac-dev-playbook).

## Running Superlumic

```
curl -s https://raw.githubusercontent.com/stackedsax/superlumic/master/superlumic | bash -s https://github.com/stackedsax/mac-dev-playbook
```

Or if you have an aversion to piping scripts over the internet into bash, download the [Superlumic script](https://raw.githubusercontent.com/stackedsax/superlumic/master/superlumic) and run it.

## Out of the box result?

You should get a one-liner that installs all of my [mac-dev-playbook config](https://github.com/stackedsax/mac-dev-playbook/blob/master/config.yml) via mac-dev-playbook.