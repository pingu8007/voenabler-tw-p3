# TW VoLTE/VoWiFi Enabler for Pixel 3/3a/4 (including XL variant)

Systemlessly activates __VoLTE__ (Voice over LTE) and __VoWiFi__ (Voice over Wi-Fi) on carriers:

* __ChunghwaTel__ (TW / Chunghwa Telecom)
* __FarEastOne__ (TW / FarEast Telecom)
* __TM__ (TW / Taiwan Mobile)
* __TStar__ (TW / TStar Telecom)
* __APT__ (TW / Asia Pacific Telecom)

Now support Android 10 and Android 11!

## Prerequisite

You must have VoLTE and VoWifi service enabled on your voice plan. All major carrier in Taiwan have both enabled by default.

Have a test and make sure that they are working, then you are good to go!

## VoLTE/VoWiFi Activation

It is mandatory to [have your Pixel rooted with Magisk](https://www.xda-developers.com/google-pixel-4-root-magisk/) to install this module.
Make sure that Magisk is installed properly on your system, then proceed with these steps:

1. __Install__ this module (Zip file) on Magisk and __reboot__ the system.
1. After rebooting, __the phone may be showing "No service"__ due to the parsing of new configurations, so please wait until the operator name showed up.
1. Go to __Settings -> Network and Internet -> Mobile network__ and __enable__ __*"Enhanced 4G LTE Mode"*__ and __*"Wi-Fi calling"*__.
1. __Turn off__ Wi-Fi
1. Go to __Phone -> dial \*#\*#4636#\*#\*__ -> __Phone information__ tap at the top-right button, __select *"IMS Service Status"*__.
1. Check if __IMS Registration__ is __Registered__ and __Voice over LTE__ is __Available__ then, congrats, you're succeeded.

(Voice over Wi-Fi will be activated upon the *"Wi-Fi calling"* option in 2.)

## VoLTE/VoWiFi Deactivation

1. __Uninstall__ the module from Magisk
1. __Delete__ all the folders in /data/vendor that begin with modem
1. __Reboot__ your Pixel.

## Downloads

Check Github releases.

## OTA updates

After every OTA, to keep VoLTE/VoWiFi working, __re-install the module__ by uninstalling then install the module again.

## Notes

Since this module is fork from [voenabler-th-p3](https://github.com/thongtech/voenabler-th-p3), following carrier should also work. But they are out of scope and is not guaranteed.

* __AIS__ (Advanced Wireless Network)
* __DTAC__ (dtac TriNet)
* __TRUE-H__ (True Move H Universal Communication)

This module may also enables LTE 3CA (Carrier Aggregation) for AIS and TRUE-H on Pixel 4/4XL.

## Acknowledgements

Thanks to: [thongtech](https://github.com/thongtech/voenabler-th-p3), [nooriro](https://github.com/Magisk-Modules-Repo/volte-kr-crosshatch/), [Occy](https://m.cafe.naver.com/CommentView.nhn?search.clubid=26545115&search.articleid=159482&search.refcommentid=34700816&search.commentid=34700816&search.menuid=454&search.focus=true&search.showCafeHome=true&search.perPage=5#focusing) and [Chinese developers](https://www.google.com/search?newwindow=1&q=fdr_check)
