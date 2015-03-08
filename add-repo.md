Add A GitHub Repository To Your Local Machine
=============================================

####In your favorite web browser
1. Go to your profile on github.com
2. Click on "Repositories"
3. Click "New" towards the top-right of the screen
4. Give your repository a name (no spaces or silly characters)
5. Give your repository a description. Be as descriptive as you can, explain the purpose of the repository 
6. Set your repository to "public" or "private," I suggest public unless required to keep with the spirit of GitHub
7. Check the "Initialize this repository with a README" box unless you have already run `git init` in a directory via Terminal
8. If you know you want to ignore a specific code language, select it in the "Add .gitignore" dropbox, we can add specific folders and files to this later on
9. Give your repository a usage license. I suggest looking at [this site](http://choosealicense.com/ "Choose A License"); I prefer the MIT license
10. Click, "Create repository"
11. On this new page (URL should be github.com/username/repo-name) find the SSH clone URL in the right menu and click the "Copy to clipboard" button. If it says "HTTPS clone URL" above the input box, click on the blue "SSH" link below, this will change the clone URL to use SSH instead of HTTPS, and then click on the "Copy to clipboard" button

####In Terminal
12. Move to the parent directory where you would like to clone your new GitHub repository. You will use a "/" to move deeper into your folder structure. If you have spaces in your folder names you will have to put a "\" before them, like so: `cd ~/School/HCC/Spring\ 2015/ART229/Projects`. Note: It's quicker, easier, and less confusing if you can avoid using spaces in your directory names as much as possible.
13. Create a new directory where we can clone our GitHub repository into. You can use the same "\" character before any spaces in your folder name, like so `mk-dir Project\ 1-Profile\ Page`
14. Move into your new directory, `cd Project\ 1-Profile\ Page`
15. Clone your GitHub repository to your new directory, `git clone git@github.com:username/project-name.git` you can paste your SSH clone URL in to replace the git@github.com... business and avoid any typo errors. 
16. If you get an error message about your directory already being a GitHub Repository you can change the remote url by running `git remote set-url origin git@github.com:username/project-name.git`. This will change which remote repository your local machine points to when running git pull and git push. Avoid this if you can when just starting off. 
17. 