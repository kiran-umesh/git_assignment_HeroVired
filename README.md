# git_assignment_HeroVired
Collaboration on Github assignment with Rama

**
****For Question 1 in the Assignment: ****
cloned the new repo to local:**

Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert
$ git clone https://github.com/kiran-umesh/git_assignment_HeroVired.git
Cloning into 'git_assignment_HeroVired'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.


**Created new branch "dev":**

Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (main)
$ git checkout -b dev
Switched to a new branch 'dev'


**Created the app file:**
Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (dev)
$ nano CalculatorPlus.py

**
**Added it for tracking****
Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (dev)
$ git add .
warning: in the working copy of 'CalculatorPlus.py', LF will be replaced by CRLF the next time Git touches it

**Committed the file for the first time**
Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (dev)
$ git commit -m "Initial commit of the Calc plus app on Dev"
[dev 557cee2] Initial commit of the Calc plus app on Dev
 1 file changed, 47 insertions(+)
 create mode 100644 CalculatorPlus.py

**Pushed it to remote repo:**
Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (dev)
$ git push origin dev
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 683 bytes | 683.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/kiran-umesh/git_assignment_HeroVired/pull/new/dev
remote:
To https://github.com/kiran-umesh/git_assignment_HeroVired.git
 * [new branch]      dev -> dev


**Switched to Main and merged the Dev branch to main:**
Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (dev)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (main)
$ git merge dev
Updating 81e0436..557cee2
Fast-forward
 CalculatorPlus.py | 47 +++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 47 insertions(+)
 create mode 100644 CalculatorPlus.py

Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (main)
$


**Pushed main to remote repo:**

Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (main)
$ git push origin main
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/kiran-umesh/git_assignment_HeroVired.git
   81e0436..557cee2  main -> main

**Created Release version 1.0**

**Created a new branch - feature/sqrt:**
Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (main)
$ git checkout -b feature/sqrt
Switched to a new branch 'feature/sqrt'

Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (feature/sqrt)


**Updated code to add sqrt functionality:**
Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (feature/sqrt)
$ nano CalculatorPlus.py
Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (feature/sqrt)
$ git status
On branch feature/sqrt
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   CalculatorPlus.py

no changes added to commit (use "git add" and/or "git commit -a")


**Committed changes in Feature branch before moving to Dev branch for working bug fix, to keep the branch clean and up-to-date:**
Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (feature/sqrt)
$ git commit -m "Adding sqrt code to the calc plus app in feature branch"
[feature/sqrt f859873] Adding sqrt code to the calc plus app in feature branch
 1 file changed, 5 insertions(+), 5 deletions(-)


**Updated file on Dev branch to add bug fix for division code:**
Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (dev)
$ nano CalculatorPlus.py
Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (dev)
$ git add CalculatorPlus.py

Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (dev)
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   CalculatorPlus.py



**Merged the feature code for sqrt onto Main branch by raising pull request and was approved by Ram495.**


**Committed the code for testing and pushed to remote:**
Kiran@Radha-Krishna-01 MINGW64 /d/DevOps_Cert/git_assignment_HeroVired (dev)
$ git commit -m "Added bug fix for Division code on Dev branch"
[dev 20e2b55] Added bug fix for Division code on Dev branch
 1 file changed, 4 insertions(+)

**Raised pull request to merge Feature code to Dev adding a reviewer**

![image](https://github.com/user-attachments/assets/a89d395e-582b-4cb5-8b2f-05f9c23c62e3)

****Merged the code post approval**

![image](https://github.com/user-attachments/assets/7df53505-7be5-4398-8738-9e2fdec5365b)

**Created a new release with V2.0****

![image](https://github.com/user-attachments/assets/e85f2805-0e5f-439e-9ba4-0bbea4bb18e2)
