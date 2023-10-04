# Git integration for [Toggl Track](https://toggl.com/track/)

## Installation

1. Clone the repo
2. Log in to Toggl Track in your browser.
3. Fill out the API key. Your API Key is at the bottom of your profile settings page.
4. Fill out the workspace id. Click on "Projects" and find the workspace id in the URL.
5. Fill out the project id. Click on a project and find the project id in the URL.
6. Copy the commit-msg file into the repository you wish to track: `cp /path/to/toggl-git/repo/commit-msg /path/to/your/repo/.git/hooks/commit-msg`
7. Make it executable:  `chmod +x /path/to/your/repo/.git/hooks/commit-msg`
8. Make a commit, and see it working :)

## Features
1. If the timer is not running, it will start the timer for the selected project when you commit.
2. If the timer is running on a different project, then it will stop the timer, and start it for the selected project.
3. It will add the commit message to the description of time entry.
