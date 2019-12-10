Ansible role that generates DH parameters
=================

A very simple role for generating a DH parameter file on your hosts using [Ansible](http://www.ansibleworks.com/).

Usage
-----

Clone this repo into your roles directory:

    $ git clone https://github.com/emielmolenaar/ansible-role-generate-dhparam.git roles/generate-dhparam

And add it to your play's roles:

    - hosts: ...
      roles:
        - generate-dhparam
        - ...

I recommend using a `requirements.yml` in your roles directory though:

    - src: https://github.com/emielmolenaar/ansible-role-generate-dhparam.git
      name: generate-dhparam

Installing the role will require a `ansible-galaxy install -r ./roles/requirements.yml -p ./roles` from the root directory of your playbook.
