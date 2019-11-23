
~/home/workspace/hy000jin/brewfile master*
❯ cd /Users/.ssh
cd: no such file or directory: /Users/.ssh

~/home/workspace/hy000jin/brewfile master*
❯ ls
Brewfile           README.md          id_rsa_hyooo
Brewfile.lock.json id_rsa_ctilab      id_rsa_hyooo.pub
LICENSE            id_rsa_ctilab.pub  initial

~/home/workspace/hy000jin/brewfile master*
❯ cd /Users

/Users
❯ ls
Shared    hyojinkim

/Users
❯ cd hyojinkim/.ssh

~/.ssh
❯ ls
config       ctilab.pub   hy000jin.pub k1my0.pub
ctilab       hy000jin     k1my0        known_hosts

~/.ssh
❯ ssh -add -l
ssh: illegal option -- d
usage: ssh [-46AaCfGgKkMNnqsTtVvXxYy] [-B bind_interface]
           [-b bind_address] [-c cipher_spec] [-D [bind_address:]port]
           [-E log_file] [-e escape_char] [-F configfile] [-I pkcs11]
           [-i identity_file] [-J [user@]host[:port]] [-L address]
           [-l login_name] [-m mac_spec] [-O ctl_cmd] [-o option] [-p port]
           [-Q query_option] [-R address] [-S ctl_path] [-W host:port]
           [-w local_tun[:remote_tun]] destination [command]

~/.ssh
❯ ssh-add -l
4096 SHA256:/Vg4FjfQIf1oAdDKAMZLTwgKRH+haI+ecSEVc5apyXI hyooj10@gmail.com (RSA)
2048 SHA256:Ic+aYTC9ZtWbeSxxyW+SMVz2wf+FldlUcnweT4YqlpA hyooj10@gmail.com (RSA)
2048 SHA256:nZFaMV2CkqggNGUYHqXAkSh6FNpZi/rkOWbbH6Hhqjk cti.hyooo@gmail.com (RSA)
2048 SHA256:eyvo7FIKdmWpQwWHsPjq/UsZhiRpXVmvDcb/FVwRXco hyooojin@ctilab.co.kr (RSA)

~/.ssh
❯ ssh-add -D
All identities removed.

~/.ssh
❯ ls
config       ctilab.pub   hy000jin.pub k1my0.pub
ctilab       hy000jin     k1my0        known_hosts

~/.ssh
❯ ssh-add -l
The agent has no identities.

~/.ssh
❯ ls
config       ctilab.pub   hy000jin.pub k1my0.pub
ctilab       hy000jin     k1my0        known_hosts

~/.ssh
❯ ssh-add -l
The agent has no identities.

~/.ssh
❯ eval 'ssh-agent -s'
SSH_AUTH_SOCK=/var/folders/xt/gwb2bn6s429gx3wslz5sf2vw0000gn/T//ssh-xInlSQRgGSZo/agent.8527; export SSH_AUTH_SOCK;
SSH_AGENT_PID=8528; export SSH_AGENT_PID;
echo Agent pid 8528;

~/.ssh
❯ rm -rf *.pub

~/.ssh
❯ rm -rf hy000jin

~/.ssh
❯ rm -rf ctilab

~/.ssh
❯ rm -rf k1my0

~/.ssh
❯ ls
config      known_hosts

~/.ssh
❯ vi known_hosts

~/.ssh 12s
❯ ssh-keygen -t rsa -C "hyooj10@gmail.com" -f "id_rsa_k1my0"
Generating public/private rsa key pair.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in id_rsa_k1my0.
Your public key has been saved in id_rsa_k1my0.pub.
The key fingerprint is:
SHA256:Hd6ivKCORAACRBUZADzh1jq/bl7/MW2yueQI158YwdQ hyooj10@gmail.com
The key's randomart image is:
+---[RSA 2048]----+
|@=+++            |
|+o..      .      |
|.o..     ..E     |
|...     oo o     |
| o.     So+ .    |
| .o    ...o.     |
|  .. o..oB o     |
| . oo.+.+.@ .    |
|  ==o  ooB.o     |
+----[SHA256]-----+

