# gitIntro
A skeleton repo for learning how to use GitHub and git.

Some useful links:

- [A guide to licences](https://help.github.com/en/articles/licensing-a-repository) How do I want people to be able to use my repo?
- [Github tutorials](https://guides.github.com) Useful short guides on different aspects of using GitHub and git.
- [A glossary of git terms](https://git-scm.com/docs/gitglossary) For distinguishing your _staging_ from _pushing_ and your _forking_ from _cloning_.
- [Download git](https://git-scm.com/downloads) For issuing git via the command-line.
- [Git Book](https://git-scm.com/book/en/v2) For a detailed and comprehensive guide to using git.


## An Intoductory Exercise

### 1. Setting things up

- If you don't already have one, set up a free GitHub account by visiting [github.com](https://github.com) and clicking **Sign up for GitHub**.

- Ensure you have git running on your machine:

  To test, open a command prompt (Windows), terminal (MacOS) or shell (linux) and type:

  `git --help`

  If you see a page of help instructions you are good to go. If you receive a message like _git: command not found_ you will need to install git yourself:

  Visit [git-scm.com/downloads](https://git-scm.com/downloads) and follow the instructions for your platform. You can accept all the default options provided by the install program.

  Once installed, open a new command prompt/terminal/shell and check `git --help` works as expected.

### 2. Creating and editing your own repo

- Log in to GitHub and create a new public repo called `gitIntro`. Select the options to include a README file and choose an MIT licence (see [A guide to licences](https://help.github.com/en/articles/licensing-a-repository) for more on differences between licences).

- Still via the GitHub pages, edit your newly created README file (look for the pencil icon) to provide a welcoming message. _Remember, everything you edit/add here is public_.

### 3. Making a fork from someone else's repo

_This activity works best if you are completing it with someone else in order to see how to work together on a shared project. But if this is not practical, you can use this repo as the one you will fork._

- Open a new web page and open up one of your colleague's newly created repos (or this one). It should have the form `github.com/XXX/gitIntro` where `XXX` is their GitHub account name.

- _Fork_ a copy of their repo by clicking the 'fork' link. This will create a copy of their repo in your own 'remote' GitHub space.

- Point your browser to this newly forked copy in your own GitHub space and click the green `Clone or download` button. Copy the URL provided, which will be something like _git<span>@github</span>.com:myAccountName/gitIntro.git_.

### 4. Working with a local copy of a remote repo

- Open a command prompt/terminal/shell and `cd` to a place where you would like to store a local copy of the remote repo.

- In the command window, type `git clone XXX` where _XXX_ is the reference you have just copied (_git<span>@github</span>.com:myUsername/gitIntro.git_) and you can ctrl-v to paste it to the end of the line). This should download the repo from the remote location on GitHub and create a local copy of it on you computer. You can now make changes to this local copy that won't at this stage have any effect on the remote version sitting on GitHub.

- In your favourite editor create a new file called `myName.md` where _myName_ is your name without any spaces (e.g. `JoWood.md`). In this file, add some simple biographical details (that you are happy to be made public) and then save it.

### 5. Pushing local changes back to a remote repo

- From the command line, ensure you are in the folder containing your local copy of the forked repo and then type:

   `git add myName.md` (where _myName.<span>md</span>_ is the name of the file you have just created)
   
   `git commit --message "Add my details"`
   
   `git push`

   If you point a browser to your repo on GitHub and refresh the page, you should see your newly created file now listed as part of the repo.
   
 ### 6. Making a Pull Request (PR)

As a final step, you are going to make a request to the originator of the repo you forked asking them to incorporate the modifications you made to your version of it, back into their original version (If you have forked this repo, I will most likely reject PRs, but please feel free to make one in order to practice).

- With your browser pointing to your forked repo on GitHub, click the 'New Pull Request' button and give the PR a title such as “Add my bio details” and in the comment section add a rationale for your request, for example "I'd like to add my details to your repo so you can see my programming interests".

- Click the "Create Pull Request" button. This will send a message to the author of the repo you forked with the details of the changes you are requesting. It is now up to them to accept or reject your request!

- If a colleague completing this exercise has forked your original repo (hopefully they have), you will receive a notification from GitHub that a PR has been made. If you are happy with their addition (hopefully you will be), accept their PR. You should now have a repo jointly authored by you and any other colleagues who have forked your repo and submitted a PR to you.
