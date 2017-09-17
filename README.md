Manjaro Dark Conky -Abhishek Munagekar
=======================================

![Screenshot](https://github.com/munagekar/MJRDarkConcky/blob/master/MJRDarkConky.png)
This is a dark conky manager theme which was tested with the following concky version.

    conky 1.10.6_pre compiled Tue May 16 08:25:34 UTC 2017 for Linux 4.10.9-1-ARCH x86_64

This theme was tested on Manjaro 17.0.5 64 bit XFCE but should work fine with any other distro and desktop environment.
It is fully modular and can be easily customized,comes with widgets for Time, Day of Week, Weather Forecast, News, And Real Time Bitcoin Value. I am also Planning to add a forex & live cricket & stock indice plugin. If you want a cool desktop definitely give this theme a try.

Wallpaper
---------

Use any dark wallpaper, should be really black. Texture & Gradients will look cool.
Any dark minimalistic wallpaper should also do
The Wallpaper shown in the screenshot is also attached however you can change it anything you prefer.
I have used the following wallpaper : https://pre00.deviantart.net/c84a/th/pre/f/2016/213/c/a/manjaro_monochrome_ws_wallpaper_by_rvc_2011-dac94gy.jpg
![Wallpaper](https://pre00.deviantart.net/c84a/th/pre/f/2016/213/c/a/manjaro_monochrome_ws_wallpaper_by_rvc_2011-dac94gy.jpg)

Python Dependencies
-------------------

Make sure you have the following packages installed for Python2

    urllib
    json
    feedparser
    dateutil
    datetime
    

You can get them using pip.

Python Issues
-------------

Since Manjaro uses python3 by default and the theme has two python files which had to be called using python2 however is if you are using Ubuntu you will have to edit these files and use python instead of python 2.
Make changes in the following files

    ~/.conky/TransparentTilesv3/weather_forecast
    ~/.conky/ConkyWhiteTilesv2/news

News & Weather Issues
---------------------

I have fixed yahoo weather api issues.
News is retrieved from Times of India Headlines RSS feed
Weather is retrieved from Yahoo Weather. With City: Katraj Country:India
You might want to change these settings in

    ~/.conky/AbhishekManjaro/weather.py

    ~/.conky/AbhishekManjaro/news.py


Installation & Using the Theme
------------------------------

This theme has the following dependencies

 - Conky Package
 - Conky Manager
 - Python
 - Lua(Not sure possibly required by Conky)
Use your package manager to get theme if they aren't installed on your machine.

Clone the repository and copy the AbhishekManjaro folder into ~/.conky.

Manage Weather Configuration by making changes in `weather.py`

Manage News RSS stream by making changes in `news.py`
Finally select the theme using Conky Manager.



Screenshot
----------

This screenshot was taken on Manjaro 17.04 XFCE desktop so you might get slightly different results
I have also installed plank and set background to transparent for my dock.
The default XFCE Panel has been moved to the top
And Numix Circular Icon Theme has been used to get circular icons.

Future Development
----------

 1. Ubuntu Fork for The Theme to make it easy for beginners. This more efforts on my parts as I will have to replicate the work there. - Low Priority
 2. Forex Widget - High Priority
 3. Live Cricket Widget
 4. Live Stock Indice Widget


Version History
----------
 1.0 : Came with Weather Forecast Widget , Modified Gotham Style Panel, Network Panel, Modified CPU Temperature Panel, News Widget. 
 2.0 : Moved cache to AbhishekManjaro folder instead of /tmp. This corrects the weather bug, since weather data fetching requires internet. Now old weather data can be used till new data is fetched. Cool New Real Time Bitcoin Price Widget. Reduced the size of theme by removing unnecessary files.

