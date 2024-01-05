# Add branch protection to the repository

We can add some security to the main repository to prevent anyone pushing code to the main branch without first having this reviewed by another member of the team. This is called branch protection.

## To set branch protection

Branch protection can only be set by the repository owner or collaborators who have admin permissions or a custom role with 'edit repository rules' enabled.

1. In the main repository, open the <kbd>settings</kbd> tab and then click on <kbd>Branches</kbd> in the left hand menu.

    ![Settings and Branch Menu](https://github.com/kera-cudmore/hackathon_templates/assets/92253071/f5e670ea-1fb2-4439-8780-86b2ae120104)

2. Click the <kbd>add branch protection rule</kbd> button.

    ![Create Branch Protection Rule](https://github.com/kera-cudmore/hackathon_templates/assets/92253071/c61d50e5-2bfd-415a-afda-22ded107c70f)

3. In the **Branch name pattern** section, enter the branch you would like to protect - as we want to prevent any code being pushed to the main branch, we will enter main (if your branch is called master, enter master instead).

    ![Branch to Protect Field](https://github.com/kera-cudmore/hackathon_templates/assets/92253071/67209221-e868-4364-b540-a0df26df6699)

4. In the **Protect matching branches** section, we will want to select the following checkboxes:

    * `Require a pull request before merging` - this will require all pushes to the main branch to have completed a pull request before the code can be merged.

    * `Require approvals` - this requires that another member of the team must have reviewed and approved the code before it can be merged. You can select the number of approvals needed in the dropdown box.

    * `Require conversation resolution before merging` - *optional* - any conversations relating to the code must be resolved before the code can be merged.

    * `Do not allow bypassing the above settings` - *optional* - this will prevent the owner of the repo, admin and people with the role 'bypass branch protections' pushing directly to the main branch without review.


    ![Protect Matching Branches Rules](https://github.com/kera-cudmore/hackathon_templates/assets/92253071/20b5c96b-9ebf-4671-acd3-a6946f2ae9ee)

5. Click the <kbd>Create</kbd> button at the bottom of the page to enable the branch protection.
