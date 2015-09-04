# aptget Role

Simple ansible role to manage `apt-get` updates and upgrades.

Role Variables
--------------

    aptget_update: True

Whether or not to keep the `apt` cache up to date.
    
    aptget_update_cache_valid_time: 3600

How old can the cache be and still be close enough to fresh.
    
    aptget_upgrade: False

Do a simple upgrade. Generally used by passing `-e aptget_upgrade=True` on
the `ansible-playbook` command line.
    
    aptget_distupgrade: False

Do a distro upgrade. Again, generally do this by passing `-e
aptget_distupgrade=True` on the `ansible-playbook` command line.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - slaarti.aptget

License
-------

Unlicense; see the LICENSE file.

Author Information
------------------

Chris Pinard <slaarti@gmail.com>
