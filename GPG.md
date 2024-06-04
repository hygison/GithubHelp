
From: https://stackoverflow.com/questions/61067967/git-gpg-failed-to-sign-the-data-in-visual-studio-code

To sign the commit in using gpg
```
export GPG_TTY=$(tty)
```

```
echo "test" | gpg --clearsign
```
