# Hotline Management Console (1.2.1)
Allows you to manage your Hotline server process with a text based UI

---

Install all the dependancies by running this command:

- ./installdeps

Run "hmc". If you need to change any settings after this, edit "~/.hmcrc" and make the desired changes. This can be done within hmc itself.

You also need to have my Hotline Startup Script and Backup Script installed.

To send out daily emails of the downloads add this to crontab:

1. create a cron job like this:

        59 23 * * * /home/hotlineuser/HotlineManagement/DownloadedFiles
        1 1 * * * /home/hotlineuser/HotlineManagement/checkmobiusversion


2. Create the prefs by running /home/hotlineuser/HotlineManagement/DownloadedFiles prefs

3. Create the update prefs by running /home/hotlineuser/HotlineManagement/checkmobiusversion

4. Add these lines to the tracker list:
>>>>
  - badmoon.biz:5499
  - hotline.duckdns.org:5499
  - hotline.jpn.ph:5499
  - tracked.nailbat.com:5499
  - tracked.stickytack.com:5499
<<<<
And add these to the IgnoreFiles section:
>>>>
  - '^_'       # Ignore all files starting with "_"
  - '^index\.html'       # Ignore index.html files
>>>>
5. Set the "EnableTrackerRegistration" variable to "true"

