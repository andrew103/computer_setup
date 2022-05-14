Install git and confirm
```
sudo apt install git
git --version
```

Setup author identity
```
git config --global user.email "andrew_103@rocketmail.com"
git config --global user.name "Andrew Euredjian"
```

Generate GitHub SSH Key for remote repo operations (`id_ed####` could be different than shown)
```
ssh-keygen -t ed25519 -C "andrew_103@rocketmail.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
```

Add key to GitHub (filename could be different)
```
cat ~/.ssh/id_ed25519.pub
```


1) Go to https://github.com/settings/keys
2)