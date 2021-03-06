NavigationTabStrip
==================

Navigation tab strip with smooth interaction.

[![DevLight](https://lh4.googleusercontent.com/-9btnRFp_eVo/V5cfwZsBpMI/AAAAAAAAC4E/s4NGoezKhpAVdVofAoez1QWpzK5Na8_cQCL0B/w147-h20-no/devlight-badge.png)](http://devlight.com.ua)

[![Android Arsenal](https://img.shields.io/badge/Android%20Arsenal-NavigationTabStrip-yellow.svg?style=flat)](http://android-arsenal.com/details/1/3603)
[![Android](https://img.shields.io/badge/platform-android-brightgreen.svg?style=flat&label=Platform)](https://github.com/DevLight-Mobile-Agency)
[![Download](https://api.bintray.com/packages/gigamole/maven/navigationtabstrip/images/download.svg) ](https://bintray.com/gigamole/maven/navigationtabstrip/_latestVersion)
[![Crates.io](https://img.shields.io/crates/l/rustc-serialize.svg?maxAge=2592000&label=License)](https://github.com/DevLight-Mobile-Agency/NavigationTabStrip/blob/master/LICENSE.txt)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/d41363ef8b8542b5ad7c6a3b1a788e95)](https://www.codacy.com/app/gigamole53/NavigationTabStrip?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=DevLight-Mobile-Agency/NavigationTabStrip&amp;utm_campaign=Badge_Grade)

![](https://lh6.googleusercontent.com/-wpGnxe1Vefc/VziiygaS9WI/AAAAAAAACd4/c4fU_EG-DHkoby1SIbI5BDtqITpGiZZhwCL0B/w326-h551-no/nts.gif)

You can check the sample app [here](https://github.com/DevLight-Mobile-Agency/NavigationTabStrip/tree/master/app).

Download
------------

You can download a `.aar` from GitHub's [releases page](https://github.com/DevLight-Mobile-Agency/NavigationTabStrip/releases).

Or use Gradle jCenter:

```groovy
dependencies {
    repositories {
        mavenCentral()
        maven {
            url  'http://dl.bintray.com/gigamole/maven/'
        }
    }
    compile 'com.github.devlight.navigationtabstrip:navigationtabstrip:+'
}
```

Or Gradle Maven Central:

```groovy
compile 'com.github.devlight.navigationtabstrip:navigationtabstrip:1.0.3'
```

Or Maven:

```groovy
<dependency>
    <groupId>com.github.devlight.navigationtabstrip</groupId>
    <artifactId>navigationtabstrip</artifactId>
    <version>1.0.3</version>
    <type>aar</type>
</dependency>
```

Android SDK Version
=========

`NavigationTabStrip` requires a minimum SDK version of 11. 

Sample
========

<b>Parameters</b>

For `NTS` you can set such parameters as:
 
 - color:
    
    allows you to set strip color.
    
 - size:
     
    allows you to set titles size. By default `NTS` use auto titles size.
    
 - weight:
     
    allows you to set weight(height) of strip.
    
 - factor:
     
    allows you to set strip resize factor.
    
 - titles:
    
    allows you to set `NTS` titles. This is your tabs.
    
 - type:
    
    allows you to set strip type - line or point.
    
 - gravity:
    
    allows you to set strip gravity - top or bottom.
    
 - view pager:
     
    allows you to connect `NTS` with `ViewPager`. If you want your can also set `OnPageChangeListener`.    
    
 - typeface:
 
    allows you to set custom typeface to your titles.
 
 - corners radius:
    
    allows you to set corners radius of strip.

 - animation duration:
  
    allows you to set animation duration.
      
 - inactive color:

    allows you to set inactive titles color.
     
 - active color:
  
    allows you to set active title color.
     
 - tab strip listener:
  
    allows you to set listener which triggering on start or on end when you set tab index.

<b>Tips</b>

If your set `ViewPager` you can action down on active tab and do like drag.

`NTS` use only upper case titles.

<b>Init</b>

Check out in code init:

```java
final NavigationTabStrip navigationTabStrip = (NavigationTabStrip) findViewById(R.id.nts);
navigationTabStrip.setTitles("Nav", "Tab", "Strip");
navigationTabStrip.setTabIndex(0, true);
navigationTabStrip.setTitleSize(15);
navigationTabStrip.setStripColor(Color.RED);
navigationTabStrip.setStripWeight(6);
navigationTabStrip.setStripFactor(2);
navigationTabStrip.setStripType(NavigationTabStrip.StripType.LINE);
navigationTabStrip.setStripGravity(NavigationTabStrip.StripGravity.BOTTOM);
navigationTabStrip.setTypeface("fonts/typeface.ttf");
navigationTabStrip.setCornersRadius(3);
navigationTabStrip.setAnimationDuration(300);
navigationTabStrip.setInactiveColor(Color.GRAY);
navigationTabStrip.setActiveColor(Color.WHITE);
navigationTabStrip.setOnPageChangeListener(...);
navigationTabStrip.setOnTabStripSelectedIndexListener(...);
```
            
Other methods check out in sample.

And XML init:

```xml
<com.gigamole.navigationtabstrip.NavigationTabStrip
    android:layout_width="match_parent"
    android:layout_height="50dp"
    app:nts_color="#000"
    app:nts_size="15sp"
    app:nts_weight="3dp"
    app:nts_factor="2.5"
    app:nts_titles="@array/titles"
    app:nts_type="point"
    app:nts_gravity="top"
    app:nts_typeface="fonts/typeface.otf"
    app:nts_corners_radius="1.5dp"
    app:nts_animation_duration="300"
    app:nts_active_color="#000"
    app:nts_inactive_color="#c4c4c4"/>
```

Getting Help
======

To report a specific problem or feature request, [open a new issue on Github](https://github.com/DevLight-Mobile-Agency/NavigationTabStrip/issues/new).

License
======

Apache 2.0 and MIT. See [LICENSE](https://github.com/DevLight-Mobile-Agency/NavigationTabStrip/blob/master/LICENSE.txt) file for details.

Inspiration
======

|     |     |     |
|:---:|:---:|:---:|
![](https://d13yacurqjgara.cloudfront.net/users/259538/screenshots/2594107/tabs-transition.gif)|![](https://s-media-cache-ak0.pinimg.com/originals/42/b4/47/42b447c201642b2e82c981bc6599d850.gif)|![](https://s-media-cache-ak0.pinimg.com/originals/40/ae/5e/40ae5eed129a90ac9e7ee73cdb24e69d.gif)

Author
=======

Made in [DevLight Mobile Agency](https://github.com/DevLight-Mobile-Agency)

Created by [Basil Miller](https://github.com/GIGAMOLE) - [@gigamole](mailto:gigamole53@gmail.com)

Support
=======

If you'd like to support future development and new product features, please make a payments on Gratipay and Beerpay or become a patron on Patreon.

[![Gratipay](https://img.shields.io/gratipay/user/gigamole.svg?maxAge=2592000)](https://gratipay.com/~GIGAMOLE/)
[![Beerpay](https://beerpay.io/DevLight-Mobile-Agency/NavigationTabStrip/badge.svg?style=flat)](https://beerpay.io/DevLight-Mobile-Agency/NavigationTabStrip)
[![Patreon](https://lh5.googleusercontent.com/-lXI_oKp5724/V58ysdDtxHI/AAAAAAAAC7s/g91W_YT2SM0Q_VaIhDAMmoe-jHPP3ijJwCL0B/w140-h20-no/patreon-badge.png)](https://www.patreon.com/gigamole)

Also, if you use this library in applications that are available on Google Play, please report it to us or author.

Thanks in advance.