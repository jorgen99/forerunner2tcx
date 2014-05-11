forerunner2tcx
==============
Extract training sessions from a connected Garmin-device with
garmin-forerunner-tools and then convert them to Garmin Training Center
tcx-format. The tcx-files can then be uploaded to your training site of
choice. For example Garmin Training Center, Runkeeper, Endomondo, Strava
etc

It converts the last 10 workouts and only if they havn't already been
converted.

forerunner2tcx uses garmin-forerunner-tools, which you can install with:

    sudo apt-get install garmin-forerunner-tools 

If you garmin-forerunner-tools doesn't work with your Garmin device,
this script won't do much good. So, after installing
garmin-forerunner-tools try running the following command to see if it
works: 

    garmin_save_runs

forerunner2tcx also uses
[garmin-dev](https://github.com/cstrelioff/garmin-dev) to do the actual
gmn- to tcx- converting. It's a git submodule so in order to use it you
must run

    git submodule init
    git submodule update



