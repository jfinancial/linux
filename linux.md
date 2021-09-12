# OSX Linux

#### Networking
- `ipconfig getifaddr en0` => Gets current IP
- `scutil --dns | grep 'nameserver\[[0-9]*\]' ` => Finds name servers being used

#### Top
- Shift + P = sort processed by CPU Utilisation
- Shift + M = Sort processed by Memory Usage
- Shift + E = Change unit of memory

#### Sudo 
The `/etc/sudoers` file controls who can run what commands as what users on what machines and can also control special things such as whether you need a password for particular commands. The file is composed of aliases (basically variables) and user specifications (which control who can run what).
- `sudo su -` -> Sudo to root 

#### How many cores
it
- `nproc` => prints the number of processing units available in a Linux system. It is part of GNU Core utils.
