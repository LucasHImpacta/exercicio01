PASSO a):

@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 $ echo 01 > arquivo.txt
@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 $ cat arquivo.txt 
01



PASSO b):



@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status 
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        arquivo.txt

nothing added to commit but untracked files present (use "git add" to track)
@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 



PASSO c):




@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add arquivo.txt 
@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status 
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   arquivo.txt

@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 





PASSO d,e):




@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 02 > arquivo.txt
@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff arquivo.txt
diff --git a/arquivo.txt b/arquivo.txt
index 8a0f05e..9e22bcb 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-01
+02
@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 





PASSO f):



@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add arquivo.txt 
@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   arquivo.txt

@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 





PASSO g):




@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff arquivo.txt
@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 





PASSO h,i):




@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo 03 > arquivo.txt
@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git diff arquivo.txt
diff --git a/arquivo.txt b/arquivo.txt
index 9e22bcb..75016ea 100644
--- a/arquivo.txt
+++ b/arquivo.txt
@@ -1 +1 @@
-02
+03




PASSO j):




@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git restore arquivo.txt
@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   arquivo.txt

@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 




PASSO k):




@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m "Meu Primeiro commit"
[main (root-commit) 1a9e45f] Meu Primeiro commit
 1 file changed, 1 insertion(+)
 create mode 100644 arquivo.txt
@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git log 
commit 1a9e45ff3a77f9de76b1ff8ad5c0f6d08f905720 (HEAD -> main)
Author: Lucas Henrique <lucas.lmendonca@aluno.faculdadeimpacta.com.br>
Date:   Fri Aug 9 22:58:07 2024 +0000

    Meu Primeiro commit
@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 




PASSO l):




@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ cat .gitignore
*.txt@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git add .gitignore 
@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git commit -m "Adicionando arquivo gitignore"
[main f030cbe] Adicionando arquivo gitignore
 1 file changed, 1 insertion(+)
 create mode 100644 .gitignore




PASSO m):




@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ echo teste > novo.txt
@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ git status
On branch main
nothing to commit, working tree clean
@LucasHImpacta ➜ /workspaces/codespaces-blank/exercicio01 (main) $ 
