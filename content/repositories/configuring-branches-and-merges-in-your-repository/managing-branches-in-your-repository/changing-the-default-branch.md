---
title: Changing the default branch
intro: 'If you have more than one branch in your repository, you can configure any branch as the default branch.'
permissions: People with admin access for a repository can change the default branch for the repository.
versions:
  fpt: '*'
  ghes: '*'
  ghec: '*'
redirect_from:
  - /github/administering-a-repository/setting-the-default-branch
  - /articles/setting-the-default-branch
  - /github/administering-a-repository/changing-the-default-branch
  - /github/administering-a-repository/managing-branches-in-your-repository/changing-the-default-branch
topics:
  - Repositories
shortTitle: Change the default branch
---
## About changing the default branch

You can choose the default branch for a repository. The default branch is the base branch for pull requests and code commits. For more information about the default branch, see [AUTOTITLE](/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-branches#about-the-default-branch).

You can also rename the default branch. For more information, see [AUTOTITLE](/repositories/configuring-branches-and-merges-in-your-repository/managing-branches-in-your-repository/renaming-a-branch).

{% data reusables.branches.set-default-branch %}

## Prerequisites

To change the default branch, your repository must have more than one branch. For more information, see [AUTOTITLE](/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-and-deleting-branches-within-your-repository#creating-a-branch).

{% ifversion not fpt %}

Rulesets at the organization{% ifversion ghec %} or enterprise{% endif %} level that apply to branches of a repository will not allow the repository administrator to rename branches of the targeted repository or change the default branch to another branch. See [AUTOTITLE](/organizations/managing-organization-settings/managing-rulesets-for-repositories-in-your-organization){% ifversion ghec %} or [AUTOTITLE](/admin/enforcing-policies/enforcing-policies-for-your-enterprise/enforcing-policies-for-code-governance){% endif %}.

{% endif %}

Additionally, you need to have admin access to a repository to change the default branch.

## Changing the default branch

{% data reusables.repositories.navigate-to-repo %}
{% data reusables.repositories.sidebar-settings %}
1. Under "Default branch", to the right of the default branch name, click {% octicon "arrow-switch" aria-label="Switch to another branch" %}.
1. Select the branch dropdown menu and click a branch name.
1. Click **Update**.
1. Read the warning, then click **I understand, update the default branch.**