~/.ssh 7s
❯ ssh-keygen -t rsa -C "cti.hyooo@gmail.com" -f "id_rsa_hy000jin"
Generating public/private rsa key pair.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in id_rsa_hy000jin.
Your public key has been saved in id_rsa_hy000jin.pub.
The key fingerprint is:
SHA256:rVYFISkOSWajK9ic8wAkMwJOJBT5BucvSlGPqr0RdKY cti.hyooo@gmail.com
The key's randomart image is:
+---[RSA 2048]----+
|@*o.=.  ..o.     |
|B= *o.. .. .     |
|..O =o .    .    |
|.* @ ..  . .     |
|o E .   S o      |
| + * .   o       |
|o.o o   o        |
|....   .         |
|  ..             |
+----[SHA256]-----+

~/.ssh
❯ ssh-keygen -t rsa -C "hyooojin@ctilab.co.kr" -f "id_rsa_ctilab"
Generating public/private rsa key pair.
Enter passphrase (empty for no passphrase):
Enter same passphrase again:
Your identification has been saved in id_rsa_ctilab.
Your public key has been saved in id_rsa_ctilab.pub.
The key fingerprint is:
SHA256:LTiv2ON+fjKnIEMgxzUPWP7X5/OpXsLT8MNIKB2vNwk hyooojin@ctilab.co.kr
The key's randomart image is:
+---[RSA 2048]----+
|   o=            |
| ..o +           |
|. + . .   .      |
| o . . . + +     |
|    . + S E =    |
|   .   + o B B   |
|    o . . . @ *  |
|     =.o+ o. B o |
|    .o=+o* .o.o  |
+----[SHA256]-----+

~/.ssh
❯ eval 'ssh-agent -s'
SSH_AUTH_SOCK=/var/folders/xt/gwb2bn6s429gx3wslz5sf2vw0000gn/T//ssh-zbXpYMD6OY9u/agent.8922; export SSH_AUTH_SOCK;
SSH_AGENT_PID=8923; export SSH_AGENT_PID;
echo Agent pid 8923;

~/.ssh
❯ ssh-add ~/.ssh/id_rsa_hy000jin
Enter passphrase for /Users/hyojinkim/.ssh/id_rsa_hy000jin:
Identity added: /Users/hyojinkim/.ssh/id_rsa_hy000jin (cti.hyooo@gmail.com)

~/.ssh
❯ ssh-add ~/.ssh/id_rsa_ctilab
Enter passphrase for /Users/hyojinkim/.ssh/id_rsa_ctilab:
Identity added: /Users/hyojinkim/.ssh/id_rsa_ctilab (hyooojin@ctilab.co.kr)

~/.ssh
❯ ssh-add ~/.ssh/id_rsa_k1my0
Enter passphrase for /Users/hyojinkim/.ssh/id_rsa_k1my0:
Identity added: /Users/hyojinkim/.ssh/id_rsa_k1my0 (hyooj10@gmail.com)

~/.ssh
❯ cat id_rsa_k1my0.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQDm1IhBURYKSfY9pD+W2ac5Os2n7YHB0xsYLDfZzZOLxAYZ1O+QjEezgnOzesUtQ4bvq8uT+mDZVNDSn0w1bbgIbtIoqg7MNH8GAAb2DA1+hK7lzQlsVtHeMDKjPrsfQIzfCzi0HsR/a0VclCFqgAA/msl+9TmciVWvWwd9OUVSirp+bq5WNEzgFf4wS47LH4k/+4dDH9AzZ9X/5XL5gd0wPg4F2TOUoH49QyWUC2CTZDGoEMVi9aadBoFprmFqdQtyQyh0eD9tn9S5yrPaNCtc1xX9E1kslKOScFEjD3xaDDChPIQappHKLILn3k2FXNG1Cj4xNaVm49/VsUVK1vJx hyooj10@gmail.com

~/.ssh
❯ cat id_rsa_hy000jin.pub
ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQCbDdwq/PUPYhOqVwUJ+CBictD0Pd15X8QsPQhwVrbTcITYWQupMMmTb5efDslyTCQeMgzcdxxfvKoicInHJky4+g2Ic0MdvcZBOdEnmL8qOObgZNqsE6KMVAbX/vVfXSURGi5Mshx9AG+Ut6999yrw3NBX2Rn5loyDuoZfgS3yYEbAk+T8CvWbbeeIdBD1tD8kZ13sZemBQKbMNZOU7kUI/0crcNO0EEAPf144k1pM+6iB8emWuoLGxJLmAwiBQoetnhZ38ExjC1iGd9nhHNYTFKYEtYT3HWA1r048I8B75FloiT2cKADIeJZe1eCD2AN+RcaF0qv31wwRawiIJeet cti.hyooo@gmail.com

