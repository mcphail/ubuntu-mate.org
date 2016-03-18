<!--
.. title: Ubuntu MATE 16.04 Beta 2
.. slug: ubuntu-mate-xenial-beta2
.. date: 2016-03-24 20:00:00 UTC
.. tags: Ubuntu,MATE,Xenial,beta2,draft
.. link:
.. description: Ubuntu MATE 16.04 (Xenial Xerus) LTS Beta 2
.. type: text
.. author: Martin Wimpress
-->

We are preparing Ubuntu MATE Xenial Xerus (16.04) for distribution on
[April 21st, 2016](https://wiki.ubuntu.org/XenialXerus/ReleaseSchedule)
With this *Beta 1* pre-release, you can see what we are trying out in
preparation for our next (stable) version.

## What works?

People tell us that Ubuntu MATE is stable. You may, or may not, agree.

Ubuntu MATE *Beta Releases* are *NOT* recommended for:

  * Regular users who are not aware of pre-release issues
  * Anyone who needs a stable system
  * Anyone uncomfortable running a possibly frequently broken system
  * Anyone in a production environment with data or workflows that need to be reliable

Ubuntu MATE *Beta Releases* are recommended for:

  * Regular users who want to help us test by finding, reporting, and/or fixing bugs
  * Ubuntu MATE, MATE, and GTK+ developers

## What changed since the Ubuntu MATE 16.04 Beta 1 release?

First of all, I'd like to extend my thanks to:

  * **[Luke Horwell](https://ubuntu-mate.community/users/lah7/)** and **[Robin Thompson](https://github.com/robint99)** for for their work on Ubuntu MATE Welcome and Software Boutique.
  * **[Gunnar Hjalmarsson](https://launchpad.net/~gunnarhj)** for his help making `im-config` and `gnome-language-selector` compatible with Ubuntu MATE.
  * **[Rico Tzschichholz](https://launchpad.net/~ricotz)** for his help completing MATE integration for Synapse.
  * **[Alexei Sorokin](https://build.opensuse.org/user/show/XRevan86)** and **[Alberts Muktupāvels](https://launchpad.net/~albertsmuktupavels)** for their help improving MATE integration in Compiz.
  * **[Timo Jyrinki](https://launchpad.net/~timo-jyrinki)**, **[Daniel Holbach](https://launchpad.net/~dholbach)** and **[Artur Rona](https://launchpad.net/~ari-tczew)** for sponsoring package updates for Ubuntu MATE.

<div align="center">
<img src="/gallery/blog/ubuntu-mate-1604-beta2.png" alt="Ubuntu MATE 16.04 Beta 2" />
</div>

Thanks to everyone else from the Ubuntu MATE community who contributed to this release!

### Here is what changed in Ubuntu MATE 16.04 Beta 2 since Beta 1.

  * Added Synapse 0.2.99.2-1
    * Synapse now features complete MATE integration. Synapse is
    installed by default but not active by default. It can be enabled
    using MATE Tweak.
  * Updated to MATE Tweak 3.5.7
    * Adds *Enable Launcher* to the *Interface* section which
    activates/deactives Synapse.
    * Also fixed [LP: 1548011](https://bugs.launchpad.net/bugs/1548011)
  * Updated to Compiz 0.9.12.2+16.04.20160318-0ubuntu1
    * Improved MATE Compiz integration, `gtk-window-decorator` will now
    use settings from Marco when Compiz detects it is running in a MATE
    session.
    * Google Chrome and Chromium windows are now considered Compiz
    windows in fullscreen to avoid tearing.
    * Refined the Compiz profile for MATE to correct some minor issues.
  * Updated to Plank 0.11
    * Adds Docklets and also includes a new theme for Ubuntu MATE
    contributed by [Holger Rueckershaeuser](http://holgerrpl.tk/).
  * Updated to MATE Menu 5.6.9
    * While search for an application, the top match will be launched
    when Enter is pressed. [LP: #1552363](https://bugs.launchpad.net/bugs/1552363)
  * Updated to Ubuntu MATE Welcome 16.04.5
    * Fix splash screen flicker. [LP: #1549072](https://bugs.launchpad.net/bugs/1549072)
    * Fix Codec installation. [LP: #1558986](https://bugs.launchpad.net/bugs/1558986)
    * Fix system information.
    * Fix subscription updates.
    * Fix Abobe Flash, Dropbox and RednoteBook installs.
    * Fix Google Chrome repsoitory, i386 is no longer available.
    * Fix LibreOffice upgrades.
    * Add Ardour, Corebird, Gajim, GNOME Software, Gpick, Time Tracker,
    MuseScore, Nuvola Player, OBS Studio, Pinta, Simple Screen Recorder,
    Subsurface, SparkleShare, Vivaldi, Wireshark and Zenmap to
    Software Boutique.
    * Add translation framework.    
    * Add Chinese (zh_TW) and English (en_GB) translations.
  * Updated to Ubuntu MATE Artwork 16.04.4
    * Icon rendering in menus is faster and icon inheritance is fixed.
    * Corrected rendering of Mozo (menu editor).
    * Update buttons and scrollbars so GTK2 and GTK3 themes are more
    closely aligned.
    * Add resize area and shadows for CSD windows.
    * Add minimal style for CSD windows running without a compositor.
    * Add community contributed wallpaper [Blissful Sky](https://ubuntu-mate.community/t/i-made-a-new-wallpaper-blissful-sky/4277) by Jordyn.
    * Adds panel/indicator icons for Synapse.
    * Fixes [LP: #1552363](https://bugs.launchpad.net/bugs/1552363),
    [LP: #1552363](https://bugs.launchpad.net/bugs/1552363),
    [LP: #1556618](https://bugs.launchpad.net/bugs/1556618),
    [LP: #1549079](https://bugs.launchpad.net/bugs/1549079),
    [LP: #1541929](https://bugs.launchpad.net/bugs/1541929),
    [LP: #1551029](https://bugs.launchpad.net/bugs/1551029),
    [LP: #1499521](https://bugs.launchpad.net/bugs/1499521),
    [LP: #1442738](https://bugs.launchpad.net/bugs/1442738),
    [LP: #1364073](https://bugs.launchpad.net/bugs/1364073)
  * Updated to Ubuntu MATE Settings 16.04.4
    * Auto-corrects pre-existing MATE incompatible input methods.
    * Add modified mate-panel.desktop, specific to Ubuntu MATE, to cater
    for the all supported  compositors and disk encryption strategies.
    [LP: #1553070](https://bugs.launchpad.net/bugs/1553070)
    * Add all optical video mime types and enable autoplay.
    * Correct the settings for Plank. See LP: #1556651  
    * Correct the GNOME Main Menu entry for `network-config-tool`.
  * Updated to `mate-dock-applet` 0.69.
    * Several bugs fixes. [LP: #1555324](https://bugs.launchpad.net/bugs/1555324)
    [LP: #1550392](https://bugs.launchpad.net/bugs/1550392)
    [LP: #1554128](https://bugs.launchpad.net/bugs/1554128)
  * Updated Ubuntu MATE Ubiquity Slideshow artwork.  
  * Fixed Python plug-ins for Caja
    * Folder Color, Deja Dup Caja, Insync Caja and others now work again.
  * Fixed `im-config` and `gnome-language-selector`.
    *  Ensures a MATE compatible input method is selected by default.
    [LP: #1550325](https://bugs.launchpad.net/bugs/1550325)
  * Replaced guvcview with Cheese.

<div class="bs-component">
    <div class="jumbotron">
        <h1>Download Ubuntu MATE 16.04</h1>
        <p>Join the fun and experience a retrospective future.</p>
        <a href="/xenial/" class="btn btn-primary btn-lg">Download</a>
        </p>
    </div>
</div>

## Known Issues

Here are the known issues.

### Ubuntu family issues

This is our known list of bugs that affect all flavours.

  * Cryptsetup password prompt is not shown.
    * [LP: #1359689](https://bugs.launchpad.net/bugs/1359689)
    * [LP: #1530548](https://bugs.launchpad.net/bugs/1530548)
  * Plymouth does not display the graphical boot splash.
    * [LP: #1370707](https://bugs.launchpad.net/bugs/1370707).
  * Shutdown/Restart of the live session does not work in Virtualbox and VMWare guests.
    * [LP: #1447038](https://bugs.launchpad.net/bugs/1447038)
  * The input box for editing a Wired connection static IP address doesn't appear correctly.
    * [LP: #1530323](https://bugs.launchpad.net/bugs/1530323)
  * Swap partition *may* fail to be created when installing on a disk with existing partitions.
    * [LP: #990744](https://bugs.launchpad.net/bugs/990744)

### Ubuntu MATE issues

This is our known list of bugs that jut affect Ubuntu MATE.

  * The Blueman applet may crash on login on computer that have Bluetooth
  but the device is disabled.
    * [LP: #1533206](https://bugs.launchpad.net/bugs/1533206)

The issues outlined above will be resolved via updates.

### PowerPC

  * Running Linux on PowerPC can require some tinkering and the following are useful references.
    * [PowerPC Known Issues](https://wiki.ubuntu.com/PowerPCKnownIssues)
    * [PowerPC FAQ](https://wiki.ubuntu.com/PowerPCFAQ)

You'll also want to check the Ubuntu MATE bug tracker to see what has already
been reported. These issues will be addressed in due course.

  * [Ubuntu MATE Bug Tracker](https://bugs.launchpad.net/ubuntu-mate)

## Feedback

Is there anything you can help with or want to be involved in? Maybe you just
want to discuss your experiences or ask the maintainers some questions. Please
[come and talk to us](https://ubuntu-mate.community/).