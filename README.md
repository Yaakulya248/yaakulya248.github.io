*HEY! This is just a sample edit*

Here's the link for youtube.com [Youtube Link](https://www.youtube.com)

## Introduction (Testing done by Yaakulya)
Hello everyone, this is Yaakulya. I'm a freshman at NYUAD 

## Learning from stratch

#### Why Should I Use This?
This website will be ready soon

## [Getting Started Guide](https://ncsu-libraries.github.io/jekyll-academic-docs/)
Complete documentation for getting started as well as advanced features of Jekyll Academic can be found at [https://ncsu-libraries.github.io/jekyll-academic-docs/](https://ncsu-libraries.github.io/jekyll-academic-docs/).

## Migrating to a new default branch name
We've decided to change this project's default branch name to 'main'.  If you've forked this repository prior to July 20th, 2021, then you should a message with update instructions when you go to your fork in github: 

![fork renamed message](https://user-images.githubusercontent.com/3514165/126372022-ae4c07fa-dec7-427c-a4b5-cdd73aec75eb.png)

In your fork on GitHub, go to the branches view, and click on the edit icon next to the 'master' branch.  Change the branch name to main.  Underneath the input box where you change the name you will be presented with the commands that you will need to run on your local copy of your fork.

![local instructions for default branch name change ](https://user-images.githubusercontent.com/3514165/126372635-208fbc4b-698e-4938-bdae-5ff19eed2c96.png)


## Upgrade Notes for June 2021 release
If you are running a fork of Jekyll Academic before June 2021, we made some breaking changes to upgrade the underlying Jekyll version and to address the constant github/dependabot security notices mentioned in issue #4.

We have updated Jekyll to version 4 and removed reveal.js as an included library. We still want to support reveal.js presentations, so we have taken the suggestion from issue #4 and made the reveal.js directory a [git submodule](https://git-scm.com/book/en/v2/Git-Tools-Submodules). If you are running Jekyll Academic as a Github Page, this should hopefully be a minor change.

If, however, you are running Jekyll Academic locally or on a custom server, after merging this repo's commits in to your fork, you will need to go to the command line in your local or custom instance and perform the following command:

  `$ git submodule update --init`

If you have any reveal.js presentations posted, you may need to make some updates for them to display properly using reveal.js version 4.  See [Jekyll's documentation](https://revealjs.com/upgrading/) for details.

## Keeping reveal.js up to date
Moving forward, if you'd like to update reveal.js you will need to run the following commands:

  `$ git submodule update --remote`
