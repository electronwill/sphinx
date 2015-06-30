#Contributing to this GitHub test repository

On an OS X or Linux machine, make a GitHub account if you don't already have one, and log in.

Open a terminal window.

If you haven't already, install conda.

If you haven't already, set up SSH with GitHub using the instructions at https://help.github.com/articles/generating-ssh-keys/ .

If you haven't already, install git.

If you haven't already, set your name and email address in git:

    git config --global user.email "you@example.com"
    git config --global user.name "Your Name"

Set git to use the friendlier nano editor instead of the default vi editor for commit messages:

    git config --global core.editor "nano"

Make a new GitHub working directory, which we will somewhat arbitrarily call 'ghw', and go into it:

    mkdir ghw
    cd ghw

Go to https://github.com/electronwill/sphinx . On the right there’s a box that says "HTTPS clone URL". Click the "SSH" link underneath it so it shows the "SSH clone URL" instead. Copy that URL, such as git@github.com:electronwill/sphinx.git . Next, "clone" the repository at the URL https://github.com/electronwill/sphinx . Cloning the repository creates a copy of it on your local computer, where you can make edits before publishing them to the repository on GitHub.

    git clone git@github.com:electronwill/sphinx.git

Go into the sphinx directory in the local copy of the repository:

    cd sphinx

Make up a branch name for the change you’re about to make, such as "sign-guest-book", and enter this:

    git checkout -b sign-guest-book

To be continued...
