github-aur
==========
Maintain your AUR packages with GitHub and Travis CI.

With github-aur you can push your PKGBUILD (+ related files) into a GitHub repository.
Afterwards the continuous integration service Travis CI will check if your packages 
are OK and uploads them into the AUR.

```
How it works

          git push                                           checks
   0      PKGBUILD   +-----------+  forwards  +-----------+  uploads  +-----------+
 - | -   ----------> |  GitHub   | ---------> | Travis CI | --------> |    AUR    |
  / \                +-----------+            +-----------+           +-----------+
          ^
          |
          +--- This is the only thing you have to do to update your package 
               in the AUR! Travis-CI and this project will everything else.
```
