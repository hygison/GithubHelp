
From: https://stackoverflow.com/questions/61067967/git-gpg-failed-to-sign-the-data-in-visual-studio-code

To sign the commit in using gpg
```
export GPG_TTY=$(tty)
```

```
echo "test" | gpg --clearsign
```

Cache the password for a longer time (157680000 = 5 years)
```
mkdir -p ~/.gnupg
echo "default-cache-ttl 157680000" >> ~/.gnupg/gpg-agent.conf
```

To open the config file
```
nano ~/.gnupg/gpg-agent.conf
```
