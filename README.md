# Branching Policies

"I am [Angel Consola](https://github.com/DarkAvanger), student of the [Bachelor's Degree in Video Games by UPC at CITM](https://www.citm.upc.edu/ing/estudis/graus-videojocs/). This content is generated for the second year's subject Project 2.

# Concept

Branching Policies are rules that help to maintain control and improve the quality code of your project. These are made in order to help with organization and solve any structure related problem without much complexity. These policies are meant to work in parallel. Overall, the combination of an involved team and a good and structured Branching Policy help with the correct development of the projects.


To determine the advantages of Branching Policies we will work with the most common ones, which include Trunk-Based Development (This one is less used and outdated nowadays) and Feature Branching Development (This is the one currently being used by most companies).

# Why do we need Branching Policies?

Branching Policies are a must for organising a team, as it creates an easier workflow, it also provides clear instructions on how to manage all the work and commits made to the main branch. This prevents the main repository to get messed up, since the main branch is not directly manipulated by the team, but instead by the administrator of the repository, meaning that the main branch is protected against any issues that may come up.

The only user with permission to allow merge and pull requests is the administrator, meaning that the administrator has the main responsability of that repository. There could be more than one administrator, which they could be a Lead Programmer and a QA Lead, each of them will administrate different pulls and merges, as they are in charge of different aspects of the same project. Everything mentioned above can and should be managed on the Github website.

The non-administrators of the project will need to develop and create their own feature branches, then they will have to merge it with the main branch (Creating a pull request). With this method we can avoid damaging the main branch while keeping a good workflow between team members, as each of them is able to modify the code on it's own without disrupting other coworker's work.

# Trunk-Based Development

Trunk-Based Development is based on a single branch were all the teamm¡ works in the same branch, while having a different branch for releases. This also comes with a couple drawbacks, as if someone uploads the wrong code or anything is messed up the entire team needs to wait until the issue is solved, this process can slow down a project. This Policy has been outdated and it is barely used, Featire Branching Development has taken the advantatge as it is more efficient. 

![](https://github.com/DarkAvanger/BranchingPolicies/blob/main/Images/TrunkBasedDev.png)

# Feature Branching Development

Feature Branching Development is completely opposite to Trunk Based Development, this is mainly because all the implementations happen outside of the main branch and they only get implemented after the task is completed, therefore it provides a more efficient workspace while avoiding the drawbacks Trunk Based Development has. Even thought this Policy is not perfect either, and has some drawbacks. For example, if a branch does not stay updated with the main branch this will end up causing issues when implementing it in the main branch.

Git Flow is an example of a Feature Branching Policy.

![](https://github.com/DarkAvanger/BranchingPolicies/blob/main/Images/GitFlow.png)

# Git Flow Structure

Gitflow structure is divided into two main branches. The Master Branch and The Develop Branch, these branches are the only ones that remain until the end of the project.

![](https://github.com/DarkAvanger/BranchingPolicies/blob/main/Images/GitflowB.png)

## Master and Develop

The Master Branch only contains the main version of the project.

![](https://github.com/DarkAvanger/BranchingPolicies/blob/main/Images/MainBranches.png)

## Feature

The Develop Branch which contains the development progress of the project.

![](https://github.com/DarkAvanger/BranchingPolicies/blob/main/Images/FeatureBranch.png)

## Release

 The Release branches off the Develop branch and it must merge back into that branch or the Master Branch.
 
 This branch supports fixing errors, number of releases, versions and everything related to the master branch.
 
 ![](https://github.com/DarkAvanger/BranchingPolicies/blob/main/Images/ReleaseBranch.png)

## Hotfix

Branches off the Master branch, merges back into Develop and Master branch.

Hotfix branches are unplanned fixes, which include bugs. These branches are a must as they solve the undesired state of a Master branch. It is important when critical errors happen, as a new hotfix branch must be created and the issue must be solved immediatly. While a hotfix branch is created it does not stop production and other team members can continue with their respective development schedule.

![](https://github.com/DarkAvanger/BranchingPolicies/blob/main/Images/HotfixBranches.png)

# App Veyor

This is an app that can be connected to your Github account, it will generate a build for each commit that is made in the repository. We can configure Appveyor to create the builds for specific branches such as develop, release, master and hotfix. This will make the QA team easier to manage their work.

![](https://github.com/DarkAvanger/BranchingPolicies/blob/main/Images/Appveyor.png)

# Sources

- [Azure Branching Policies](https://docs.microsoft.com/en-us/azure/devops/repos/git/branch-policies?view=azure-devops&tabs=browser)
- [Azure Pull Request](https://docs.microsoft.com/en-us/azure/devops/repos/git/pull-requests?view=azure-devops&tabs=browser#complete-the-pull-request)
- [Git Hub Branches and Merges](https://docs.github.com/en/repositories/configuring-branches-and-merges-in-your-repository/defining-the-mergeability-of-pull-requests/about-protected-branches)
- [Azure DevOps Video](https://www.youtube.com/watch?v=2nukM2TzD1Q)
- [dev.to](https://dev.to/evdbogaard/branch-policies-in-azure-repos-11c5)
- [git-scm](https://git-scm.com/book/en/v2/Git-Branching-Branching-Workflows)
