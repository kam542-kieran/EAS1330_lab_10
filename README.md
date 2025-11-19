# EAS1330_lab_10

# This is a title
## This is a subtitle
*This text is italicized*
**This text is bold**

# added readme file
This is a README file that I'm editing on my computer

1. Created a new repo on github
2. Copied SSH URL from github
   - Click "code" button on github
   - Copy SSH URL
4. Navigated to home directory on terminal
   - cd ~
5. Configured git on computer by identifying self with name and email
   - git config --global user.name "name"
   - git config --global user.email "github_email"
6.  Generated SSH keys to allow communication between computer and github
   - ssh-keygen -t ed25519 -C "github_email"
7. Added new key to ssh agent and displayed the public key
   - eval "#(ssh-agent -s)"
   - ssh-add ~/ .ssh/id_ed25519
   - cat ~/ .ssh/id_ed25519.pub
8. Copied SSH key from terminal (ssh-ed25519 and following characters)
9. Added SSH key to github account
   - Navigated to SSH and GPG keys page on github
   - Cliked "New SSH key" and named it
   - Copied SSH key
10. Cloned repo from github to computer
   - git clone git@github.com: username/name_of_repo.git
11. Tested connection in terminal
   - cd ~/repo_name
   - ls
   - Should return README.md
12.  Made changes from terminal using a text editor (pico in this case)
   - pico README.md
   - {inserted desired text to add}
13. Saved work and exited
   - ctrl + O, enter, ctrl + x
14. Committed and pushed changes to github from terminal
   - git add README.md
   - git commit -m "message"
   - git push
15. Created python script on github
   - created new file on repo, named it, and committed changes
16. Accessed python script from terminal
   - git pull
   - python3 "script_name"

If there are problems with the local copy:
1. Go up one directory
   - cd ..
2. Delete the local repo
   - rm -rf "repo_name"
3. Make a new clone
   - git clone git@github.com:username/name_of_repo.git
     

