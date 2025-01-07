When using multiple accounts and you want to download or upload code with ssh, this can help you reduce your time by reading this instead of asking AI again :D

Steps:
1. Create a ssh key
```
ssh-keygen -t ed25519 -C "email@example.com"
# save it as "NAME" you want
```

2. Create config file at ~/.ssh/config

```
Host <AAA>
  Hostname github.com
  AddKeysToAgent yes
  IdentityFile ~/.ssh/<NAME>
```

3. When clone the code, the command looks like this:

```
# git clone git@github.com:<username>/<repoName>.git change to code beblow
git clone git@<AAA>:<username>/<repoName>.git
```

Got it?

Happy clone code :))
