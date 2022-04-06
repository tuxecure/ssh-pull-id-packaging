# ssh-pull-id-packaging
Packaging for [ssh-pull-id](https://sourceforge.net/projects/ssh-pull-id/) by [krisjacewicz](https://sourceforge.net/u/krisjacewicz/)
ssh-pull-id is a command line tool that does what ssh-copy-id does but in the opposite direction: instead of pushing your ssh-id to another machine, it pulls another machine's ssh-id into your host.

the tool was made with Ubuntu Touch in mind, because its default ssh config is such, that ssh-copy-id won't work. this is because Ubuntu Touch device does not accept ssh client with password authentication, but only with public key based authentication. and copy-ssh-id itself uses password authentication to connect first, then push public key to the remote host, so that later key based authentication can be used instead.

ssh-pull-id will reverse the direction, now you use the tool to pull another host's public key. the typical scenario it was created for, is when you use it on Ubuntu Touch device, and pull is made from another host which allows password based authentication.

## Before
![image](https://user-images.githubusercontent.com/10421851/162029364-aa55f3b3-f944-4b70-bbbb-edb23bac2037.png)


## running ssh-pull-id
![image](https://user-images.githubusercontent.com/10421851/162029403-6deccb36-4630-4b72-9d4d-edbdfdf38449.png)

## After
![image](https://user-images.githubusercontent.com/10421851/162029469-87b34e78-9f39-43fb-858a-d19c78182416.png)