~/.ssh
❯ cd /Users/hyojinkim/home/workspace/hy000jin

~/home/workspace/hy000jin
❯ ls
List                          TIL
Project                       Temp
Referrer                      brewfile
Snazzy.itermcolors            무제 폴더
Study                         손기정.docx

~/home/workspace/hy000jin
❯ cd brewfile

~/home/workspace/hy000jin/brewfile master*
❯ git remote -v
origin	https://github.com/hy000jin/brewfile.git (fetch)
origin	https://github.com/hy000jin/brewfile.git (push)

~/home/workspace/hy000jin/brewfile master*
❯ git config --global user.email "hyooj10@gmail.com"

~/home/workspace/hy000jin/brewfile master*
❯ git config --global user.name "k1my0"

~/home/workspace/hy000jin/brewfile master*
❯ git remote -v
origin	https://github.com/hy000jin/brewfile.git (fetch)
origin	https://github.com/hy000jin/brewfile.git (push)

~/home/workspace/hy000jin/brewfile master*
❯ cd /Users/.ssh
cd: no such file or directory: /Users/.ssh

~/home/workspace/hy000jin/brewfile master*
❯ ls
Brewfile           README.md          id_rsa_hyooo
Brewfile.lock.json id_rsa_ctilab      id_rsa_hyooo.pub
LICENSE            id_rsa_ctilab.pub  initial

~/home/workspace/hy000jin/brewfile master*
❯ cd /Users/hyojinkim/.ssh

~/.ssh
❯ ls
config              id_rsa_ctilab.pub   id_rsa_hy000jin.pub id_rsa_k1my0.pub
id_rsa_ctilab       id_rsa_hy000jin     id_rsa_k1my0        known_hosts

~/.ssh
❯ vi config

~/.ssh 57s
❯ vi config

~/.ssh 1m 45s
❯ cd /Users/hyojinkim/home/workspace/hyo
cd: no such file or directory: /Users/hyojinkim/home/workspace/hyo

~/.ssh
❯ cd /Users/hyojinkim/home/workspace

~/home/workspace
❯ ls
ctilab   hy000jin tmp

~/home/workspace
❯ cd hy000jin

~/home/workspace/hy000jin
❯ ls
List                          TIL
Project                       Temp
Referrer                      brewfile
Snazzy.itermcolors            무제 폴더
Study                         손기정.docx

~/home/workspace/hy000jin
❯ cd brewfile

~/home/workspace/hy000jin/brewfile master*
❯ git remote -v
origin	https://github.com/hy000jin/brewfile.git (fetch)
origin	https://github.com/hy000jin/brewfile.git (push)

~/home/workspace/hy000jin/brewfile master*
❯ cd /Users/hyojinkim/.git
cd: no such file or directory: /Users/hyojinkim/.git

~/home/workspace/hy000jin/brewfile master*
❯ cd /Users/hyojinkim/.ssh

~/.ssh
❯ ls
config              id_rsa_ctilab.pub   id_rsa_hy000jin.pub id_rsa_k1my0.pub
id_rsa_ctilab       id_rsa_hy000jin     id_rsa_k1my0        known_hosts

~/.ssh
❯ cd /Users/hyojinkim/home/workspace/hy000jin

~/home/workspace/hy000jin
❯ ls
List                          TIL
Project                       Temp
Referrer                      brewfile
Snazzy.itermcolors            무제 폴더
Study                         손기정.docx

~/home/workspace/hy000jin
❯ cd brewfile

~/home/workspace/hy000jin/brewfile master*
❯ ls
Brewfile           README.md          id_rsa_hyooo
Brewfile.lock.json id_rsa_ctilab      id_rsa_hyooo.pub
LICENSE            id_rsa_ctilab.pub  initial

~/home/workspace/hy000jin/brewfile master*
❯ cd .git

~/home/workspace/hy000jin/brewfile/.git master
❯ ls
COMMIT_EDITMSG config         index          objects
FETCH_HEAD     description    info           refs
HEAD           hooks          logs

~/home/workspace/hy000jin/brewfile/.git master
❯ cd ..

~/home/workspace/hy000jin/brewfile master*
❯ ls
Brewfile           README.md          id_rsa_hyooo
Brewfile.lock.json id_rsa_ctilab      id_rsa_hyooo.pub
LICENSE            id_rsa_ctilab.pub  initial

~/home/workspace/hy000jin/brewfile master*
❯ git remote -v
origin	https://github.com/hy000jin/brewfile.git (fetch)
origin	https://github.com/hy000jin/brewfile.git (push)

