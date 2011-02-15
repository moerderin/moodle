QUICK INSTALL
=============

For the impatient, here is a basic outline of the
installation process, which normally takes me only
a few minutes:

1) Move the Moodle files into your web directory.

2) Create a single database for Moodle to store all
   it's tables in (or choose an existing database).

3) Visit your Moodle site with a browser, you should
   be taken to the install.php script, which will lead
   you through creating a config.php file and then
   setting up Moodle, creating an admin account etc.

4) Set up a cron task to call the file admin/cron.php
   every five minutes or so.


For more information, see the INSTALL DOCUMENTATION:

   http://docs.moodle.org/en/Installing_Moodle


Good luck and have fun!
Martin Dougiamas, Lead Developer



Install xampp

Install msysgit
-Download latest version from http://code.google.com/p/msysgit/downloads/list (ie: Git-1.7.4-preview20110204.exe)
-check "Git Bash Here"
-check "Git GUI Here"

Run Git from the Windows Command Prompt
-checkout as-is, commit unix-style line endings

Install tortoise
-OpenSSH, git default ssh client

Before making commits, it is useful to add your name and email:
-git config --global user.name "Your Name"
-git config --global user.email yourmail@domain.tld

Documentation:
-http://docs.moodle.org/en/Development:Quick_Git_start_guide_for_Moodle_development

-git clone https://YOUR_GITHUB_USERNAME@github.com/ccle/moodle.git ./YOUR_LOCAL_MOODLE_FOLDER/
-git checkout DEV
-(OPTIONAL) git checkout -b <feature_name>
-change file
-git commit -a -m "updating README.txt to include basic git instructions"
-git push origin DEV (or <feature_name> if working on a feature branch)
-