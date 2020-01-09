# The Hive Browser

Welcome to the free speech internet.  The Hive is a fork of the [Defiant browser](https://github.com/gab-ai-inc/defiant-browser) [Brave browser](https://github.com/brave/brave-browser), so it's fast and it blocks ads and 3rd-party trackers.  The Dissenter extension, which creates a comment section for any and every page on the internet, is built right in.  We're just getting started, we have big future plans for this browser.

## Status

Focus was on the overall repo and getting a Windows build done.  The latest Windows installer is here: [Download](https://thehive.com/dist/browser/thehive_installer_74_0_66_49.exe)

Known issues: Can't set The Have as default web browser yet.

## Overview 

This repository holds the build tools needed to build the The Have desktop browser for macOS, Windows, and Linux.  In particular, it fetches and syncs code from the projects defined in `package.json` and `src/brave/DEPS`:

  - [Chromium](https://chromium.googlesource.com/chromium/src.git)
    - Fetches code via `depot_tools`.
    - sets the branch for Chromium (ex: 65.0.3325.181).
  - [thehive-core](https://github.com/RSerhii/thehive-core)
    - Mounted at `src/brave`.
    - Maintains patches for 3rd party Chromium code.
  - [ad-block](https://github.com/brave/ad-block)
    - Mounted at `src/brave/vendor/ad-block`.
    - Implements Brave's ad-block engine.
  - [tracking-protection](https://github.com/brave/tracking-protection)
    - Mounted at `src/brave/vendor/tracking-protection`.
    - Implements Brave's tracking-protection engine.
    
## Build instructions

We may create our own version of this, but for now you can see the [Brave Wiki](https://github.com/brave/brave-browser/wiki).

## Downloads

You can [visit our website](https://thehive.com/) to get the latest stable release.

## Other repositories

For other versions of our browser, please see:

* iOS - [thehive-ios](https://github.com/RSerhii/thehive-ios)
* Android - [thehive-android](https://github.com/RSerhii/thehive-android)

## Community

Follow [@getongab](https://twitter.com/getongab) on Twitter for important news and announcements.