~/home/workspace/hy000jin/brewfile master*
❯ git remote set-url origin git@github.com-k1my0:k1my0/brewfile.git

~/home/workspace/hy000jin/brewfile master*
❯ ssh -add -l
ssh: illegal option -- d
usage: ssh [-46AaCfGgKkMNnqsTtVvXxYy] [-B bind_interface]
           [-b bind_address] [-c cipher_spec] [-D [bind_address:]port]
           [-E log_file] [-e escape_char] [-F configfile] [-I pkcs11]
           [-i identity_file] [-J [user@]host[:port]] [-L address]
           [-l login_name] [-m mac_spec] [-O ctl_cmd] [-o option] [-p port]
           [-Q query_option] [-R address] [-S ctl_path] [-W host:port]
           [-w local_tun[:remote_tun]] destination [command]

~/home/workspace/hy000jin/brewfile master*
❯ ssh-add -l
2048 SHA256:rVYFISkOSWajK9ic8wAkMwJOJBT5BucvSlGPqr0RdKY cti.hyooo@gmail.com (RSA)
2048 SHA256:LTiv2ON+fjKnIEMgxzUPWP7X5/OpXsLT8MNIKB2vNwk hyooojin@ctilab.co.kr (RSA)
2048 SHA256:Hd6ivKCORAACRBUZADzh1jq/bl7/MW2yueQI158YwdQ hyooj10@gmail.com (RSA)

~/home/workspace/hy000jin/brewfile master*
❯ ls
Brewfile           README.md          id_rsa_hyooo
Brewfile.lock.json id_rsa_ctilab      id_rsa_hyooo.pub
LICENSE            id_rsa_ctilab.pub  initial

~/home/workspace/hy000jin/brewfile master*
❯ cd /.git
cd: no such file or directory: /.git

~/home/workspace/hy000jin/brewfile master*
❯ ls
Brewfile           README.md          id_rsa_hyooo
Brewfile.lock.json id_rsa_ctilab      id_rsa_hyooo.pub
LICENSE            id_rsa_ctilab.pub  initial

~/home/workspace/hy000jin/brewfile master*
❯ cd .git

~/home/workspace/hy000jin/brewfile/.git master
❯ ls
COMMIT_EDITMSG config         index          objects
FETCH_HEAD     description    info           refs
HEAD           hooks          logs

~/home/workspace/hy000jin/brewfile/.git master
❯ vi config

~/home/workspace/hy000jin/brewfile/.git master 18s
❯ cd ..

~/home/workspace/hy000jin/brewfile master*
❯ ssh -T git@github.com-k1my0
Hi k1my0! You've successfully authenticated, but GitHub does not provide shell access.

~/home/workspace/hy000jin/brewfile master*
❯ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	id_rsa_ctilab
	id_rsa_ctilab.pub
	id_rsa_hyooo
	id_rsa_hyooo.pub

nothing added to commit but untracked files present (use "git add" to track)

~/home/workspace/hy000jin/brewfile master*
❯ cd ..

~/home/workspace/hy000jin
❯ ls
List                          TIL
Project                       Temp
Referrer                      brewfile
Snazzy.itermcolors            무제 폴더
Study                         손기정.docx

~/home/workspace/hy000jin
❯ cd brewfile

~/home/workspace/hy000jin/brewfile master*
❯ ls
Brewfile           README.md          id_rsa_hyooo
Brewfile.lock.json id_rsa_ctilab      id_rsa_hyooo.pub
LICENSE            id_rsa_ctilab.pub  initial

~/home/workspace/hy000jin/brewfile master*
❯ rm -rf id_rsa_*

~/home/workspace/hy000jin/brewfile master
❯ ls
Brewfile           LICENSE            initial
Brewfile.lock.json README.md

~/home/workspace/hy000jin/brewfile master
❯ vi README.md

~/home/workspace/hy000jin/brewfile master* 1m 57s
❯ rm -rf initial

~/home/workspace/hy000jin/brewfile master*
❯ ls
Brewfile           Brewfile.lock.json LICENSE            README.md

~/home/workspace/hy000jin/brewfile master*
❯ rm -rf Brewfile.lock.json

~/home/workspace/hy000jin/brewfile master*
❯ ls
Brewfile  LICENSE   README.md

~/home/workspace/hy000jin/brewfile master*
❯ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	deleted:    Brewfile.lock.json
	modified:   README.md
	deleted:    initial

