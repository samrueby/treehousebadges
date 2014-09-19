Treehouse Badges
===============

Are you a Treehouse student, workin' hard, earnin' badges, but have no way to showcase your hard work? Look no further.

![alt tag](https://dl.dropboxusercontent.com/u/24678623/Treehouse%20Badges/animaterd-widget.gif)

**Benefits**

* Look awesome
* Treehouse logo hooks up to your referal URL (people sign up, your cost goes down)
* Look at all of these pretty badges

**Okay I'm sold how do I do it?**

Well you need jQuery and you need to link to the JavaScript file. Other than that, you just call `treehouseBadges({profileName: 'yourProfile'})` 
on the jQuery selector where you would like the badge to show.

**Find your profile name**

1. Click View Profile from the menu.
![View Profile](https://dl.dropboxusercontent.com/u/24678623/Treehouse%20Badges/1-find%20profile.png)

2. Grab the last portion of the URL.
![View Profile](https://dl.dropboxusercontent.com/u/24678623/Treehouse%20Badges/2-geturl.png)


**Options**

Pass an object with your own settings to override the defaults below.

`var defaults = {
    profileName: 'yourProfile',
    width: 500
};`

If you'd lilke to style it differently, you can by inspecting the markup produced. Sorry about the inline styles, use `!important` or something.

`<div id="putMyBadgesHere"></div>
  <!-- Only include the following line if you don't already have jQuery. -->
    <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.11.1/jquery.min.js" type="text/javascript"></script>
    <script src="https://s3.amazonaws.com/RedStaplerSoftware/treehouseBadges.min.js" type="text/javascript"></script>
    <script type="text/javascript">
        <!-- Or just use $ instead of jQuery.noConflict(true) if you don't have the possibility of conflicting with another instance of jQuery. -->
    jQuery.noConflict(true)('#putMyBadgesHere').treehouseBadges({ width: 330 });    
    </script>`