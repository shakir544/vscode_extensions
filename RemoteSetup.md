# Setup instructions to connect to remote machine from VSCode 

### Install VSCode (ofcourse :P)
### Install VSCode extensions (Python)
1. Python
2. Pyright 
3. Remote Development Extension 

### Generate SSH Keys (ssh-keygen)
    ssh-keygen -t rsa -b 4096 -c "user@servername.com" -f /home/user/.ssh/id_rsa_remote-ssh
    Generating public/private rsa key pair.
    Enter passphrase (empty for no passphrase):
    Enter same passphrase again:
    Your identification has been saved in /home/user/.ssh/id_rsaremote-ssh.
    Your public key has been saved in /home/user/.ssh/id_rsaremote-ssh.pub.
    The key fingerprint is:
    SHA256:ISPyzUc8F+A5CbMgSpBcHlYTi5ML9KtAiU5v/7TI87s me@example.com
    The key's randomart image is:
    +---[RSA 4096]----+
    |++o+o++ ... |
    |=o=.+.o* o . |
    |o=.*..+ X . |
    |+ oo++ + = |
    |.. =. o S |
    |. o . . |
    | . . . |
    | ..+ . |
    | ooEo |
    +----[SHA256]-----+

### Copy SSH Key (ssh-copy-id)
    ssh-copy-id -i ~/.ssh/id_rsa-remote-ssh.pub user@SERVER_ID.mylabserver.com
