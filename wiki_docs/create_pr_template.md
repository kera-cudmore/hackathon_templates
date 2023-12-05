# Creating a PR Template

Creating a PR template streamlines the PR process by automatically providing the template in the PR body to all contributors who create a PR. This way all contributors are providing the required information for their PR in the same format, making the reviewers job a little bit easier.

## Create the template

1. On the main repository page above the files list, click the `Add file` button and then select `Create new file` from the dropdown.

2. You can choose to save your PR template in the root directory, the docs folder or in the hidden .github folder. These instructions will place the template in the `.github` folder so in the name field we will name the template:

    `.github/pull_request_template.md`

3. In the body section, add the pull request template. This can include references to the related issue in the repo, a description of the changes made, whether there are any breaking changes, screenshots of the changes for the front-end or mention a person to review the changes.

    ```markdown
    # Project Name Pull Request

    ❗ _**Please replace the text below the headers with your own comments.**_ ❗️

    ## Pull Request details:

    - Closes issue: #

    - INFO ABOUT THE WORK IN YOUR PULL REQUEST GOES HERE (Please be as descriptive as possible)

    ## Any Breaking changes:

    - IF ANYTHING YOU'RE COMMITTING WOULD BREAK SOMETHING, INCLUDE HERE WHAT WOULD BREAK
    - IF YOU HAVE NO BREAKING CHANGES, ENTER 'None'

    ## Associated Screenshots:

    _( Feel free to add gifs/png screenshots of your feature in action 😊 )_

    - IF YOU HAVE ANY SCREENSHOTS, INCLUDE THEM HERE.
    - IF YOU HAVE NO SCREENSHOTS, ENTER 'None'

    ```

4. Click `Commit changes...`, add a commit message, ensure the branch is the main branch and then commit the changes.

5. You should now be able to see the template when you create a Pull Request.
