# Create SSH key pair (based on gitlab steps)
 - https://git.dev.zgrp.net/help/user/ssh.md#generate-an-ssh-key-pair

## For example, if three accounts were added, should look like this:

```sh
# GitLab.com
# github account
Host github.com
HostName github.com
PreferredAuthentications publickey
IdentityFile ~/.ssh/id_rsa_myaccount_github

# gitlab account
Host gitlab.com
HostName gitlab.com
PreferredAuthentications publickey
IdentityFile ~/.ssh/id_rsa_myaccount_gitlab

# gitlab company account
Host gitlab.my_company.com
HostName gitlab.my_company.com
PreferredAuthentications publickey
IdentityFile ~/.ssh/id_rsa_mycompanyaccount_gitlab
```