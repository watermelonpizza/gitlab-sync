# How to use
1. Ensure the project is set to 'git clone' mode. Because this uses gits --mirror system gitlab needs to cleanly clone the repo instead of just pulling the latest. 
    * Go to 'CI/CD Pipelines' settings and change to the mode to git clone
2. Set the project (environment) variables: `GITHUB_TOKEN` and `GIT_REPO`. 
    * You will need to get a token from github to use as the authentication. (You could set up ssl if you know what you are doing, the token is the easiest).
    * Go to [The github tokens page](https://github.com/settings/tokens) to generate a new one and set `GITHUB_TOKEN` as the token
    * Set the `GIT_REPO` as your repo id. Basically the <username>/<reponame> part of the url to your repo. E.g. `watermelonpizza/gitlab-sync`
3. And that's it! Ensure you have the gitlab and github repo setup (you must create both for this to work. It doesn't create one for you.)