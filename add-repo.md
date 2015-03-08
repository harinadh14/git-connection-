Add A GitHub Repository To Your Local Machine
=============================================

####In your favorite web browser
1. Go to your profile on github.com
1. Click on "Repositories"
1. Click "New" towards the top-right of the screen
1. Give your repository a name. Avoid spaces and silly characters
1. Give your repository a description. Be as descriptive as you can, explain the purpose of the repository 
1. Set your repository to "public" or "private," I suggest public unless required to keep with the spirit of GitHub
1. Check the "Initialize this repository with a README" box unless you have already run `git init` in a directory via Terminal
1. If you know you want to ignore a specific code language, select it in the "Add .gitignore" dropbox, we can add specific folders and files to this later on
1. Give your repository a usage license. I suggest looking at [this site](http://choosealicense.com/ "Choose A License"); I prefer the MIT license
1. Click, "Create repository"
1. On this new page (URL should be github.com/username/repo-name) find the SSH clone URL in the right menu and click the "Copy to clipboard" button. If it says "HTTPS clone URL" above the input box, click on the blue "SSH" link below, this will change the clone URL to use SSH instead of HTTPS, and then click on the "Copy to clipboard" button

####In Terminal
1. Move to the parent directory where you would like to clone your new GitHub repository. You will use a "/" to move deeper into your folder structure. If you have spaces in your folder names you will have to put a "\" before them, like so: `cd ~/School/HCC/Spring\ 2015/ART229/Projects`. Note: It's quicker, easier, and less confusing if you can avoid using spaces in your directory names as much as possible (but not always possible)
1. Clone your GitHub repository to a new directory. There are two main ways to do this:
    - Create the new project repository as you are cloning your repository.
        - Run `git clone git@github.com:username/project-name.git new-project-name` you can paste your SSH clone URL in to replace the "git@github.com..." business and avoid any typo errors. You can also leave off the "new-directory-name" in which case your new directory's name will be the same as your GitHub repository's name when you created it. When (if) you designate your new directory's name in the clone command, you can use the same "\" character to add a space to name, e.g. `git clone git@github.com:username/project-name.git New\ Project\ Name` 
        - Note: If you get an error message about your directory already being a GitHub repository, you can change the remote URL by running `git remote set-url origin git@github.com:username/project-name.git`. This will change which remote repository your local machine points to when running git pull and git push. Avoid this if you can when just starting off
    - Create a new directory where we can clone our GitHub repository into *before* cloning. 
        - Create the new directory in your parent folder. You can use the same "\" character before any spaces in your folder name, like so `mkdir Project\ 1-Profile\ Page`
        - Move into your new directory, `cd Project\ 1-Profile\ Page`
        - Run `git clone git@github.com:username/project-name.git .` and DO NOT forget the "." at the end. That "." represents the current directory (the one we just made and moved into), which tells GitHub to clone our repository into the directory that we're currently in
1. Open your repository in your favorite text editor `open -a "Atom" .` (note the "." again) and get to work!