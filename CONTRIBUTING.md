# CONTRIBUTING

The following guide will give you a brief explanation of how collaborating on GitHub typically works.

## Prerequisites

In order to collaborate on this project, you'll need [Git](https://git-scm.com/) and/or [GitHub Desktop](https://desktop.github.com/). (I say "and/or" as GitHub Desktop more than likely will install Git for you.)

If you go the Git route, you'll be entering commands via a command prompt/terminal whereas GitHub Desktop is a GUI alternative.

This guide will explain the Git route as that's what I'm most familiar with, but you should be able to figure out how to do many of the same things using GitHub Desktop.

## Getting ready for your first contribution

If it's your first time working on a project, you'll first need to clone the repository onto your local machine so that you can work on it.

This can be done in one of two ways (it doesn't matter which way you choose). Just open a command prompt or terminal wherever you want the project to be on your local machine and enter one of the following commands:

```bash
git clone git@github.com:IcePanorama/VRDungeonCrawler.git
```

or

```bash
git clone https://github.com/IcePanorama/VRDungeonCrawler.git
```

If all goes well, you should see something like:

```bash
Cloning into 'VRDungeonCrawler'...
remote: Enumerating objects: 19, done.
remote: Counting objects: 100% (19/19), done.
remote: Compressing objects: 100% (12/12), done.
remote: Total 19 (delta 6), reused 17 (delta 4), pack-reused 0
Receiving objects: 100% (19/19), done.
Resolving deltas: 100% (6/6), done.
```

Now simply type `cd VRDungeonCrawler` and you're ready to start working.

## Creating contributions

Creating contributions to any project on GitHub usually follows this sequence:

* [We pull the main branch](#pulling-the-main-branch),
* [We create a new branch for our contributions](#creating-a-new-branch),
* [We make whatever changes we need to make](#tracking-changes),
* Finally, [we submit a "Pull Request" to have our changes applied to the main branch of the project](#submitting-a-pull-request).

Let's go step by step in more detail.

For the sake of explanation, we're going to imagine that you want to add a feature to the project where the player can pick up coins.

### Pulling the main branch

We don't want to make changes to the project without first ensuring that our local copy of the repo is the latest possible verision of the repo available.

This can be accomplished in a single command: ``git pull origin main``.

### Creating a new branch

Our main branch (hopefully) works fine! We don't want to potentially mess up our main branch by making changes directly to it.

In order to prevent such a thing from happening, we're going to create a new branch where we can make our changes.

```bash
git checkout -b coin-pickups
```

We now have a brand new branch called coin-pickups!

The `git checkout -b` part is what's really important here. You can name your new branch whatever you like, although it's considered best practice to give the branch a good, descriptive name.

### Tracking changes

As you work on whatever feature/bugfix you're working on, you can track changes with the following two commands:

```bash
git add . # Adds all edited files to your next commit
# Alternatively,
git add example_file.exe # if you only want to commit changes to a specific file

git commit -m "Foo bar" # Make your message descriptive, e.g. "imported coin model"
```
It's considered best practice to make your commits as small as possbile.

An example of a bad commit would be: "Added coin model, added collision shape to coin, did some other stuff".

Commits ideally should do one thing (i.e., "Added coin model" and "added collision shape to coin" should ideally be separate commits). This makes it easier for us to revert back to older versions of our project if issues arise.

Secondly, "did some other stuff" is incredibly vague. Be specific. 

If you made a lot of tiny changes to a file, something like "Refactored file.txt" is a better alternative.

### Submitting a Pull Request

Once all your work is done, run the following command to push your changes to GitHub:

```bash
git push origin coin-pickups
```

Next, open up GitHub in your browser. Navigate to the VRDungeonCrawler repository, and look for the message which reads, "Your recently pushed branches:".

Below that, you should see a button which says "Compare & pull request". Click on that button.

On the next page, write a comment describing what you did in the comment box.

Finally, scroll down to the bottom of the page and hit "Create pull request".

At this stage, your changes have officially been pushed to GitHub, but they haven't yet been applied to our main branch. First, someone (probably me) should to check your code for potential conflicts.

Congratulations, you've made your first contribution on GitHub!

### Video explanation

Sometimes seeing this process done is easier to follow than just reading what I've written here. [I'd recommend this video if you'd like to see how the process is done for yourself](https://youtu.be/MnUd31TvBoU).
