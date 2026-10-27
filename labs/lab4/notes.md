# Lab 4: Git & GitHub — Answers

## Question 1: What does `--global` mean?

The `--global` option saves my Git name and email in my user-wide Git configuration, so they apply to all my repositories by default. Without it, the configuration would normally apply only to the current repository if I run the command inside one.

## Question 2: What appeared in `ls -a`?

The `.git` directory appeared in `ls -a` but not in ordinary `ls` because it is hidden. It stores Git's repository information, including commit history, configuration, and other data needed to track changes.

## Question 3: How many files were offered for tracking?

Git listed the files and folders in the repository that were not being tracked. The exact number depends on the output shown when I ran git status.

## Question 4: What disappeared after creating `.gitignore`?

After creating `.gitignore`, files inside `.venv/`, Python cache directories such as `__pycache__/`, compiled `.pyc` files, and `.DS_Store` were ignored by Git. This keeps unnecessary generated files and local environment data out of the repository.

## Question 5: Should `.gitignore` be committed?

Yes, `.gitignore` should be committed because it tells Git which files to ignore. Sharing it ensures that other contributors follow the same rules when working on the repository.

## Question 6: What happened when `README.md` was staged?

`README.md` moved from the untracked-files section to the changes-to-be-committed section in `git status`. This means `git add README.md` copied its current contents into Git's staging area, ready for the next commit.

## Question 7: What did Git print after the commit?

After the commit, Git displayed the branch name, the short commit hash, your commit message, and a summary line showing the number of files changed along with any insertions or deletions (for example: `1 file changed, 1 insertion(+)`).

## Question 8: What are the first seven characters of a commit called?

The first seven characters are an abbreviated commit hash, a shortened representation of the commit's unique identifier. They help identify and refer to a particular version of the repository.

## Question 9: What are the four steps of the Git loop?

The four steps are edit, stage, commit, and repeat. I modify files, use `git add` to stage changes, use `git commit` to save a snapshot, and repeat whenever I make further changes.

## Question 10: Why is the file called `README.md`?

`README.md` is a conventional repository introduction that GitHub automatically displays on the repository's front page. The `.md` extension indicates Markdown formatting, allowing headings, lists, and other formatted text.

## Question 11: What does `gh auth login` do?

`gh auth login` authenticates GitHub CLI on my computer with my GitHub account. This saves the authentication credentials needed for authorized operations, such as pushing to a repository, without requiring me to enter my account password for every push.

## Question 12: What appears on the GitHub repository's front page?

The repository's `README.md` is displayed as formatted text on the front page. GitHub automatically renders it because README files are intended to introduce a repository and explain its contents.

## Question 13: Does pushing change local history?

No, pushing does not rewrite my local commit history. It uploads local commits to the remote repository so that GitHub can contain the same commits.

## Question 14: Private repository versus no repository

A private repository exists on GitHub but can only be accessed by its owner and authorized collaborators. If no repository exists on GitHub, there is no remote repository there for collaborators to access or review.
