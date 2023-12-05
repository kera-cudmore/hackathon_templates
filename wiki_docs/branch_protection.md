# Add branch protection to the repository

We can add some security to the main repository to prevent anyone pushing code to the main branch without first having this reviewed by another member of the team. This is called branch protection.

## To set branch protection

Branch protection can only be set by the repository owner or collaborators who have admin permissions or a custom role with 'edit repository rules' enabled.

1. In the main repository, open the **settings** tab and then click on **Branches** in the left hand menu.

2. Click the **add branch protection rule** button.

3. In the **Branch name pattern** section, enter the branch you would like to protect - as we want to prevent any code being pushed to the main branch, we will enter main (if your branch is called master, enter master instead).

4. In the **Protect matching branches** section, we will want to select the following checkboxes:

    * `Require a pull request before merging` - this will require all pushes to the main branch to have completed a pull request before the code can be merged.

    * `Require approvals` - this requires that another member of the team must have reviewed and approved the code before it can be merged. You can select the number of approvals needed in the dropdown box.

    * `Require conversation resolution beofore merging` - any conversations relating to the code must be resolved before the code can be merged.

    * `Do not allow bypassing the above settings` - this will prevent the owner of the repo, admin and people with the role 'bypass branch protections' pushing directly to the main branch without review.

5. Click the **Save changes** button to enable the branch protection.
