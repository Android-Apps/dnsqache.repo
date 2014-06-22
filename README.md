DnsQache
=====================
This repository provides for the git-repo XML manifest for DnsQache.
Effectively the default.xml file represents a 'bill of materials' necessary to build and deliver DnsQache.

Submitting Patches
------------------
You can send patches by using commands similar to the following example for Ubuntu (though development is not limited to Ubuntu):

    sudo apt-get install git-review
    cd <project>
    <make edits>
    git add -A
    git commit -m "Message"
    git-review

Register at [DnsQache Gerrit] (http://review.tomhite.us) (coming soon.) and use the username that you registered with git-review. **Make sure to add your ssh keys to your Gerrit profile.**

Submit patches in a **single commit. Squash multiple commits using rebase similar to: git rebase -i HEAD~<# of commits>**

The git-review package will only have to be installed once

If you are going to make extra additions, just repeat steps (Don't repo start again), but instead of git commit -m
use git commit --amend. Gerrit will recognize it as a new patchset.

To view the status of your and other's patches, visit [DnsQache Code Review](http://review.tomhite.us)

Getting Started
---------------

To get started with development, you'll need to get
familiar with [Git, Gerrit and Repo](http://source.android.com/download/using-repo).

Setup build environment - Android SDK and NDK properly setup and on the path, Java (Sun), Make.

To initialize your local repository using the DnsQache trees, use a command like this:

    repo init -u https://github.com/Android-Apps/dnsqache.repo.git -b <branch>

To initialize for master branch builds:

    repo init -u https://github.com/Android-Apps/dnsqache.repo.git -b master

Then to sync up:

    repo sync -j#

Where # is the specific number of Jobs (i.e., threads used for parallel syncing), 4 is default, change in accordance to internet performance/bandwidth/speed.

Then to build:

    Coming soon.
