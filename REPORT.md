ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~$ export GITHUB_USERNAME=Lopatukhin
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~$ export GITHUB_EMAIL=thegoldenorder112@gmail.com
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~$ export GITHUB_TOKEN=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
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~$ alias edit=<nano|vi|vim|subl>
bash: syntax error near unexpected token `newline'
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~$ cd ${GITHUB_USERNAME}/workspace
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ source scripts/activate
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ mkdir ~/.config
mkdir: cannot create directory ‘/home/ilia_lopatukhin/.config’: File exists
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ cat > ~/.config/hub <<EOF
> github.com:
- user: ${GITHUB_USERNAME}
  oauth_token: ${GITHUB_TOKEN}
  protocol: https
> EOF
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$  git config --global hub.protocol https
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ mkdir projects/lab02 && cd projects/lab02
mkdir: cannot create directory ‘projects/lab02’: File exists
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ cd projects/lab02
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git init
Reinitialized existing Git repository in /home/ilia_lopatukhin/Lopatukhin/workspace/projects/lab02/.git/
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git config --global user.name ${GITHUB_USERNAME}
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git config --global user.email ${GITHUB_EMAIL}
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git remote add origin https://github.com/${GITHUB_USERNAME}/lab02.git
error: remote origin already exists.
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git pull origin master
Username for 'https://github.com': Lopatukhin
Password for 'https://Lopatukhin@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/Lopatukhin/lab02.git/'
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ gut pull origin main
Command 'gut' not found, did you mean:
  command 'gum' from snap gum (0.13.0)
  command 'got' from deb got (0.95-1)
  command 'cut' from deb coreutils (9.4-2ubuntu2)
  command 'gt' from deb genometools (1.6.5+ds-2)
  command 'gout' from deb scotch (7.0.4-1)
  command 'hut' from deb hut (0.4.0-1ubuntu0.2)
  command 'git' from deb git (1:2.43.0-1ubuntu7.2)
  command 'nut' from deb nutsqlite (2.0.6-4)
  command 'gpt' from deb gpt (1.1-7)
  command 'lut' from deb tracetuner (3.0.6~beta+dfsg-3)
  command 'gmt' from deb gmt (6.4.0+dfsg-2build2)
See 'snap info <snapname>' for additional versions.
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git pull origin main
Username for 'https://github.com': Lopatukhin
Password for 'https://Lopatukhin@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/Lopatukhin/lab02.git/'
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git pull origin main
Username for 'https://github.com': Lopatukhin
Password for 'https://Lopatukhin@github.com': 
remote: Repository not found.
fatal: repository 'https://github.com/Lopatukhin/lab02.git/' not found
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git pull origin main
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 1.44 KiB | 1.44 MiB/s, done.
From https://github.com/Lopatukhin/lab02
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
hint: You have divergent branches and need to specify how to reconcile them.
hint: You can do so by running one of the following commands sometime before
hint: your next pull:
hint: 
hint:   git config pull.rebase false  # merge
hint:   git config pull.rebase true   # rebase
hint:   git config pull.ff only       # fast-forward only
hint: 
hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per
hint: invocation.
fatal: Need to specify how to reconcile divergent branches.
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ touch README.md
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	tasks/

nothing added to commit but untracked files present (use "git add" to track)
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git add README.md
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git commit -m"added README.md"
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	tasks/

nothing added to commit but untracked files present (use "git add" to track)
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git push origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/Lopatukhin/lab02.git'
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git push origin master
Username for 'https://github.com': Lopatukhin
Password for 'https://Lopatukhin@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/Lopatukhin/lab02.git/'
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git push origin master
Username for 'https://github.com': Lopatukhin
Password for 'https://Lopatukhin@github.com': 
remote: Support for password authentication was removed on August 13, 2021.
remote: Please see https://docs.github.com/get-started/getting-started-with-git/about-remote-repositories#cloning-with-https-urls for information on currently recommended modes of authentication.
fatal: Authentication failed for 'https://github.com/Lopatukhin/lab02.git/'
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ ls
examples  include  README.md  sources  tasks
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git push origin master
Username for 'https://github.com': Lopatukhin
Password for 'https://Lopatukhin@github.com': 
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 12 threads
Compressing objects: 100% (8/8), done.
Writing objects: 100% (12/12), 1.07 KiB | 1.07 MiB/s, done.
Total 12 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/Lopatukhin/lab02/pull/new/master
remote: 
To https://github.com/Lopatukhin/lab02.git
 * [new branch]      master -> master
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ *build*/
bash: *build*/: No such file or directory
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git pull origin master
From https://github.com/Lopatukhin/lab02
 * branch            master     -> FETCH_HEAD
Already up to date.
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git log
commit a5aceed602e102f9b2728413b84bf7fbbfe225c7 (HEAD -> master, origin/master)
Author: Lopatukhin <thegoldenorder112@gmail.com>
Date:   Sat Jun 14 22:50:21 2025 +0300

    added sources

commit d8089fdaeb3a816fda880e5b5e3ea1abd8153120
Author: Lopatukhin <thegoldenorder112@gmail.com>
Date:   Sat Jun 14 21:04:30 2025 +0300

    added README.md
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ mkdir sources
mkdir: cannot create directory ‘sources’: File exists
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ mkdir include
mkdir: cannot create directory ‘include’: File exists
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ mkdir examples
mkdir: cannot create directory ‘examples’: File exists
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ cat > sources/print.cpp <<EOF
> #include <print.hpp>

void print(const std::string& text, std::ostream& out)
{
  out << text;
}

void print(const std::string& text, std::ofstream& out)
{
  out << text;
}
EOF
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ cat > include/print.hpp <<EOF
> #include <fstream>
#include <iostream>
#include <string>

void print(const std::string& text, std::ofstream& out);
void print(const std::string& text, std::ostream& out = std::cout);
EOF
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ cat > examples/example1.cpp <<EOF
> #include <print.hpp>

int main(int argc, char** argv)
{
  print("hello");
}
EOF
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ cat > examples/example2.cpp <<EOF
> #include <print.hpp>

#include <fstream>

int main(int argc, char** argv)
{
  std::ofstream file("log.txt");
  print(std::string("hello"), file);
}
EOF
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ edit README.md
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
	tasks/

nothing added to commit but untracked files present (use "git add" to track)
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git add 
Nothing specified, nothing added.
hint: Maybe you wanted to say 'git add .'?
hint: Turn this message off by running
hint: "git config advice.addEmptyPathspec false"
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git add .
warning: adding embedded git repository: tasks/lab02
hint: You've added another git repository inside your current repository.
hint: Clones of the outer repository will not contain the contents of
hint: the embedded repository and will not know how to obtain it.
hint: If you meant to add a submodule, use:
hint: 
hint: 	git submodule add <url> tasks/lab02
hint: 
hint: If you added this path by mistake, you can remove it from the
hint: index with:
hint: 
hint: 	git rm --cached tasks/lab02
hint: 
hint: See "git help submodule" for more information.
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git commit -m"added sources"
[master aa1e60a] added sources
 1 file changed, 1 insertion(+)
 create mode 160000 tasks/lab02
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git push origin master
Username for 'https://github.com': Lopatukhin
Password for 'https://Lopatukhin@github.com': 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 302 bytes | 302.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Lopatukhin/lab02.git
   a5aceed..aa1e60a  master -> master
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ cd ~/workspace/
bash: cd: /home/ilia_lopatukhin/workspace/: No such file or directory
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ popd
bash: popd: directory stack empty
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ cd ~/workspace/
bash: cd: /home/ilia_lopatukhin/workspace/: No such file or directory
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ cd ..
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects$ cd ..
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ export LAB_NUMBER=02
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ git clone https://github.com/tp-labs/lab${LAB_NUMBER}.git tasks/lab${LAB_NUMBER}
Cloning into 'tasks/lab02'...
remote: Enumerating objects: 96, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 96 (delta 0), reused 1 (delta 0), pack-reused 93 (from 1)
Receiving objects: 100% (96/96), 1.29 MiB | 1.16 MiB/s, done.
Resolving deltas: 100% (28/28), done.
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ mkdir reports/lab${LAB_NUMBER}
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ cd reports/lab${LAB_NUMBER}
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/reports/lab02$ edit REPORT.md
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/reports/lab02$ gist REPORT.md
Error: Got Net::HTTPUnauthorized from gist: {"message":"Bad credentials","documentation_url":"https://docs.github.com/rest","status":"401"}
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/reports/lab02$ ls
REPORT.md
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/reports/lab02$ cd ..
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/reports$ cd ..
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace$ cd projects
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects$ cd lab02
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ ls
examples  include  README.md  sources  tasks
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git remote add origin https://github.com/Lopatukhin/lab02
error: remote origin already exists.
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git push -u origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/Lopatukhin/lab02.git'
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git push -u origin master
Username for 'https://github.com': Lopatukhin
Password for 'https://Lopatukhin@github.com': 
branch 'master' set up to track 'origin/master'.
Everything up-to-date
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git checkout master
Already on 'master'
Your branch is up to date with 'origin/master'.
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git checkout -b main
Switched to a new branch 'main'
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ git push -u origin main
Username for 'https://github.com': Lopatukhin
Password for 'https://Lopatukhin@github.com': 
To https://github.com/Lopatukhin/lab02.git
 ! [rejected]        main -> main (non-fast-forward)
error: failed to push some refs to 'https://github.com/Lopatukhin/lab02.git'
hint: Updates were rejected because the tip of your current branch is behind
hint: its remote counterpart. If you want to integrate the remote changes,
hint: use 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
ilia_lopatukhin@Ilia-lopatukhin-Y3-Max:~/Lopatukhin/workspace/projects/lab02$ 

