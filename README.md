# Weather Underground widget for HABpanel (Openhab)

## Description
Weather Underground widget for HABpanel (Openhab). You must use the Weather Underground binding SNAPSHOT-2.3.0 minimum build #1212, otherwise the iconKey binding will not work.

## Installation
- Install the Weather Underground binding via PaperUI.
- Configure the Thing: Local Weather (You can set your preferred language)
- Import the downloaded widget to your HABpanel
- Download weather-underground-icons repository from [here](https://github.com/manifestinteractive/weather-underground-icons)
- The 'weather-underground-icons' folder should be stored in your '/conf/html/' folder.
- Set the 'ServerPath' variable in the widget to '/static/weather-underground-icons-master/dist' (default).
- Place the three .png images in your '/conf/html/weather-underground-icons/dist/images' folder.

The complete structure would look like this:

- /conf/html
  - weather-underground-icons
    - css
    - js
    - dist
      - wu-icons-style.css
      - wu-icons-style.min.css
      - icons <= this is where the different icon theme’s are stored
      - images
        - feel.png
        - humidity.png
        - wind.png
        
Your ServerPath variable in the widget would look like this:

<div ng-init="ServerPath='/static/weather-underground-icons-master/dist'; IconSet='white'">

You can set the 'IconSet' to one of the following options:
- black
- solid-black
- solid-white
- white

The location of your ‘/conf/html’ folder depends on your Openhab installation.

## Help
If you need any help, use this [topic](https://community.openhab.org/t/weather-underground-widget-with-forecast/40260) on the Openhab community forum.

For issues and feature requests, please use the [Issues module](https://github.com/BasvanH/habpanel-widget-weatherunderground/issues) on Github.
