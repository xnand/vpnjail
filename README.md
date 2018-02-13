# vpnjail

Bash script to be called from openvpn, to isolate shell or programs from the non-vpn network. Tested on Arch Linux only. Up and down scripts working, with --up-restart sometimes goes crazy, so restarting openvpn is required in this case (or making a pull request to fix this script?).

    git clone https://github.com/xnand/vpnjail.git
    cd vpnjail
    chmod 755 vpnjail
    sudo ./vpnjail setup
    
    
or as a one-liner

    wget https://raw.githubusercontent.com/xnand/vpnjail/master/vpnjail && chmod 755 vpnjail && ./vpnjail setup
    
    
to download it and create the two symlinks that need to be called by openvpn (see content of the script), then directly call the script from command line to get a shell inside the newly created namespace.

PS: needs root priviledges. If you want to execute stuff as non-root, type "sudo -u *youruser* bash" or whatever shell you use, inside the namespace.
