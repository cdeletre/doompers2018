# doompers

![Get all the slides](https://github.com/cdeletre/doompers/blob/master/images/get-all-the-slides.jpeg)

Just a simple Python script to automatically check and download new uploaded slides from talks at Trooper 2018. It is based on the script I've written for Troopers 2017 not deeply tested.

This updated version of the script should work for Troopers 2018.

Ask help for usage :
```
$ ./main.py -h
Usage: main.py [options]

Options:
  -h, --help            show this help message and exit
  -f FILE, --file=FILE  Write track data to FILE (troopers-2017.json by
                        default)
  -v, --verbose         Verbose mode
  -t, --text-only       Text only, no slides are downloaded
  -r, --re-download     Re-download slides
```

The first run should give you something like this :
```
$ ./main.py
$ ./main.py
Loading data from troopers-2018.json
Extracting track urls
Adding new tracks
Updating with track data and downloading slides if found
Slide url found for ylpzm7, will try to download
Slide url found for yh9q7w, will try to download
Slide url found for eafyrq, will try to download
Slide url found for e8ysss, will try to download
Slide url found for vnyeal, will try to download
Slide url found for n9gmgn, will try to download
Slide url found for ugcntl, will try to download
Slide url found for kfyuzy, will try to download
Slide url found for m8cwua, will try to download
Slide url found for z3k3yt, will try to download
...
Writing to file troopers-2018.json
Done

$ ls ./slides
TR18_AD_Active-Directory-Security-The-Journey.pdf
TR18_AD_Introducing-a-Comprehensive-AD-Security-Metric.pdf
TR18_AR_Ads-networks-are-following-you-follow-them-back.pdf
TR18_AR_How-To-Bring-HID-Attacks-To-Next-Level.pdf
...
```
