 # OTHER COMMANDS
 
> FLUTTER AND ADB

flutter run -d LG  

adb uninstall com.[PROJECT_NAME_HERE]

> FLUTTER BUILDS  

flutter run --release  
*Makes a release APK on your attached phone using the appropriate build type (of the normal 3 types)*

flutter build apk --split-per-abi   
*Makes the 3 build types in your computer folder:*  
*[ROOT]\build\app\outputs\flutter-apk*

Here is a super-useful article on APK builds:  
https://www.woolha.com/tutorials/flutter-build-android-apk

flutter build apk --no-shrink   
*Still doing research on "no-shrink", but in the mean time here is a related link:*  
https://dev.to/techwithsam/how-to-solve-shrinker-error-in-flutter-2f09

