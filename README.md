# test-conflict

Voici une ligne du README.md avec deux fautes de frappe à corriger

-----------------------
zineddine@MacBook-Air-de-Zineddine test-conflict % git pull

error: Pulling is not possible because you have unmerged files.

hint: Fix them up in the work tree, and then use 'git add/rm <file>'

hint: as appropriate to mark resolution and make a commit.

fatal: Exiting because of an unresolved conflict.

zineddine@MacBook-Air-de-Zineddine test-conflict % git diff

diff --cc README.md

index b3bf9f6,ec9ffe0..0000000

--- a/README.md

+++ b/README.md

@@@ -1,3 -1,3 +1,7 @@@

----------------------------

  

++<<<<<<< HEAD

+Voici une ligne du README.md avec deux fautes de frappe à corriger

++=======

+ Voici une ligne du README.md avec deux (deux) fotes de frape (fautes de frappe) à corriger

++>>>>>>> 9cef7817032fddc4f7cf194b831ec20cf2dd93a5

-------------------------


-------------


zineddine@MacBook-Air-de-Zineddine test-conflict % git push
To github.com:zineddineghl/test-conflict.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'github.com:zineddineghl/test-conflict.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
zineddine@MacBook-Air-de-Zineddine test-conflict % git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (1/1), done.
remote: Total 3 (delta 1), reused 3 (delta 1), pack-reused 0
Unpacking objects: 100% (3/3), 265 bytes | 66.00 KiB/s, done.
From github.com:zineddineghl/test-conflict
   bb8515a..9cef781  main       -> origin/main
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
