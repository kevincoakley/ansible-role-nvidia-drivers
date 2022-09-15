ansible-role-nvidia-drivers
=========

![](https://github.com/kevincoakley/ansible-role-nvidia-drivers/workflows/Molecule%20Test/badge.svg)

Installs the NVIDIA drivers and libnvidia-container-tools on a Linux system.

Requirements
------------

User must provide a URL to download the NVIDIA driver from. 

Role Variables
--------------

nvidia_driver_download_url
nvidia_license_server_address (optional) 


Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    ---
    - name: Converge
      hosts: all
      become: true

      vars:
        nvidia_driver_download_url: http://us.download.nvidia.com/XFree86/Linux-x86_64/390.25/NVIDIA-Linux-x86_64-390.25.run
        nvidia_license_server_address: mylicense.server.com

      roles:
        - role: ansible-role-nvidia-drivers

License
-------

BSD

Author Information
------------------

Kevin Coakley (https://github.com/kevincoakley)
