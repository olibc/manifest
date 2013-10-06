olibc - Another C library optimized for embdded Linux.

Downloading the source tree
---------------------------

Repo is a tool that makes it easier to work with Git in the context of Android.
For more information about Repo, see [Version Control](http://source.android.com/source/version-control.html).

To install, initialize, and configure Repo, follow these steps:

* Make sure you have a bin/ directory in your home directory, and that it is included in your path:
  ```
  $ mkdir ~/bin
  $ export PATH=~/bin:$PATH
  ```

* Download the Repo script and ensure it is executable:
  ```
  $ curl  http://commondatastorage.googleapis.com/git-repo-downloads/repo > ~/bin/repo
  $ chmod a+x ~/bin/repo
  ```

After installing Repo, set up your client to access the android source repository:

* Create an empty directory to hold your working files. Give it any name you like:
  ```
  $ mkdir -p workspace-olibc
  $ cd workspace-olibc
  ```

* Run repo init to bring down the latest version of Repo with all its most recent bug fixes:
  ```
  $ repo init -u https://github.com/olibc/manifest.git
  ```

* To pull down files to your working directory from the repositories as specified in the default manifest, run
  ```
  $ repo sync
  ```
