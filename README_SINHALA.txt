My English Dictation - Android Studio project
----------------------------------------------
මෙය දැනට test කළ Grade 4 browser app එක Android WebView app එකක් ලෙස package කිරීමට සකස් කළ project එකකි.

APK build කරන ආකාරය:
1. Android Studio install කර open කරන්න.
2. File > Open තෝරා මෙම ZIP extract කළ MyEnglishDictation folder එක open කරන්න.
3. Gradle Sync අවසන් වන තුරු ඉන්න.
4. Android SDK Platform 35 සහ Build Tools අවශ්‍ය නම් Android Studio SDK Manager හරහා install කරන්න.
5. Build > Build Bundle(s) / APK(s) > Build APK(s) තෝරන්න.
6. APK එක app/build/outputs/apk/debug/app-debug.apk යටතේ ලැබේ.

සටහන්:
- App එක offline HTML asset එකක් ලෙස load වේ.
- JavaScript, local storage, Web Audio සහ browser speech synthesis enabled.
- Sinhala pronunciation hints හා voice accent availability device එකේ installed English voices මත රඳා පවතී.
- Level progress එම phone එකේ local storage තුළ save වේ.
- මෙය source project එකකි; APK එක මෙහි compile කර නැත. Build සඳහා Android SDK සහ Gradle අවශ්‍යයි.


ONLINE APK BUILD (GitHub Actions)
---------------------------------
මෙම project එකේ .github/workflows/build-apk.yml workflow එක සකස් කර ඇත.
1. GitHub account එකකින් NEW repository එකක් සාදන්න.
2. ZIP එක extract කර ඇති project folder එකේ ඇතුළත files/folders සියල්ල repository එකට upload කරන්න.
   (root එකේ settings.gradle, build.gradle, app/ සහ .github/ තිබිය යුතුය.)
3. Commit changes කරන්න. GitHub Actions tab එකට ගොස් workflow run එක බලන්න.
4. Build සාර්ථක නම් run එකේ Artifacts යටතේ My-English-Dictation-debug-apk.zip download කරන්න.
5. ZIP එක extract කර app-debug.apk Android phone එකට copy කර install කරන්න.

Public repository එකක standard GitHub-hosted runner usage free බව GitHub දක්වයි.
Private repository එකක Free account එකට monthly included minutes සීමාවක් ඇත.
Repository public කරන විට source code එක ඕනෑම කෙනෙකුට පෙනෙන බව මතක තබාගන්න.
