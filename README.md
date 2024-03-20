# Git Flow Workflow

Git flow is a popular Git branching strategy aimed at simplifying release management, and was introduced by software developer Vincent Driessen in 2010. Fundamentally, Git flow involves isolating your work into different types of Git branches.

**_In the Git flow workflow, there are five different branch types:_**

- `main`/`master`
- `develop`
- `feature`
- `release`
- `hotfix`

<p align="center">
    <img src="images/git_flow_workflow.png" alt="Git flow workflow" width="500"/>
</p>

## The `main`/`master` branch

The purpose of the `main` branch in the Git flow workflow is to contain production-ready code that can be released.

In Git flow, the `main` branch is created at the start of a project and is maintained throughout the development process. The branch can be tagged at various commits in order to signify different versions or releases of the code, and other branches will be merged into the `main` branch after they have been sufficiently vetted and tested.

<p align="center">
    <img src="images/main_branch.png" alt="The main/master branch" width="275"/>
</p>

## The `develop` branch

The `develop` branch is created at the start of a project and is maintained throughout the development process, and contains pre-production code with newly developed features that are in the process of being tested.

Newly-created features should be based off the `develop` branch, and then merged back in when ready for testing.

## The `feature` branch

The `feature` branch is the most common type of branch in the Git flow workflow. It is used when adding new features to your code.

When working on a new feature, you will start a `feature` branch off the `develop` branch, and then merge your changes back into the `develop` branch when the feature is completed and properly reviewed.

<p align="center">
    <img src="images/feature_branch.png" alt="The feature branch" width="120"/>
</p>

## The `hotfix` branch

In Git flow, the `hotfix` branch is used to quickly address necessary changes in your `main` branch.

The base of the `hotfix` branch should be your `main` branch and should be merged back into both the `main` and `develop` branches. Merging the changes from your `hotfix` branch back into the `develop` branch is critical to ensure the fix persists the next time the `main` branch is released.

<p align="center">
    <img src="images/hotfix_branch.png" alt="The hotfix branch" width="275"/>
</p>
