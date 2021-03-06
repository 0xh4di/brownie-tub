# BROWNIE TUB

[![Known Vulnerabilities](https://snyk.io/test/github/cybersecmoo/brownie-tub/badge.svg?targetFile=package.json)](https://snyk.io/test/github/cybersecmoo/brownie-tub?targetFile=package.json)
![AppVeyor](https://img.shields.io/appveyor/build/cybersecmoo/brownie-tub?label=windows%20build)
![Travis (.com)](https://img.shields.io/travis/com/cybersecmoo/brownie-tub?label=linux%20build)
![GitHub issues](https://img.shields.io/github/issues/cybersecmoo/brownie-tub)

## A Standalone Web Shell Client ##

BROWNIE TUB can support essentially any web shell that is based on commands being passed via HTTP(S).

### FEATURES ###

- Flexible: can support command-passing in any HTTP header, in any cookie, POST parameter, or GET parameter.
- Securable: can integrate with password authentication mechanisms
- Easy-to-Use: simple GUI allows easy control and configuration of your shells
- Persistent: Stores data in an RxDB store (backed by PouchDB)
- Control multiple shells from one app: track as many shells as you'd like, and switch between them seamlessly
- Note that BROWNIE TUB comes with a small set of commands (i.e. read file, change directory) out-of-the-box. Feel free to fork and add more, though.
  - This is because the concept of BROWNIE TUB is to support web shells designed as initial footholds.
  - If your entire campaign is web-shell-based, then you will want to add extra commands, for sure.
  - You could also add an `Issue`, with a label of `Enhancement`, and I'll see if I have time to implement it (around my day job etc. of course)

### Building this Yourself ###

1. Clone this repo
2. Run `npm install` to grab the dependencies
3. Run `npm run rebuild` to rebuild the sqlite3 module, so it works with electron
4. Run `npm run build` to build the react part
5. Run `npm run electron-pack` to package the app.

### Pre-Built Binaries ###

Under `Releases`, there are binaries (`.exe`, `.deb`, `.AppImage`) for Windows and Linux platforms.
