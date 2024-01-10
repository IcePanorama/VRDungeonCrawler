# CONTRIBUTING

The following guide will give you a brief explanation of how collaborating on GitHub typically works.

## Prerequisites

In order to collaborate on this project, you'll need [Git](https://git-scm.com/) and/or [GitHub Desktop](https://desktop.github.com/). (I say "and/or" as GitHub Desktop more than likely will install Git for you.)

If you go the Git route, you'll be entering commands via a command prompt/terminal whereas GitHub Desktop is a GUI alternative.

This guide will explain the Git route as that's what I'm most familiar with, but you should be able to figure out how to do many of the same things using GitHub Desktop.

## Getting ready for your first contribution

If it's your first time working on a project, you first need to clone the repository onto your local machine so that you can work on it.

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

Now simply `cd VRDungeonCrawler` and you're ready to start working.

## Creating contributions

Creating contributions to any project on GitHub usually follows this sequence: we pull the main branch to make sure we're up to date, we create a new branch for our contribution, we make whatever changes we need to make, and then we submit a "Pull Request" to have our changes applied to the main branch of the project.
