Ansible role: google_chrome
=========

Ansible role to install Google Chrome on Linux.

Requirements
------------

gpg

Role Variables
--------------

    google_chrome_gpg_key: https://dl.google.com/linux/linux_signing_key.pub
    google_chrome_gpg_key_fingerpint: 4CCA1EAF950CEE4AB83976DCA040830F7FAC5991

The Google Chrome gpg key URL and fingerprint.

    google_chrome_rpm_repository_url: https://dl.google.com/linux/chrome/rpm/stable/x86_64
    google_chrome_apt_repository_url: deb [arch=amd64] https://dl.google.com/linux/chrome/deb/ stable main

The Google Chrome apt and rpm repositories URL.


Dependencies
------------

None

Example Playbook
----------------

    - hosts: all
      roles:
         - role: egdoc.google_chrome

License
-------

GPL-2.0

Author Information
------------------

Role created by Egidio Docile