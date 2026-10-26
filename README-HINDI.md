# LUXORA Android Project — Simple Hindi Guide

Yeh ZIP LUXORA 2.3 HTML preview ko ek basic Android WebView app ke andar kholta hai. Isse APK GitHub Actions se build kiya ja sakta hai. Yeh APK build setup hai; abhi compile/test result ka daawa nahi hai.

## Tablet par upload karne ke steps
1. ZIP ko download karke extract karna zaroori nahi agar GitHub web upload extracted files accept na kare; sabse aasaan tareeka hai ZIP extract karna kisi Android file manager se.
2. Browser mein apni private repository kholo: https://github.com/princeraj14s/LUXORA
3. `Add file` → `Upload files` chuno.
4. ZIP ko seedha upload mat karna. ZIP extract karke uske andar ke files/folders upload karo: `.github`, `app`, `build.gradle`, `gradle.properties`, `settings.gradle`, `README-HINDI.md`.
5. Commit changes dabao.
6. Repository ke `Actions` tab mein `Build LUXORA APK` workflow kholna. Agar push se automatic run na ho, workflow ko `Run workflow` dabakar start karo.
7. Green successful run kholna → neeche `Artifacts` mein `LUXORA-debug-APK` download karo.
8. Download ZIP ko extract karo; usmein `app-debug.apk` hoga. APK ko tap karke install karo. Android pooche toh browser/file manager ko “Install unknown apps” permission deni pad sakti hai.

## Important sachchai
- `app/src/main/assets/index.html` LUXORA 2.3 preview par based hai.
- Android shell HTML ko app ke andar dikhata hai. Iska matlab yeh nahi ki har preview button native Android par automatically kaam karega.
- Wallpaper ko system wallpaper banana, ringtone ko system ringtone set karna, payments, real icon-pack installation aur premium unlocks ke liye extra native integrations aur testing chahiye. Preview ke demo/placeholder actions ko real feature na samjhein.
- Build fail ho toh Actions ke red run ka error text copy karke share karna; uske hisaab se fix hoga.
