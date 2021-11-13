![](/home/scale/github/NTUST-HIS-Lab.github.io/imgs/hislab-top.png)

![version](https://img.shields.io/static/v1?label=version&message=v0.1&color=<COLOR>)![Documentation](https://img.shields.io/badge/documentation-yes-brightgreen)![issues](https://img.shields.io/github/issues/NTUST-HIS-Lab/NTUST-HIS-Lab.github.io)![license](https://img.shields.io/github/license/NTUST-HIS-Lab/NTUST-HIS-Lab.github.io)

# Requirements

- Welcome! :smile:






# FAQs

## A. Usage 

* For using github repositories (`clone` / `pull` / `push`) , 
  you need setting up your `git config` and `ssh key`:

```bash
git config --global user.name "your_github_name"	# replace "" as yours
git config --global user.email "yours@gapps.ntust.edu.tw"	# replace "" as yours

ssh-keygen -t rsa -C "yours@gapps.ntust.edu.tw"	# replace "" as yours

# if you have some problems, you can try following commands to solve them.
# ssh -v git@github.com
# ssh-agent -s
# ssh-add ~/.ssh/id_rsa
# if an error occurs, use "ssh-agent -s" to continue "ssh-add ~/.ssh/id_rsa"
# ssh -T git@github.com
```

* Check your ssh key:

```bash
cd ~/.ssh
ls
# there will be three files there, "id_rsa"  "id_rsa.pub"  "known_hosts"
```

* Copy the content in `id_rsa.pub` and save it in your github: `Settings` - `SSH and GPG keys` - `SSH keys`. 
  You need to create a `New SSH key` to save it.

* Then enter the project folder you need to push, just use the command:

```bash
# git init
# git remote rm origin
# git branch -M main

git remote add origin git@github.com:NTUST-HIS-Lab/NTUST-HIS-Lab.github.io.git
git add .
git commit -m "describe"	# replace "" as you need
git push -u origin main
```

