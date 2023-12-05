# Project Set Up for Collaborators

# Forking and Cloning

1. On the repo page for **repo link here**, click the fork button in the top right. This will create a copy of the original repository in your GitHub, and you will be redirected to the main repo page for your forked version. Any changes you make in your forked repo won't affect the original repo until you create a pull request to have those changes merged into the original (more on this soon!)

2. In your forked repo, click the code button and select HTTPS. Copy the link displayed.

3. Open up your Integrated Development Environment (IDE) and in the terminal enter:

    ```bash
    git clone {insert copied url here}
    ```

    This will then clone the project for you to work on locally.

    ❗️If using GitPod or CodeAnywhere, you can skip this step and just click the green GitPod or Purple CodeAnywhere extension button on your repo.

# Setting the Upstream

As mentioned above, any changes you make in your forked repo won't affect the original repo (the upstream) unless you push those changes to the original, making a Pull Request. Lets get set up to push to the upstream below:

1. In the terminal run the following command:

    ```bash
    git remote add upstream **CHANGE THIS TO REPO https://github.com/kera-cudmore/this-is-the-way.git**
    ```

    This command lets your editor know what repo is the upstream, and allows them to 'connect' with each other. 

2. To check that we have that set up correctly, we can run the following command and should see something like the example below:

    ```bash
    git remote -v

    origin    https://github.com/YOUR_USERNAME/** CHANGE this-is-the-way.git** (fetch)
    origin    https://github.com/YOUR_USERNAME/** CHANGE this-is-the-way.git** (push)
    upstream  https://github.com/kera-cudmore/** CHANGE this-is-the-way.git** (fetch)
    upstream  https://github.com/kera-cudmore/** CHANGE this-is-the-way.git** (push)
    ```

    You should have 2 origins listed from your forked repo (one used for pushing and one for fetching) and 2 from the upstream. Setting this up creates the relationship between the upstream and your forked repo and is what allows you to perform Pull Requests.

    ❗️This step may already have been done for you if you've created your workspace from the GitPod/CodeAnywhere buttons in your forked repo. You can check if this is the case by running the following command to make sure you have something like the example above:

    ```bash
    git remote -v
    ```

# Setting up a branch

The last thing to set up before getting started is a branch. These are a great way to create another layer of security in the project, by allowing you to experiment without worrying about the code.

1. In the terminal, run the following command:

    ```bash
    git checkout -b your-branch-name-here
    ```

    This command is a shortcut, and allows you to create a new branch and move onto that branch in one command.

2. Now we want to tell git that we want this to be our *tracked* branch, and can do so by running the following command:

    ```bash
    git push -u origin your-branch-name-here
    ```

    Its up to you whether you choose to work on the same branch throughout, or whether you create a new branch for each feature you work on. If you choose to create a new one, just remember you'll need to perform these steps again.

And you're done, the project is all set up!