no changes added to commit (use "git add" and/or "git commit -a")

~/home/workspace/hy000jin/brewfile master*
❯ git add .

~/home/workspace/hy000jin/brewfile master*
❯ git commit -m "brewfile update"
[master ce39893] brewfile update
 3 files changed, 4 insertions(+), 679 deletions(-)
 delete mode 100644 Brewfile.lock.json
 delete mode 100644 initial

~/home/workspace/hy000jin/brewfile master ⇡
❯ git push origin master
To github.com-k1my0:k1my0/brewfile.git
 ! [rejected]        master -> master (non-fast-forward)
error: failed to push some refs to 'git@github.com-k1my0:k1my0/brewfile.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

~/home/workspace/hy000jin/brewfile master ⇡
❯ git checkout -b hyojinkim
Switched to a new branch 'hyojinkim'

~/home/workspace/hy000jin/brewfile hyojinkim
❯ git checkout master
Switched to branch 'master'
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

~/home/workspace/hy000jin/brewfile master ⇡
❯ git pull origin master
From github.com-k1my0:k1my0/brewfile
 * branch            master     -> FETCH_HEAD
 + d1f5092...ae6e72c master     -> origin/master  (forced update)
fatal: refusing to merge unrelated histories

~/home/workspace/hy000jin/brewfile master ⇣⇡
❯ git pull origin master --allow-unrelated-histories
From github.com-k1my0:k1my0/brewfile
 * branch            master     -> FETCH_HEAD
CONFLICT (add/add): Merge conflict in README.md
Auto-merging README.md
Automatic merge failed; fix conflicts and then commit the result.

~/home/workspace/hy000jin/brewfile master|merge* ⇣⇡
❯ ls
Brewfile  LICENSE   README.md

~/home/workspace/hy000jin/brewfile master|merge* ⇣⇡
❯ vi README.md

~/home/workspace/hy000jin/brewfile master|merge* ⇣⇡ 14s
❯ git checkout hyojinkim
README.md: needs merge
error: you need to resolve your current index first

~/home/workspace/hy000jin/brewfile master|merge* ⇣⇡
❯ git remote -v
origin	git@github.com-k1my0:k1my0/brewfile.git (fetch)
origin	git@github.com-k1my0:k1my0/brewfile.git (push)

~/home/workspace/hy000jin/brewfile master|merge* ⇣⇡
❯ ls
Brewfile  LICENSE   README.md

~/home/workspace/hy000jin/brewfile master|merge* ⇣⇡
❯ cd ..

~/home/workspace/hy000jin
❯ ls
List                          Study                         brewfile2
Project                       TIL                           무제 폴더
Referrer                      Temp                          손기정.docx
Snazzy.itermcolors            brewfile

~/home/workspace/hy000jin
❯ cd brewfile

~/home/workspace/hy000jin/brewfile master
❯ ls
Brewfile  LICENSE   README.md

~/home/workspace/hy000jin/brewfile master
❯ vi README.md

~/home/workspace/hy000jin/brewfile master 11s
❯ cd ..

~/home/workspace/hy000jin
❯ ls
List                          Study                         brewfile2
Project                       TIL                           무제 폴더
Referrer                      Temp                          손기정.docx
Snazzy.itermcolors            brewfile

~/home/workspace/hy000jin
❯ cd brewfile

~/home/workspace/hy000jin/brewfile master
❯ ls
Brewfile  LICENSE   README.md

~/home/workspace/hy000jin/brewfile master
❯ git checkout hyojinkim
Switched to branch 'hyojinkim'

~/home/workspace/hy000jin/brewfile hyojinkim
❯ ls
Brewfile  LICENSE   README.md

~/home/workspace/hy000jin/brewfile hyojinkim
❯ vi README.md

~/home/workspace/hy000jin/brewfile hyojinkim 10s
❯ git pull origin master
From github.com-k1my0:k1my0/brewfile
 * branch            master     -> FETCH_HEAD
Updating ce39893..6b1c6ef
Fast-forward
 README.md | 5 +++++
 1 file changed, 5 insertions(+)
commit 541cf80b88d32cdb66da4461a999033f920003bb (HEAD -> hyojinkim)
Author: hy000jin <cti.hyooo@gmail.com>
Date:   Sat Nov 23 19:48:26 2019 +0900

    brewfile update

