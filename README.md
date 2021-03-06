# Middleman template

Welcome on this short guide on how to quickstart your next Middleman project.

## Getting started

In your terminal, check you have Middleman:

```bash
gem install middleman
# You should have a version >= 4.2.1
```

Then run the following:

```bash
cd ~/code/YOUR_GITHUB_NICKNAME
middleman init YOUR_PROJECT -B -T poulpes/middleman-template
cd YOUR_PROJECT

git init
git add .
git commit -m 'Generated a new middleman project with poulpes/middleman-template'

hub create    # To create a repo on GitHub
git remote -v # Check that the `origin` remote is set.
git push origin master
```

You should be able to run:

```bash
middleman server
```

And go to [localhost:4567](http://localhost:4567)

## Deployment

Make sure that your `git status` is clean and run:

```bash
middleman deploy
```

This should build your Middleman project and push it to the `gh-pages` of your GitHub repository. Then go to `YOUR_GITHUB_NICKNAME.github.io/YOUR_PROJECT` to see it live 🚀 !
