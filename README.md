# ApprendreGit
=>mkdir AndroidProjet
=>cd AndroidProjet
=>git init
  Initialized empty Git repository in C:/Users/user/AndroidProjet/.git/
=>git status
  On branch master
  No commits yet
  nothing to commit (create/copy files and use "git add" to track)

=>git add index.html
=>git commit -m "first commit"
  [master (root-commit) a69297d] first commit
  1 file changed, 8 insertions(+)
  create mode 100644 index.html

=>git add index.html
=>git commit -m "modifier la couleur du fond"
  [master dcc214d] modifier la couleur du fond
   1 file changed, 3 insertions(+), 3 deletions(-)

=>git log
  commit dcc214d4e5f6de8d88141de05278e7802c26895e (HEAD -> master)
  Author: Ikram Idrissi 
  Date:   Sun Oct 21 16:25:53 2018 +0100
  modifier la couleur du fond
  commit a69297df5fb84a452322c4e1961ee0bd63b95fdb
  Author: Ikram Idrissi
  Date:   Sun Oct 21 16:22:42 2018 +0100
  first commit

=>git branch
  * master

=>git branch backgroundcolor

=>git branch
  backgroundcolor
  * master

=>git checkout backgroundcolor
  Switched to branch 'backgroundcolor'

=>git add index.html
=>git commit -m "modfifer la couleur du titre"
  [backgroundcolor 2aae090] modfifer la couleur du titre
   1 file changed, 1 insertion(+), 1 deletion(-)

=>git log
  commit 2aae0904f4565e07ae012cc68514c2b60cd5ca75 (HEAD -> backgroundcolor)
  Author: Ikram Idrissi
  Date:   Sun Oct 21 16:32:09 2018 +0100
  modfifer la couleur du titre
  commit dcc214d4e5f6de8d88141de05278e7802c26895e (master)
  Author: Ikram Idrissi 
  Date:   Sun Oct 21 16:25:53 2018 +0100
  modifier la couleur du fond
  commit a69297df5fb84a452322c4e1961ee0bd63b95fdb
  Author: Ikram Idrissi 
  Date:   Sun Oct 21 16:22:42 2018 +0100
  first commit

=>git checkout master
  Switched to branch 'master'

=>git merge backgroundcolor
  Updating dcc214d..2aae090
  Fast-forward
  index.html | 2 +-
  1 file changed, 1 insertion(+), 1 deletion(-)

=>git branch -d backgroundcolor
  Deleted branch backgroundcolor (was 2aae090).

=>git log
  commit 2aae0904f4565e07ae012cc68514c2b60cd5ca75 (HEAD -> master)
  Author: Ikram Idrissi 
  Date:   Sun Oct 21 16:32:09 2018 +0100
  modfifer la couleur du titre
  commit dcc214d4e5f6de8d88141de05278e7802c26895e
  Author: Ikram Idrissi
  Date:   Sun Oct 21 16:25:53 2018 +0100
  modifier la couleur du fond
  commit a69297df5fb84a452322c4e1961ee0bd63b95fdb
  Author: Ikram Idrissi 
  Date:   Sun Oct 21 16:22:42 2018 +0100
  first commit

=>=>git remote add origin https://github.com/kIdrissiIkram/ApprendreGit.git
=>git remote
  origin

=>git push origin master
  Enumerating objects: 9, done.
  Counting objects: 100% (9/9), done.
  Delta compression using up to 4 threads
  Compressing objects: 100% (6/6), done.
  Writing objects: 100% (9/9), 878 bytes | 439.00 KiB/s, done.
  Total 9 (delta 2), reused 0 (delta 0)
  remote: Resolving deltas: 100% (2/2), done.
  remote:
  remote: Create a pull request for 'master' on GitHub by visiting:
  remote:      https://github.com/kIdrissiIkram/ApprendreGit/pull/new/master
  remote:
  To https://github.com/kIdrissiIkram/ApprendreGit.git
  * [new branch]      master -> master
