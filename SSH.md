Create and save SSH key on Macbook using VS Code in order to connect with Github

1) Set Name (Any Name, it will be used in the commits made from such computer):
  `git config --global user.name "Hygison Brandao"`
2) Set Email (Github email):
  `git config --global user.email "hygisonbrandao@gmail.com"`
3) Check for Existent SSH Keys, if there are keys, it will show up, and you can skip to Step-5:
  `ls -al ~/.ssh`
4) Create New Key (Use Github Email), after creation, keep pressing enter until it is over, no need to set anything:
  `ssh-keygen -t rsa -b 4096 -C "hygisonbrandao@gmail.com"`
5) Copy the SSH Key to the clip:
  `pbcopy < ~/.ssh/id_rsa.pub`
6) Go to Github and add new SSH Key (The key name is just something to remember where the key is being used):
  `https://github.com/settings/keys`
  
7) Check the key:
  `ssh -T git@github.com`
  > If there are no problems then It should be working when doing the commits

