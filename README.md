#Gym Exercises

##Bundle 1
 
 ##Exercise 1

```bash
gymimbaraga@Imbaragas-iMac thegym-exercises % git status
On branch main
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
gymimbaraga@Imbaragas-iMac thegym-exercises % git branch -m main master
gymimbaraga@Imbaragas-iMac thegym-exercises % git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
gymimbaraga@Imbaragas-iMac thegym-exercises % git add --all   
gymimbaraga@Imbaragas-iMac thegym-exercises % git commit -m "First trial"
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
gymimbaraga@Imbaragas-iMac thegym-exercises % git push origin master
Everything up-to-date
gymimbaraga@Imbaragas-iMac thegym-exercises % git checkout -b dev
Switched to a new branch 'dev'
gymimbaraga@Imbaragas-iMac thegym-exercises % git checkout -b test
Switched to a new branch 'test'
gymimbaraga@Imbaragas-iMac thegym-exercises % git checkout dev
Switched to branch 'dev'
gymimbaraga@Imbaragas-iMac thegym-exercises % git branch -d test
Deleted branch test (was 53d8a09).
gymimbaraga@Imbaragas-iMac thegym-exercises % git status
On branch dev
nothing to commit, working tree clean
gymimbaraga@Imbaragas-iMac thegym-exercises % 
```

## Exercise 2

```bash
Imbaragas-iMac:thegym-exercises gymimbaraga$ git branch
  dev
* exercise-2-training
  master
Imbaragas-iMac:thegym-exercises gymimbaraga$ git checkout exercise-2-training
Already on 'exercise-2-training'
Imbaragas-iMac:thegym-exercises gymimbaraga$ touch about.html
Imbaragas-iMac:thegym-exercises gymimbaraga$ git add about.html
Imbaragas-iMac:thegym-exercises gymimbaraga$ git stash save "About file stash"
Saved working directory and index state On exercise-2-training: About file stash
Imbaragas-iMac:thegym-exercises gymimbaraga$ touch home.html
Imbaragas-iMac:thegym-exercises gymimbaraga$ git add home.html
Imbaragas-iMac:thegym-exercises gymimbaraga$ git stash save "Home file stash"
Saved working directory and index state On exercise-2-training: Home file stash
Imbaragas-iMac:thegym-exercises gymimbaraga$ touch team.html
Imbaragas-iMac:thegym-exercises gymimbaraga$ git add team.html
Imbaragas-iMac:thegym-exercises gymimbaraga$ git stash save "team.html"
Saved working directory and index state On exercise-2-training: team.html
Imbaragas-iMac:thegym-exercises gymimbaraga$ git status list
On branch exercise-2-training
nothing to commit, working tree clean
Imbaragas-iMac:thegym-exercises gymimbaraga$ git stash list
stash@{0}: On exercise-2-training: team.html
stash@{1}: On exercise-2-training: Home file stash
stash@{2}: On exercise-2-training: About file stash
Imbaragas-iMac:thegym-exercises gymimbaraga$ git stash pop stash@{2}
On branch exercise-2-training
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{2} (613a4f9b2e20a8a00c0b9cf2df8514a517aaf2a5)
Imbaragas-iMac:thegym-exercises gymimbaraga$ git stash pop stash@{1}
On branch exercise-2-training
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (2ff9659b1b1778671f1ba51af1bacbd665ed738e)
Imbaragas-iMac:thegym-exercises gymimbaraga$ git add .
Imbaragas-iMac:thegym-exercises gymimbaraga$ git commit -m "Restore about the About.html and Home.html"
[exercise-2-training 893d646] Restore about the About.html and Home.html
 2 files changed, 12 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
Imbaragas-iMac:thegym-exercises gymimbaraga$ git push origin exercise-2-training
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 568 bytes | 568.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'exercise-2-training' on GitHub by visiting:
remote:      https://github.com/Muhanguzi-boss/Gym-Bundle-Exercises/pull/new/exercise-2-training
remote: 
To https://github.com/Muhanguzi-boss/Gym-Bundle-Exercises.git
 * [new branch]      exercise-2-training -> exercise-2-training
Imbaragas-iMac:thegym-exercises gymimbaraga$ git stash pop stash@{0}
On branch exercise-2-training
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (04107987e3b719d946832f9848e23eec3740ac9b)
Imbaragas-iMac:thegym-exercises gymimbaraga$ git reset --hard HEAD
HEAD is now at 893d646 Restore about the About.html and Home.html
Imbaragas-iMac:thegym-exercises gymimbaraga$ git
``` 


# Bundle 2

## Exercise 1

```bash
gymimbaraga@Imbaragas-iMac thegym-exercises % git branch ft/bundle-2 
gymimbaraga@Imbaragas-iMac thegym-exercises % git checkout ft/bundle-2 
Switched to branch 'ft/bundle-2'
gymimbaraga@Imbaragas-iMac thegym-exercises % git status
On branch ft/bundle-2
nothing to commit, working tree clean
gymimbaraga@Imbaragas-iMac thegym-exercises % touch service.html
gymimbaraga@Imbaragas-iMac thegym-exercises % git add service.html
gymimbaraga@Imbaragas-iMac thegym-exercises % git commit -m "Add service.html page"
[ft/bundle-2 d56aa9b] Add service.html page
 1 file changed, 12 insertions(+)
 create mode 100644 service.html
gymimbaraga@Imbaragas-iMac thegym-exercises % git push origin ft/bundle-2 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 478 bytes | 478.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Muhanguzi-boss/Gym-Bundle-Exercises/pull/new/ft/bundle-2
remote: 
To https://github.com/Muhanguzi-boss/Gym-Bundle-Exercises.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
gymimbaraga@Imbaragas-iMac thegym-exercises % 
```