# Rocket Ball 3D — iOS

The Rocket Ball 3D HTML game packaged as a native iOS app (WKWebView wrapper).

## Get the IPA
- the **`release` branch** — it holds only `RocketBall.ipa`, updated after every build on `main`, or
- the **Releases** page (`build-N` tags), or
- **Actions → Build IPA → latest run → Artifacts**.

The IPA is **unsigned**. Install it with a sideloading tool (AltStore, Sideloadly, TrollStore, etc.),
which signs it with your Apple ID.

## Layout
| Path | What |
|---|---|
| `RocketBall/www/index.html` | The game |
| `RocketBall/www/three.min.js` | three.js r128, bundled so the game runs offline |
| `RocketBall/AppDelegate.swift` | App + full-screen WKWebView |
| `RocketBall/Info.plist` | App metadata |
| `RocketBall/Assets.xcassets` | App icon |
| `project.yml` | XcodeGen project spec |
| `.github/workflows/build-ipa.yml` | macOS build → IPA → GitHub Release + `release` branch |

## Rebuild
Push any change, or run **Actions → Build IPA → Run workflow**.
