## Git Workflow

### Writing Commit Messages

#### Anatomy of a good commit message:

```
Commit subject (summary) in 50 characters or less

More detailed explanation, manually wrapping
lines. Use a blank line to separate the top line
from the body so that GitHub can identify your
subject line.

Separate paragraphs with blank lines.

  * Bullet points work too!
  * Use two spaces for indentation

If you're completing a Trello card, also include
its link (it's okay if this doesn't wrap):

https://trello.com/c/...

```

#### Do:
* Capitalize your commit subject
* Separate commit subject from the body with a blank line
* Use imperative mood: "Fix bug" as opposed to "Fixed bug"

#### Don't:
* End your commit subject with a period
* Use `-m`

#### Rule of Thumb for Subject Lines:

A properly formed Git commit subject will complete the following sentence:

_If applied, this commit will **your subject line here**_.

For example:

* If applied, this commit will **merge pull request #123 from user/patch-1**
* If applied, this commit will **remove deprecated methods from socket library**

#### Formatting Commit Messages with Vim

If you're using `vim` to write your commit messages, you can add the following to your `~/.vimrc` to add spell checking and automatic line wrapping to your commits.

```shell
autocmd Filetype gitcommit setlocal spell textwidth=72
```

If you'd like to start using `vim` to edit your commits, you can enter the following into Terminal to make `vim` your default Git editor.

```shell
git config --global core.editor "vim"
```
