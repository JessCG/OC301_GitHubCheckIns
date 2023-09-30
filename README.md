# OC301_GitHubCheckIns
Repository for students to upload individual GitHub check-ins

# Instructions
Check-ins should be `pushed` to GitHub on every day that there is a lecture. This can be done remotely, as long as you have access to the server. Each GitHub check-in is worth 1\% for a total of 15\%. OC 301 has a total of 19 lectures, so you can miss up to 4 GitHub check-ins without affecting your grade.

## 1. Creating a GitHub account (once; HW0)
After **Lecture 0**, you should have created a GitHub account and the instructor should have added you to your own private version of this folder. 

## 2. Setting up ssh keys (once; HW1)
In **Lecture 1**, you will set up ssh keys on the server to be ready for the GitHub check-ins. Tailored instructions will be provided in HW1.

## 3. Clone your own private version of this repository (once; HW1)
In **Lecture 1**, you will also clone your own version of this repository from GitHub to your home directory on the server. You can then try to attempt the first GitHub check-in.

## 4. GitHub check-in (every class day)
At the start of every new lecture (or at home, the day of the lecture if you prefer), follow the following instructions:

a) Log into the Jupyter Server

b) Open Terminal

c) Navigate to your `OC301_GitHubCheckIns` directory (replace `ONID` by your ONID):

    $ cd /home/ONID/OC301_GitHubCheckIns

d) `Pull` the latest version of the directory from GitHub:

    $ git pull

Typically, you should see the following message appear, unless you forgot to `push` your last check-in (no big deal):

    Already up to date.

e) Create a new check-in file with today's date, using the command we saw in ***Lecture 0*** (the file can remain empty):

    $ touch HelloWorld_$(date +"%d%B%Y").txt

f) Confirm that the new file is in your directory by using `ls`:

    $ ls

g) `Add` all of the changed files to GitHub's staging area:

    $ git add .

h) `Commit` the changes by adding a note after the option `-m`:

    $ git commit -m 'include your note here'

i) `Push` the changes to GitHub:

    $ git push

j) Confirm that your repository is up to date with the version on GitHub:

    $ git status

You should get a message that says:

    On branch main
    Your branch is up to date with 'origin/main'.

    nothing to commit, working tree clean

k) You can also go on GitHub online and confirm that there is a new file with a timestamp for just now.

If you made a mistake and changed an old file, don't worry: GitHub keeps all versions so I will be able to see when the first check-in came.

## All done! It will become easier every time.