commit a1c02e1ea009d548ef4bf5032f4623a205f86e81
Author: HyoJin Kim <hyojinkim@HyoJinui-MacBookPro.local>
Date:   Mon Jul 15 23:29:20 2019 +0900

    update brewfile

commit 4a96cdc27fc7a74363feadb9d42bb875b50ad773
Author: HyoJin Kim <hyojinkim@HyoJinui-MacBookPro.local>
Date:   Sun May 5 19:14:16 2019 +0900

    Add 'r' and 'r-studio'

commit 479b7116b1cff8c228361f3bf6023bcab30b8c4e
Author: HyoJin Kim <hyojinkim@HyoJinui-MacBookPro.local>
Date:   Sat May 4 20:42:49 2019 +0900

    add visual studio code

commit 9db833d821ed46e5c73a12066500b6de9c90ea57
Author: HyoJin Kim <hyojinkim@HyoJinui-MacBookPro.local>
Date:   Tue Apr 30 16:25:03 2019 +0900

    Initialize Brewfile
commit 541cf80b88d32cdb66da4461a999033f920003bb (HEAD -> hyojinkim)
commit 541cf80b88d32cdb66da4461a999033f920003bb (HEAD -> hyojinkim)
Author: hy000jin <cti.hyooo@gmail.com>
Date:   Sat Nov 23 19:48:26 2019 +0900

    brewfile update

commit a1c02e1ea009d548ef4bf5032f4623a205f86e81
Author: HyoJin Kim <hyojinkim@HyoJinui-MacBookPro.local>
Date:   Mon Jul 15 23:29:20 2019 +0900

    update brewfile

commit 4a96cdc27fc7a74363feadb9d42bb875b50ad773
Author: HyoJin Kim <hyojinkim@HyoJinui-MacBookPro.local>
Date:   Sun May 5 19:14:16 2019 +0900

    Add 'r' and 'r-studio'

commit 479b7116b1cff8c228361f3bf6023bcab30b8c4e
Author: HyoJin Kim <hyojinkim@HyoJinui-MacBookPro.local>
Date:   Sat May 4 20:42:49 2019 +0900

    add visual studio code

commit 9db833d821ed46e5c73a12066500b6de9c90ea57
Author: HyoJin Kim <hyojinkim@HyoJinui-MacBookPro.local>
Date:   Tue Apr 30 16:25:03 2019 +0900

    Initialize Brewfile

~/home/workspace/hy000jin/brewfile hyojinkim
❯ git reset HEAD~1
Unstaged changes after reset:
M	README.md

~/home/workspace/hy000jin/brewfile hyojinkim*
❯ vi README.md

~/home/workspace/hy000jin/brewfile hyojinkim* 10s
❯ git reset HEAD~2
Unstaged changes after reset:
D	Brewfile.lock.json
M	README.md

~/home/workspace/hy000jin/brewfile hyojinkim*
❯ ls
Brewfile  LICENSE   README.md

~/home/workspace/hy000jin/brewfile hyojinkim*
❯ vi README.md

~/home/workspace/hy000jin/brewfile hyojinkim* 6s
❯ git log

~/home/workspace/hy000jin/brewfile hyojinkim* 2m 52s
❯ git checkout 541cf80b88d32cdb66da4461a999033f920003bb
D	Brewfile.lock.json
M	README.md
Note: switching to '541cf80b88d32cdb66da4461a999033f920003bb'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at 541cf80 brewfile update

~/home/workspace/hy000jin/brewfile heads/hyojinkim*
❯ git state
git: 'state' is not a git command. See 'git --help'.

The most similar command is
	stage

~/home/workspace/hy000jin/brewfile heads/hyojinkim*
❯ git status
HEAD detached at 541cf80
Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	deleted:    Brewfile.lock.json
	modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

~/home/workspace/hy000jin/brewfile heads/hyojinkim*
❯ ls
Brewfile  LICENSE   README.md

~/home/workspace/hy000jin/brewfile heads/hyojinkim*
❯ vi README.md

~/home/workspace/hy000jin/brewfile heads/hyojinkim* 17s
❯ git log

~/home/workspace/hy000jin/brewfile heads/hyojinkim* 8s
❯ git checkout a1c02e1ea009d548ef4bf5032f4623a205f86e81
M	README.md
Previous HEAD position was 541cf80 brewfile update
HEAD is now at a1c02e1 update brewfile

~/home/workspace/hy000jin/brewfile a1c02e1...*
❯ ls
Brewfile  LICENSE   README.md

~/home/workspace/hy000jin/brewfile a1c02e1...*
❯ vi README.md

