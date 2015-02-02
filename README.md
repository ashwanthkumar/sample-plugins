# GoCD - Github Integration

WIP

This project should contain 2 projects.
1. Github PR matierial poller - This is a straightforward material poller that pools for any pull requests on the github repo and triggers a build pipeline
2. Github PR build task - Task plugin that does a checkout of the repo, merging the PR patch against the branch, builds the repo from 'gocd-build.conf' on the project root. It also replies back on the PR with the build status.

## Workflow
Suppose you already have a build pipeline for a repository 'github-project', you might want to create another pipeline that builds all the pull requests.
- Add a Github PR material (it takes a github url + branch)
- Add a build stage and job with 'Github PR Build' Task
- Send PR and watch the pipeline build
