Setting up openstack. When connecting to active instance problems with SSH key not being accepted and the instance denying access

_________________________________________
host@host ~$ ssh debian@198.299.299.299
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
@    WARNING: REMOTE HOST IDENTIFICATION HAS CHANGED!     @
@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@@
IT IS POSSIBLE THAT SOMEONE IS DOING SOMETHING NASTY!
Someone could be eavesdropping on you right now (man-in-the-middle attack)!
It is also possible that a host key has just been changed.
The fingerprint for the ED25519 key sent by the remote host is
SHA256: [ ------------------- ]
Please contact your system administrator.
Add correct host key in /home/nameMcName/.ssh/known_hosts to get rid of this message.
Offending ED25519 key in /home/nameMcName/.ssh/known_hosts:1
  remove with:
  ssh-keygen -f '/home/nameMcName/.ssh/known_hosts' -R '198.299.299.299'
Host key for 198.299.299.299 has changed and you have requested strict checking.
Host key verification failed.

________________________________________

runnnig the "ssh-keygen" command
it spits info at you
try connect again, it gets confused and start asking if sure
input the **KEY FINGERPRINT**

SSH- into it agian and should work
