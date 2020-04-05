# addMultipleAccounts
Create multiple Linux user accounts with a password and the change password on first login option in place to force the user to change their password.
Options for account creation will be set as follows:
GROUP=100                Set group ID to 100 (users)
HOME=/home               Set base home directory to /home
INACTIVE=-1              Password expiration is disabled (-1)
EXPIRE=                  Don’t set date to disable user account
SHELL=/bin/sh            Set the default shell to /bin/bash
SKEL=/etc/skel           Copy config files from /etc/skel to $HOME
CREATE_MAIL_SPOOL=no     Create a mail spool directory

After creation of the accounts the chage command will be run using option -d 0 to force the change of password at first login.