~/home/workspace/hy000jin/brewfile a1c02e1...* 8s
❯ git log

~/home/workspace/hy000jin/brewfile a1c02e1...* 8s
❯ git checkout 479b7116b1cff8c228361f3bf6023bcab30b8c4e
M	README.md
Previous HEAD position was a1c02e1 update brewfile
HEAD is now at 479b711 add visual studio code

~/home/workspace/hy000jin/brewfile 479b711...*
❯ ls
Brewfile  LICENSE   README.md

~/home/workspace/hy000jin/brewfile 479b711...*
❯ vi README.md

~/home/workspace/hy000jin/brewfile 479b711...* 17s
❯ git checkout master
error: Your local changes to the following files would be overwritten by checkout:
	README.md
Please commit your changes or stash them before you switch branches.
Aborting

~/home/workspace/hy000jin/brewfile 479b711...*
❯ git stash
Saved working directory and index state WIP on (no branch): 479b711 add visual studio code

~/home/workspace/hy000jin/brewfile 479b711...
❯ git checkout master
Previous HEAD position was 479b711 add visual studio code
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

~/home/workspace/hy000jin/brewfile master
❯ git log

~/home/workspace/hy000jin/brewfile master 20s
❯ git checkout ce39893a7d10885eca0c879f07d25b55c7b31b28
Note: switching to 'ce39893a7d10885eca0c879f07d25b55c7b31b28'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at ce39893 brewfile update

~/home/workspace/hy000jin/brewfile ce39893...
❯ ls
Brewfile  LICENSE   README.md

~/home/workspace/hy000jin/brewfile ce39893...
❯ vi README.md

~/home/workspace/hy000jin/brewfile ce39893... 13s
❯ git push orign master
fatal: 'orign' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

~/home/workspace/hy000jin/brewfile ce39893...
❯ git reset ce39893a7d10885eca0c879f07d25b55c7b31b28

~/home/workspace/hy000jin/brewfile ce39893...
❯ git checkout master
Previous HEAD position was ce39893 brewfile update
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

~/home/workspace/hy000jin/brewfile master
❯ git reset ce39893a7d10885eca0c879f07d25b55c7b31b28
Unstaged changes after reset:
M	README.md

~/home/workspace/hy000jin/brewfile master* ⇣
❯ git status
On branch master
Your branch is behind 'origin/master' by 2 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")

~/home/workspace/hy000jin/brewfile master* ⇣
❯ vi README.md

~/home/workspace/hy000jin/brewfile master* ⇣ 7s
❯ git log

~/home/workspace/hy000jin/brewfile master* ⇣ 8s
❯ git checkout ce39893a7d10885eca0c879f07d25b55c7b31b28
M	README.md
Note: switching to 'ce39893a7d10885eca0c879f07d25b55c7b31b28'.

You are in 'detached HEAD' state. You can look around, make experimental
changes and commit them, and you can discard any commits you make in this
state without impacting any branches by switching back to a branch.

If you want to create a new branch to retain commits you create, you may
do so (now or later) by using -c with the switch command. Example:

  git switch -c <new-branch-name>

Or undo this operation with:

  git switch -

Turn off this advice by setting config variable advice.detachedHead to false

HEAD is now at ce39893 brewfile update

~/home/workspace/hy000jin/brewfile heads/master*
❯ ls
Brewfile  LICENSE   README.md

~/home/workspace/hy000jin/brewfile heads/master*
❯ vi README.md

~/home/workspace/hy000jin/brewfile heads/master* 7s
❯ git log

~/home/workspace/hy000jin/brewfile heads/master* 9s
❯ git checkout d1f5092be2fb92047b6f0cd8597b51add62c7c6a
error: Your local changes to the following files would be overwritten by checkout:
	README.md
Please commit your changes or stash them before you switch branches.
Aborting

~/home/workspace/hy000jin/brewfile heads/master*
❯ git stash
Saved working directory and index state WIP on (no branch): ce39893 brewfile update

~/home/workspace/hy000jin/brewfile heads/master
❯ git checkout d1f5092be2fb92047b6f0cd8597b51add62c7c6a
Previous HEAD position was ce39893 brewfile update
HEAD is now at d1f5092 initial commit

~/home/workspace/hy000jin/brewfile d1f5092...
❯ vi README.md

~/home/workspace/hy000jin/brewfile d1f5092... 13s
❯ git checkout master
Previous HEAD position was d1f5092 initial commit
Switched to branch 'master'
Your branch is behind 'origin/master' by 2 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

