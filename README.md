# Hotline Management Console (1.1.1)
Allows you to manage your Hotline server process with a text based UI

---

Install all the dependancies by running this command:

- ./installdeps

Run "hmc". If you need to change any settings after this, edit "~/.hmcrc" and make the desired changes. This can be done within hmc itself.

You also need to have my Hotline Startup Script and Backup Script installed.

To send out daily emails of the downloads add this to crontab:

1. create a cron job like this:

        59 23 * * * /home/hotlineuser/HotlineManagement/DownloadedFiles

2. Create the prefs by running /home/hotlineuser/HotlineManagement/DownloadedFiles prefs

