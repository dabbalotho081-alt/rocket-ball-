# Rocket Ball – iOS app

Wraps the Rocket Ball 3D HTML game in a native iOS app (full screen, landscape, touch controls).

## Get the .ipa without a Mac (free, via GitHub)
1. Create a new GitHub repository and upload everything in this folder (including the hidden `.github` folder).
2. Open the repo's **Actions** tab. The "Build IPA" workflow runs automatically (or press **Run workflow**).
3. When it finishes (~5 min), open the run and download **RocketBall-ipa** → unzip → `RocketBall-unsigned.ipa`.
4. Install it on your iPhone with **Sideloadly** or **AltStore** (Windows/Mac). They sign it with your Apple ID.
   With a free Apple ID the app must be re-signed every 7 days.

## Build on a Mac with Xcode
    brew install xcodegen
    xcodegen generate
    open RocketBall.xcodeproj
Pick your Team under Signing & Capabilities, plug in your iPhone, press Run.

## Updating the game
Replace `RocketBall/www/index.html` with the new HTML and rebuild.
