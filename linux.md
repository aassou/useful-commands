# Ubuntu – How to add an executable to the search path
mkdir ~/bin

nano ~/.bashrc

* Add the following to the end of your .bashrc file while using nano or your text editor of choice:

export PATH="/home/$USER/bin:$PATH"

ln path/to/your/exec name_of_your_sym_link

# Ubuntu – How to add a symlink

ln path/to/your/exec name_of_your_sym_link

# Ubuntu – How to add an alias
alias symfony-server='php -S 127.0.0.1:8000 -t public/'

# Ubuntu – Check port usage
netstat -tulpn | grep :port