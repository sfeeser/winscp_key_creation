# Creating a PPK key from an id_rsa key using windows subsystem for linux (WSL2)

1. Given a working key:

    `~/.ssh/id_rsa`
    
2. Given the public key installled on https://github.com/settings/keys

    `~/.ssh/id_rsa.pub` 

2. Install putty tools

    `sudo apt install putty-tools`
    
3. Create the ppk

    `puttygen id_rsa -o id_rsa.ppk`
    
4. Given a simlink

    `keys -> /mnt/c/Users/<USER>/<blah>/<blah>/`
    
5. Copy the ppk to the keys directory

    `cp ~/.ssh/id_rsa.ppk   ~/keys/id_rsa.ppk`  
    
6. Set winscp to use the new ppk key    
