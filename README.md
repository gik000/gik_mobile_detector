Gik Mobile Detector
===================

This is a Drupal 7 module, based on "Mobile-Detect" library that detects if the current user is on a mobile device or on a desktop one.


At this stage the module print a class into the tag "body".
It could write one of the following three class names
  device-tablet
  device-mobile
  device-desktop

It is very usefull if you are used to limit certain javascript or css actions depending on the device.

For example you could have a colorbox only on mobile devices:

  $(document).ready(function(){
    add_colorbox();
  });
  function add_colorbox(){
    if($('body').hasClass('device-desktop') && typeof colorbox == 'object' && (typeof colorbox != undefined || typeof colorbox != 'undefined')){
    $(".my-colorbox-elements").colorbox({'max-width':'80%', 'max-height':'90%'});
    }
  }
  
==================
References

"Mobile-Detect" - https://github.com/serbanghita/Mobile-Detect
