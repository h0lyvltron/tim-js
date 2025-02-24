# My JavaScript Project

This is a simple JavaScript project to learn Git and JavaScript. It will include rudimentary explanation and instruction for someone new to Git, GitHub, and development in general. Everything is being documented in this manner to solidify my understanding as I teach myself and learn.

## Getting Started

1. __Clone the repository__:
   ```sh
   git clone https://github.com/h0lyvltron/tim-js.git
   ```
1. __Create a new repository on GitHub__:
   * Go to GitHub and log in.
   * Click the "+" icon in the top right corner and select "New repository".
   * Name your repository (e.g., tim-js), add a description if you like, and click "Create repository".

1. __Initialize the local repository__:
   ```sh
   cd /c/repos/tim-js
   ```
   * Since git is directory based, you have to be in the root directory of the repository so all files/subdirectories can be contained and everything can be version controlled correctly
   ```sh
   git init
   ```
   * Initializes a new repository in your current directory; this creates a `.git` directory that contains all the necessary files for version control
   ```sh
   git add .
   ```
   * Adds all the files in the current directory to the staging area; the `.` indicates that _all files_ should be added
   ```sh
   git commit -m "initial commit"
   ```
   * Commits the files in the staging area to the repository with a message; the `-m` flag allows you to specify a commit message inline
1. __Add the remote repository__: Replace `your-username` with your GitHub username in the following command:
   ```sh
   git remote add origin https://github.com/your-username/tim-js.git
   ```
   * Adds a remote repository URL to your local repository; the name `origin` is a convention for the remote repository name
1. __Push your local repository to GitHub__:
   ```sh
   git push -u origin main
   ```
   * Pushes committed changes up to the repository; `origin` is a name for the remote repository, and `main` is the branch name
   * After using the `-u` flag and targeting origin/main, future `git push` commands will not need to specify the repo name and branch
