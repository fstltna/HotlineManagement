# Hotline Management Console (1.0)
Allows you to manage your Hotline server process with a text based UI

---

You will need to run cpan and install these modules:

- cpan -i UI::Dialog
- cpan -i Term::ReadKey
- cpan -i Term::ANSIScreen

Run "hmc". If you need to change any settings after this, edit "~/.hmcrc" and make the desired changes. This can be done within hmc itself.

You also need to have my Hotline Startup Script and Backup Script installed.

I then suggest you add this directory (HotlineManagement) into your path, so that you can just run "git pull" to upgrade to the latest version aamc as updates come out.
