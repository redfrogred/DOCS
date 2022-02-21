# FIXES AND GOTCHAS

This document is for things that come up, rarely, that I had to sort out once already.  

## FLUTTER FIXES

> APK builds in emulator yet fails on phone  

Tried several things, but the fix was doing this on     the physical phone:  
1. Go to Settings  
2. Find the App  
3. Uninstall it  

> Various APK BUild errors   

First fix:  
in _ROOT_/Android/build.gradle change:  
ext.kotlin_version = '1.3.5'	  
to  
ext.kotlin_version = '1.5.0'

Second Fix:  
in _ROOT_/Android/App/build.gradle change:  
minSdkVersion flutter.minSdkVersion	  
to  
minSdkVersion 19  

You push these tweaks with   
>  git add android/build.gradle -f  
and
>  git add android/app/build.gradle -f
which forces them to stage even though .gitignore wants to resist...

