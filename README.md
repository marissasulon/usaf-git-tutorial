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
  * `git add` the files you want to commit (using paths from the `git status` command).
  * `git status` to verify that all and only the files you intended to add were added.
  * `git commit <file-name-here.md> -m "commit-message-here"` to commit your changes
  	* Note: Do not include the < > in the filename, DO include the quotes for the commit message!
  * Write an informative commit message, describing what has been improved.
  * `git status` to verify that the commit went as you expected.
  * `git push origin master` to send your changes back up to the forked repo on your Github account.
  * Repeat this cycle until your code is in the shape you ultimately want it.

### Making Your First Commit

- [ ] In your local clone, open the file that corresponds to your name: `your-name.md`
- [ ] Answer the first question
- [ ] Commit your changes to your local clone of the repository
- [ ] Push your commit to GitHub
- [ ] Go to GitHub.com then to your repository to verify your commit `your-name.md`
- [ ] Repeat the above steps for remaining questions

### Submitting Your First Pull Request

Once you've finished answering all the questions, it's time to merge your changes back to the master repository!

![](https://user-images.githubusercontent.com/40476562/75012045-3650a780-5425-11ea-9292-4ff9df348cec.png)

On the following page, review your changes then submit your first pull request!

![](https://user-images.githubusercontent.com/40476562/75012534-42893480-5426-11ea-8b30-fe06d8198f04.png)

If you run into any merge conflicts, flag down an instructor.

Good luck and happy coding!

## Advanced Content

Firstly, advanced content is 100% optional and not necessary to complete for your sprint to be considered finished. Advanced content is meant to be attempted only after you've finished all of the basics. It's designed to direct you down interesting paths and help you increase your autonomy, so challenge yourself to tackle these problems without extra guidance!

- [ ] Figure out how to make a new branch from your master branch
- [ ] Figure out how to push your new branch to your fork on github and then go to github and confirm that it worked!
- [ ] Play through [Terminus](http://web.mit.edu/mprat/Public/web/Terminus/Web/main.html) then add the `passwordToParadise` to the bottom of your file. Then commit and push up to GitHub.
