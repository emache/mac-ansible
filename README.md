Configuring Mac OS X with Ansible
=================================

I have two Macs and like to have (at least some of) the same apps on each.
Since Ansible 1.6, the `homebrew` and `homebrew_cask` modules have been added,
which has let me keep them in sync.

Clone into Documents, install git, brew, and ansible and run:

    ansible-playbook playbook.yml

Optionally add `--skip-tags brew` to skip the slow brew stuff.


Getting Started
---------------

1. Install [homebrew](http://brew.sh/) with the command from the site
2. `brew install python` (It's better than system python, see
   [guide](https://github.com/Homebrew/homebrew/blob/master/share/doc/homebrew/Homebrew-and-Python.md))
3. `pip install ansible` (better than homebrew package as it's always latest)
4. Then `ansible-playbook playbook.yml`


Todo
----

* My terminal theme uses Ubuntu Mono; install ubuntu fonts from
  [homebrew-fonts](https://github.com/caskroom/homebrew-fonts) when it is
  stable
