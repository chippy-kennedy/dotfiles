##Some Useful Ubuntu Configurations

###Change Local Host name - so APIs (like facebook) can read local.host as a domain for a development server
sudo vim /etc/hosts; localhost => local.host; :wq!
######**May cause issues with resolv lib, revert to fix

###Find a string in a directory
grep -rnw '/path/to/somewhere/' -e "pattern"

###Supplement a Fresh Vim Install - allow for copy/paste to clipboard
sudo apt-get install vim-gtk

###User Puttygen to Convert Keys
####ppk --> rsa
```
puttygen id_dsa.ppk -O private-openssh -o id_dsa
puttygen id_dsa.ppk -O public-openssh -o id_dsa.pub
```

###Random Unix Stuff
env vars stored in `~/.bash_profile`
