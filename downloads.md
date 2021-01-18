---
layout: page
title: Downloads
icon: fa-download
permalink: downloads
order: 3
---
{% assign apks = site.static_files | where: "apk", true %}

The very last version of the application can be found on [Google Play Store](https://play.google.com/store/apps/details?id=fr.raubel.mwg.free).

Find below previous versions:
{% for apk in apks reversed %}
* [{{apk.name}}]({{apk.path | prepend: site.url }}){% endfor %}

<!--
As free variant uses Google Play Signing, APK listed above must be downloaded from Google Play Console (App Bundle Explorer).
-->