~/home/workspace/hy000jin/brewfile master ⇣
❯ git reset d1f5092be2fb92047b6f0cd8597b51add62c7c6a
Unstaged changes after reset:
D	Brewfile.lock.json
M	README.md
D	initial

~/home/workspace/hy000jin/brewfile master* ⇣
❯ git status
On branch master
Your branch is behind 'origin/master' by 3 commits, and can be fast-forwarded.
  (use "git pull" to update your local branch)

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	deleted:    Brewfile.lock.json
	modified:   README.md
	deleted:    initial

no changes added to commit (use "git add" and/or "git commit -a")

~/home/workspace/hy000jin/brewfile master* ⇣
❯ git add .

~/home/workspace/hy000jin/brewfile master* ⇣
❯ git commit -m "brewfile update"
[master b8cdef7] brewfile update
 3 files changed, 4 insertions(+), 679 deletions(-)
 delete mode 100644 Brewfile.lock.json
 delete mode 100644 initial

~/home/workspace/hy000jin/brewfile master ⇣⇡
❯ git push origin master
To github.com-k1my0:k1my0/brewfile.git
 ! [rejected]        master -> master (non-fast-forward)
error: failed to push some refs to 'git@github.com-k1my0:k1my0/brewfile.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. Integrate the remote changes (e.g.
hint: 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

~/home/workspace/hy000jin/brewfile master ⇣⇡
❯ git branch -D hyojinkim
Deleted branch hyojinkim (was 541cf80).

~/home/workspace/hy000jin/brewfile master ⇣⇡
❯ git checkout -b hyojinkim
Switched to a new branch 'hyojinkim'

~/home/workspace/hy000jin/brewfile hyojinkim
❯ vi README.md

~/home/workspace/hy000jin/brewfile hyojinkim 21s
❯ git checkout master
Switched to branch 'master'
Your branch and 'origin/master' have diverged,
and have 1 and 3 different commits each, respectively.
  (use "git pull" to merge the remote branch into yours)

~/home/workspace/hy000jin/brewfile master ⇣⇡
❯ vi README.md

~/home/workspace/hy000jin/brewfile master ⇣⇡ 10s
❯ git pull origin master
From github.com-k1my0:k1my0/brewfile
 * branch            master     -> FETCH_HEAD
Auto-merging README.md
Merge made by the 'recursive' strategy.
 README.md | 5 +++++
 1 file changed, 5 insertions(+)

~/home/workspace/hy000jin/brewfile master ⇡ 19s
❯ vi README.md

~/home/workspace/hy000jin/brewfile master ⇡
❯ git checkout hyojinkim
Switched to branch 'hyojinkim'

~/home/workspace/hy000jin/brewfile hyojinkim
❯ git status
On branch hyojinkim
nothing to commit, working tree clean

~/home/workspace/hy000jin/brewfile hyojinkim
❯ git push origin master
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 497 bytes | 497.00 KiB/s, done.
Total 4 (delta 2), reused 0 (delta 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com-k1my0:k1my0/brewfile.git
   6b1c6ef..518712c  master -> master

~/home/workspace/hy000jin/brewfile hyojinkim
❯ git checkout master
Switched to branch 'master'
Your branch is up to date with 'origin/master'.

~/home/workspace/hy000jin/brewfile master
❯ git pull origin master
From github.com-k1my0:k1my0/brewfile
 1 README.md                                                                               Buffers
 12 <<<<<<< HEAD
 11 <div align="center">
 10   <h1>Brewfile</h1>
  9 </div>
  8
  7 <p align="center">
  6   :apple: Brewfile to install softwares in macOS for engineers
  5 </p>
  4
  3 <div align="center">
  2   <a href="https://opensource.org/licenses/mit-license.php">
  1   ┊ <img alt="MIT License" src="https://badges.frapsoft.com/os/mit/mit.svg?v=103" />
13    </a>
  1   <a href="https://github.com/ellerbrock/open-source-badge/">
  2   ┊ <img alt="Open Source Love" src="https://badges.frapsoft.com/os/v1/open-source.svg?v=103" /
  3   </a>
  4 </div>
  5
  6 <br />
  7
  8 [This brewfile](https://github.com/k1my0/brewfile) is written by [k1my0](https://github.com/k1m
  9
 1  - 1.4k README.md  markdown  # s                                        unix | utf-8  13:6  Top
