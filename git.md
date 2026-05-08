Esercizio 1
comandi usati

1. mkdir portfolio-studente
2. cd portfolio-studente
3. touch index.html style.css README.md
4. start index.html
5. start style.css
6. start README.md
7. git init
8. git status
9. git add
10. git commit
11. git log

$ git status
On branch master
nothing to commit, working tree clean

$ git log --oneline
f1f0622 (HEAD -> master) Quarto commit: Stesura finale di readme.md
66c5c24 Terzo commit: aggiunta la sezione -Progetti-
9add01e Secondo commit: aggiunta contenuto iniziale ai file index.html e style.css
ecc1aa6 Primo commit: aggiunta struttura iniziale del progetto

Esercizio 2
link git hub https://github.com/gabgigante/portfolio-studente-github.git
comandi usati

1. git remote add origin https://github.com/gabgigante/portfolio-studente-github.git
2. git push -u origin main
3. git remote -v
   origin https://github.com/gabgigante/portfolio-studente-github.git (fetch)
   origin https://github.com/gabgigante/portfolio-studente-github.git (push)
4. git add README.md
5. git add git.md
6. git commit -m "Quinto commit: aggiunta di git.md alla repository e di descrizione Git a README.md"
7. git status
   On branch main
   Your branch is up to date with 'origin/main'.

   nothing to commit, working tree clean

8. git log --oneline
   0b4e8c4 (HEAD -> main, origin/main) no comment
   d5595af Quinto commit: aggiunta di git.md alla repository e di descrizione Git a README.md
   f1f0622 Quarto commit: Stesura finale di readme.md
   66c5c24 Terzo commit: aggiunta la sezione -Progetti-
   9add01e Secondo commit: aggiunta contenuto iniziale ai file index.html e style.css
   ecc1aa6 Primo commit: aggiunta struttura iniziale del progetto

esercizio 3

1. git switch -c branch
2. git add index.html style.css
3. git commit -m "Aggiunte modifiche a index e style"
4. git push -u origin branch
5. git pull
6. git branch -v
   branch 45bd71a modifica style.css esercizio 3 (aggiunta .progetto)

- main 5a83b97 Merge pull request #1 from gabgigante/branch

7.  git log --oneline
    5a83b97 (HEAD -> main, origin/main, origin/HEAD) Merge pull request #1 from gabgigante/branch
    45bd71a (origin/branch, branch) modifica style.css esercizio 3 (aggiunta .progetto)
    22e0178 modifica index.html esercizio 3 (aggiunta Progetti)
    66081e5 no comment
    0b4e8c4 no comment
    d5595af Quinto commit: aggiunta di git.md alla repository e di descrizione Git a README.md
    f1f0622 Quarto commit: Stesura finale di readme.md
    66c5c24 Terzo commit: aggiunta la sezione -Progetti-
    9add01e Secondo commit: aggiunta contenuto iniziale ai file index.html e style.css
    ecc1aa6 Primo commit: aggiunta struttura iniziale del progetto
