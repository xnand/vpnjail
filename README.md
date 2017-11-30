# vpnjail

Bash script to be called from openvpn, to isolate shell or programs from the non-vpn network. Tested on Arch Linux only. Up and down scripts working, with --up-restart sometimes goes crazy, so restarting openvpn is required in this case (or making a pull request to fix this script?).

    git clone https://github.com/xnand/vpnjail.git && cd vpnjail && chmod 755 vpnjail && vpnjail setup
    
to download it and create the two symlinks that need to be called by openvpn (see content of the script).

Do what you want with it I don't care what kind of drugs you're buying from tor networks :)
