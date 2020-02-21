# Git Tutorial

Git is a version control system that is part of pretty much every modern development process. A version control system is a tool for tracking changes to your code. Think of it as the world's longest undo history: If you've ever broken a piece of your code and been unable to figure out how to go back to a working state, version control is what you've been looking for.

## Git Workflow

### Forking

After opening a repo, you'll click the **Fork** button to make a copy of the repo. **This step is very important;** you'll experience issues later on if you work directly from the original repo rather than your fork!!

![](https://user-images.githubusercontent.com/40476562/75009679-51201d80-541f-11ea-99e9-f85c198ea18c.png)

### Cloning

Clone down the code from your forked repo on github to your own computer using `git clone`. You'll use the URL provided by GitHub as shown:

![](https://user-images.githubusercontent.com/40476562/75010586-99403f80-5421-11ea-89cb-4d4d61a06070.png)

For example, if your repo is located at `https://github.com/your_username/usaf-git-tutorial.git`, you'd run `git clone https://github.com/your_username/usaf-git-tutorial.git` in your Terminal.

### The Revision Cycle

  * `git status` to see that you're starting from a clean state.
    * Make sure you're on the `master` branch. Unless you're using an intermediate strategy of creating feature branches, all your changes should be made on your fork's `master` branch.
  * Write the smallest possible change to your code that adds or improves something without breaking anything that used to work.
  * `git status` to see if you're right about which files have changed.
  * `git diff` to review your code, and verify that you're happy with all the things that have changed.
  * `git add` the files you want to commit (using paths from the `git status` command).
  * `git status` to verify that all and only the files you intended to add were added.
  * `git commit <file-name-here.md> -m <commit-message>` to commit your changes
  	* Note: Do not include the < >  
  * Write an informative commit message, describing what has been improved.
  * `git status` to verify that the commit went as you expected.
  * `git push origin master` to send your changes back up to the forked repo on your Github account.
  * Repeat this cycle until your code is in the shape you ultimately want it.

### Making Your First Commit

- [ ] In your local clone, open the file that corresponds to your name: `ash-coca.md`
- [ ] Answer the first question
- [ ] Commit your changes to your local clone of the repository
- [ ] Push your commit to GitHub
- [ ] Go to GitHub.com then to your repository to verify your commit `your-name.md`
- [ ] Repeat the above steps for remaining questions