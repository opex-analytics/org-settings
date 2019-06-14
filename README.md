# org-settings
Prevent-Public-Repos App Settings

A .github/prevent-public-repos.yml file is recommended to override the default settings created in Repository org-settings. This repository will contain global settings for the organization.

# Configuration for Prevent-Public-Repos

# Turn on Monitor Mode. In this mode the repo visibility is not modified and only an Issue is created
monitorOnly: true

# Enables detection of repos that change visibility from private to public (not just newly created ones)
enablePrivateToPublic: false

# Issue Title when repo is privatized
privatizedIssueTitle: '[CRITICAL] Public Repositories are Disabled for this Org'

# Issue Body when repo is privatized
privatizedIssueBody: 'NOTE: Public Repos are disabled for this organization! Repository was automatically converted to a Private Repo. Please contact an admin to override.'

# Issue Title when monitor mode is enabled
monitorIssueTitle: '[CRITICAL] Public Repository Created'

# Issue Body when monitor mode is enable
monitorIssueBody: 'Please note that this repository is publicly visible to the internet!'

# Users/Groups that should be cc'ed on the issue. Should be users/groups separated by a space.
# ccList: '@user123 @user456'

# Repos to  exclude in detection. Should be a List of Strings.
# excludeRepos: ['repo1', 'repo2']
