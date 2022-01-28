# Version Control

Version control is essential when collaborating on a software project.
Developers may be working on functionality within the same page or must
make changes that affect each other. Version control systems, like Git,
ensure projects can be run efficiently.

Version control is a way of tracking changes that are made to code. The
most popular version control system is Git: [more info on version
control and
Git](https://serengetitech.com/tech/introduction-to-git-and-types-of-version-control-systems/).

## Why Use Version Control?

-   Complete history of code so that any new breaking changes to
    codebase can be reverted.

-   Simplifies collaboration, everyone has access to the latest version
    of the codebase.

-   Improved transparency, code attributed to author.

-   Collaboration, branches can be created to work on a feature without
    holding up the team.

## Introduction to Git

Git is a distributed version control system. This means that every
developer has a full copy of the repository and its history. Many
distributed version control tools use Git - amongst the most popular are
GitHub and BitBucket. We recommend teams use GitHub for their source
control.

### Git Terms

To familiarise you with Git, below are some words you will hear repeated
often:
<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0pky{border-color:inherit;text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0pky">Term</th>
    <th class="tg-0pky">Definition</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0pky">   <br>Repository   </td>
    <td class="tg-0pky">   <br>Project folder which stores the project history   </td>
  </tr>
  <tr>
    <td class="tg-0pky">   <br>Remote repository   </td>
    <td class="tg-0pky">   <br>Version of project hosted on internet (GitHub)   </td>
  </tr>
  <tr>
    <td class="tg-0pky">   <br>Local repository   </td>
    <td class="tg-0pky">   <br>Version of project on your machine. Changes made here are not visible by   teammates unless pushed to the remote repository   </td>
  </tr>
  <tr>
    <td class="tg-0pky">   <br>Branch   </td>
    <td class="tg-0pky">   <br>A separate branch from the repository that can be used to make changes   independent of other branches (main)   </td>
  </tr>
  <tr>
    <td class="tg-0pky">   <br>Main branch   </td>
    <td class="tg-0pky">   <br>The default branch for your repository   </td>
  </tr>
</tbody>
</table>

### Git Actions

These are the most common actions you are likely to perform using git:

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-7zrl{text-align:left;vertical-align:bottom}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-7zrl">&nbsp;&nbsp;&nbsp;&nbsp;<br><span style="color:black">Term</span>&nbsp;&nbsp;&nbsp;&nbsp;</th>
    <th class="tg-7zrl">&nbsp;&nbsp;&nbsp;&nbsp;<br><span style="color:black">Definition</span>&nbsp;&nbsp;&nbsp;&nbsp;</th>
    <th class="tg-7zrl">&nbsp;&nbsp;&nbsp;&nbsp;<br><span style="color:black">Command</span>&nbsp;&nbsp;&nbsp;&nbsp;</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Clone</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Makes a local copy of a repository</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">git clone [repo]</span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Add</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Marks file as staged, such that is added in the next commit</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">git add [filename]</span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Commit</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Snapshot of repo, with several changes to the codebase</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">git commit -m "commit&nbsp;&nbsp;&nbsp;message"</span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Push</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Pushes changes (commits) to the remote repository</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">git push</span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Pull</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Pulls any changes from the latest version of the remote repository and&nbsp;&nbsp;&nbsp;integrates any file changes with your local branch</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">git pull [remote] [branch]</span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Fetch</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Pulls changes from the latest version of the remote repository but does&nbsp;&nbsp;&nbsp;not change the files to match remote repository. Can be useful if you want to&nbsp;&nbsp;&nbsp;check whether a pull will override any of your local file changes</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">git fetch [remote] [branch]</span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
</tbody>
</table>

### Local File Changes

Changes made to files that live inside a repository can be one of
several statuses.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-7zrl{text-align:left;vertical-align:bottom}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-7zrl">&nbsp;&nbsp;&nbsp;&nbsp;<br><span style="color:black">Status</span>&nbsp;&nbsp;&nbsp;&nbsp;</th>
    <th class="tg-7zrl">&nbsp;&nbsp;&nbsp;&nbsp;<br><span style="color:black">Description</span>&nbsp;&nbsp;&nbsp;&nbsp;</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Untracked</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">The file is not being monitored by the version control (does not exist).</span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Unmodified</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">The local file matches exactly the files in the remote repository.</span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Modified</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">The local file differs from the file in the remote repository.</span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
  <tr>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Staged</span>&nbsp;&nbsp;&nbsp;</td>
    <td class="tg-0lax">&nbsp;&nbsp;&nbsp;<br><span style="color:black">Changes to the local file are ready to be pushed to the remote repository&nbsp;&nbsp;&nbsp;so the file in the remote repository matches exactly the file in the local&nbsp;&nbsp;&nbsp;repository.</span>&nbsp;&nbsp;&nbsp;</td>
  </tr>
</tbody>
</table>

![Diagram of file
status](./resources/media/image1.png)

### Branching

Git branches are effectively pointers to your self-contained changes.
When you, as a developer, want to make changes to the code of a project
in a remote repository (no matter how big or small the change is), you
will create a branch to encapsulate all your changes. That branch is
entirely self-contained and is not a part of the remote repository's
code. This stops potentially unstable code from being committed to the
repository before it can be thoroughly tested and properly merged.

To learn more about branching, please refer
[here](https://www.atlassian.com/git/tutorials/using-branches).

To learn the basics of branching in a fun way, check out this
[interactive tool to learn git
branching](https://learngitbranching.js.org/). This tool is great for
beginners or people who need a refresher.

### Example Git Workflow

*Bringing everything we have discussed together*.

Once you have cloned (downloaded the most recent copy of the codebase)
from GitHub. You have what is called a *local copy* of the repository.

Then, any changes you make within your working directory (copy of the
repository on your machine) is said to be untracked. This means Git does
not know about the file and its changes.

To ensure git tracks the file and its history, you need to add the file
using the command git add \[filename\].

Once a file is tracked, its changes fall under two categories: staged or
unstaged. For unstaged changes, Git has not marked the file to be a part
of the subsequent commit. Staged changes refer to files with changes
that are to be added to the next commit. When making a change that you
want to be added to the remote copy of the repository, you need to make
sure the changes are staged. This can be done by using the command git
add \[filename\].

When all your changes are staged, then you want to commit those changes.
A commit is a snapshot/milestone with a series of changes. Commits can
be created with a message, using the following command: git commit -m
\"commit message\".

Once a commit is made, the file goes back to the unmodified state as the
local repository updates the current branch's history with the latest
changes. To ensure the remote repository is also updated, such that
everyone in the team can see the changes made, you need to push the
changes to the remote repository. This can be done by running git push.

Another developer who may want to see your changes, can pull changes by
running the command git pull \[remote\] \[branch\]. This will fetch the
latest changes from the remote repository and integrate them with their
local files.

Extra Resources

1.  [Git explained in 100
    seconds](https://www.youtube.com/watch?v=hwP7WQkmECE&ab_channel=Fireship)

2.  [GitKraken](https://www.gitkraken.com): A great GUI that sits on
    top of Git's command line integration to provide a more
    user-friendly way of interacting with version control
    systems.

What's Next

This was a very general introduction to Git. Throughout this semester,
you will be making use of GitHub - to learn more about GitHub, please
see the next chapter focused primarily on GitHub.
