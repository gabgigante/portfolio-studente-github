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
8.  git status
    On branch main
    Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

domande di teoria

1. Un branch (ramo) è una linea temporale parallela. Quando crei un branch, stai facendo una copia esatta del progetto in quel momento per lavorarci sopra senza toccare il "tronco" principale.
2. Un branch è utile perchè senza di loro, ogni modifica finirebbe subito nel codice principale. Usarli è fondamentale perché:

- Isolamento: Puoi lavorare su una nuova funzione (feature) o correggere un bug senza rischiare di rompere la versione del software che i tuoi utenti stanno usando.
- Sperimentazione: Puoi provare idee folli: se non funzionano, cancelli il branch e il progetto principale resta intatto.
- Collaborazione: Più persone possono lavorare a diverse parti dello stesso progetto contemporaneamente senza sovrascriversi a vicenda.

3. La Pull Request è il momento del confronto tra le modifiche fatte su di una branch e il lavoro iniziale. Quando hai finito il lavoro sul tuo branch e vuoi riportarlo nel tronco principale, apri una PR.
4. Ecco una guida rapida per orientarti nel mondo di Git (e del controllo versione), spiegata in modo semplice.

5. Cos’è un Branch?
   Immagina il tuo progetto come un albero. Il tronco principale (chiamato solitamente main o master) rappresenta la versione ufficiale e funzionante del codice.

Un branch (ramo) è una linea temporale parallela. Quando crei un branch, stai facendo una copia esatta del progetto in quel momento per lavorarci sopra senza toccare il "tronco" principale.

Shutterstock
Esplora

2. Perché è utile?
   Senza i branch, ogni modifica finirebbe subito nel codice principale. Usarli è fondamentale perché:

Isolamento: Puoi lavorare su una nuova funzione (feature) o correggere un bug senza rischiare di rompere la versione del software che i tuoi utenti stanno usando.

Sperimentazione: Puoi provare idee folli: se non funzionano, cancelli il branch e il progetto principale resta intatto.

Collaborazione: Più persone possono lavorare a diverse parti dello stesso progetto contemporaneamente senza sovrascriversi a vicenda.

3. Cosa fa una Pull Request (PR)?
   La Pull Request è il momento del "confronto". Quando hai finito il lavoro sul tuo branch e vuoi riportarlo nel tronco principale, apri una PR.

Sostanzialmente, stai dicendo ai tuoi colleghi (o a te stesso): "Ho fatto queste modifiche, potreste controllarle? Se vanno bene, le uniamo al progetto principale".

È lo spazio dove avviene la Code Review (revisione del codice).

Si discute delle modifiche, si chiedono correzioni e si controlla che non ci siano errori.

4. Cosa significa fare Merge?
   Il merge (fusione) è la parte finale. Una volta che la Pull Request è stata approvata, i cambiamenti del tuo branch vengono "fusi" all'interno del branch principale. Facendo così il codice del tuo branch diventa parte integrante del tronco principale.

Conflitti: A volte capita che due persone modifichino la stessa riga di codice; in quel caso Git ti chiederà di risolvere il "confronto" manualmente prima di completare il merge.

In sintesi: crei un Branch per lavorare in sicurezza, usi la Pull Request per far revisionare il lavoro e alla fine fai il Merge per rendere le tue modifiche ufficiali.
