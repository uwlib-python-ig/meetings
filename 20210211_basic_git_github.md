# MEETING NOTES

## Basic git and GitHub stuff

We spent some time working through getting set up to contribute to the [**lp3thw**](https://github.com/uw-libraries-python-interest-group/lp3thw) repository. I hope this information will be helpful to other folks without previous git and GitHub experience who are interested in sharing code with the PIG or contributing to other repositories.

As a reminder, if you are interested in contributing to the [**lp3thw**](https://github.com/uw-libraries-python-interest-group/lp3thw) repository, let me know [via email](mailto:ries07@uw.edu) and I'll send you an invite.

### Helpful software

* [**Git for Windows**](https://gitforwindows.org/) has many helpful features and makes _git_-ing very easy on Windows; you can use commands in Git for Windows' Git Bash to accomplish these basic  tasks

  **Clone and begin contributing to a repository**

  Today we walked through creating a local copy of a repository \(`git clone`\), pulling in changes to a local copy so that everything is up-to-date before doing work \(`git pull`\), and adding, committing, and pushing changes to the remote repository \(`git status`, `git add`, `git commit`, `git push`\).

* A note on the example commands below: When entering the commands shown here, don't enter the "$"; this is simply used to indicate the prompt where commands are entered, which may appear differently for you
* My prompt, for example, looks like this:

![A command prompt](https://i.imgur.com/ddcqdqY.png)

#### Create a local copy \("clone"\) of a remote repository

* Open a command-line interface \(CLI\) in the directory where you want to place your local copy
  * A nice feature of [Git for Windows](https://gitforwindows.org/) is the ability to right-click on a directory and open a Git Bash CLI there

![Right-click to open Git Bash in a directory](https://i.imgur.com/rrX3DGX.png)

* Copy a URL to clone the repository

![Viewing a GitHub repository in a browser](https://i.imgur.com/cM0H5Fc.png) ![Copy the URL](https://i.imgur.com/VkUJHzq.png)

* Clone the repository
  * Note that `CTRL+V` most likely won't work in your CLI, you'll need to right-click and paste

    ```text
    $ git clone <copied url>
    ```
* You now have a local copy of all files in the repository; you can open these folders using File Explorer, add files of your own \(see [the note below re: file-naming conventions](2021_02_11.md#Another-git-note)\), edit your files, etc.

#### Save and share your work

* Before starting work, pull any changes that have been made in the remote copy into your local copy
  * As when using the `git clone` command above, you'll need to open the CLI at the location you want the command to run; in this case you'll need to be in the local copy's directory

![Opening a CLI within the local copy](https://i.imgur.com/IpQIaIr.png)

* You can use the `git pull` command to bring any changes which have taken place in the remote repository into your local copy before starting work.

  ```text
  $ git pull
  ```

* Once you've added or made changes to a file, there are a few steps needed to push these changes to the remote repository
  * Again, you'll need to be "in" the local-copy directory in the CLI when you execute these commands
* Save any work to local files
  * If you don't save your work \("Save" in whatever text editor or other tool you've been using to write or edit code\), you can't push it to the remote repository!
* Take a look at what you've done
  * The `git status` command will give you an idea of what you've changed in your repository since you last committed \(we'll get to committing below\)

    ```text
    $ git status
    ```

    ![git status command results](https://i.imgur.com/h6TQJaM.png)
* Add your changes
  * Let git know which new work and/or changes you'd like to "commit" \(and eventually push to the remote repository\) using the `git add` command
  * You may use `git add` to add a specific file; for example to add my work from the screen capture above I could enter `git add ex42/bmr_ex42.py`
  * If you'd like to add all the changes you made at once, you can use `git add --all`
  * You can take _another_ look with `git status` to confirm  you've added the changes you wanted

    ```text
    $ git add <use filepath or '--all'>
    ```

![Using the git add command](https://i.imgur.com/kTfjigA.png)

* Now that you've told git what changes you want to push to the remote, _**commit to it**_!
  * Using `git commit` makes your changes "official," so to speak
  * Use `git commit` with the `-m` option; this will allow you to enter a brief message about the new code or changes you will be sending to the remote repository

```text
$ git commit -m "I added a comment to my code"
```

![A commit with a message](https://i.imgur.com/sbyhhqa.png)

* "Push" your changes to the remote repository

  ```text
  $ git push
  ```

  ![Using the git push command](https://i.imgur.com/JnuStDV.png)

### Another git note

This is a very simplified workflow for syncronizing with and pushing changes to a remote GitHub repository. There are many different ways to accomplish the tasks here, many potential situations which would require a different approach than that shown here, etc.

_**Not to worry!**_ Because all contributors are [encouraged to add their initials to the files they contribute](https://github.com/uw-libraries-python-interest-group/lp3thw#naming-and-storing-files), the chances for complications when contributing to [**lp3thw**](https://github.com/uw-libraries-python-interest-group/lp3thw) are fairly low. This naming convention should greatly reduce the risk of situations which might require more complex git solutions.

If you would like to learn more about using git, there are many great resources out there, and web searches along the lines of `"how to do [something] on the git command line?"` yield answers. Also, the [Pro Git Book](https://git-scm.com/book/en/v2) is freely available online, is exhaustive, and actually does include some relatively simple material on basic git work.

**tags: UWL-PIG**

