SUDOKU APP (installable web app / PWA)

OPTION 1 - Install on your phone (easiest, no app store)
1. Upload this whole folder to any free HTTPS host:
   Netlify Drop (app.netlify.com/drop), GitHub Pages, Vercel or Cloudflare Pages.
2. Open the site link on your phone.
   Android (Chrome): menu > Install app / Add to Home screen.
   iPhone (Safari): Share > Add to Home Screen.
3. It opens full-screen like a normal app and works offline after the first load.

OPTION 2 - Build an APK / App Store app (needs a computer)
Install Node.js and Android Studio, then in this folder run:
   npm init -y
   npm i @capacitor/core @capacitor/cli @capacitor/android
   npx cap init Sudoku com.example.sudoku --web-dir .
   npx cap add android
   npx cap sync
   npx cap open android     (then Build > Build APK in Android Studio)
For iOS use @capacitor/ios and Xcode on a Mac.
