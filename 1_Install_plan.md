## After Netinstall Installation
* First Steps:
  * From console:
    * From root install sudo
    ```bash
    $ apt install sudo
    ```
    * Add normal user to sudoers list
    ```bash
    $ nano /etc/sudoers
    # User privilege specification
    root    ALL=(ALL:ALL) ALL
    dev     ALL=(ALL:ALL) ALL
    ```    
    * Install network tools
    ```bash
    $ sudo apt install net-tools
    ```
    * Remove Libreoffice
    ```bash
    $ sudo apt-get remove --auto-remove libreoffice-gnome
    $ sudo apt-get purge libreoffice-gnome
    $ sudo apt-get purge --auto-remove libreoffice-gnome
    ```
    * Create alias for `ll` command
    ```bash
    $ nano .bashrc
    ## Add these lines at the end of file
    # Custom aliases
    alias l='ls -a'
    alias ll='ls -l'
    alias la='ls -la'
    ```
