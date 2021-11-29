Create apps, games, .HTML5 files and fonts for Floflis.

## Common for app/game developers

### Introduction

Pretty simple: just make an Electron app/game (Construct 2/3 or GDevelop recommended).
It is recommended to also make it support Cordova (for doing mobile releases, and for an upcoming/hypothetical mobile version of Floflis).

**Note**: this app/game need to have `electron` as module and support `npm start` command. To guarantee better support, just symlink your `node_modules` to `/1/Floflis/libs/node_modules` (and don't forget to support `electron .` in your `npm start` script at `manifest.json`.

### Detect platform

To support Floflis' features, you can do it by simply detecting if `/1` folder exists.

**Note**: For a more accurate check: detect if `/1/config/user.json` exists or check for `/etc/floflis-release`.

So, you can focus on supporting Floflis without causing confusion on other Linux OSes/platforms (MacOS, Windows' Cygwin/WSL, etc).

### Pin app/game

Floflis Platform package for NPM, soon.

#### Desktop

#### Explore menu

#### Taskbar

### Reading shared libs

When building for Floflis, you can remove any asset that is already included with Floflis, which makes your app smaller for download.

Libraries are in `/1/Floflis/libs`. Root permission will be asked when adding a library, but not when reading.

Common files for Construct 2 are included!

#### Libraries

* FrameworkJS
* Bootstrap
* jQuery
* Popper.js
* UmbrellaJS
* Slick

Todolist is FrameworkJS not having built-in libraries and fonts, but building it depending on target platform (possibly using Plugz).

#### Fonts

Fonts (which are in web format) are stored in `/1/Fonts`.

Included fonts:

* Roboto
* Material Icons
* Text Me One
* Cabin

To read a font, just reference to its `font.css` file.

### Where to save user's files

This guide teaches, for every kind of app/game, where to store files produced by its users.

#### Reading app (draft, outdated)

* Books: `/1/Books`
* Magazines: `/1/Books/Magazines`
* Comics/novels: `/1/Books/Comics`
* MkDocs and other kinds of documentations/manuals: `/1/Books/Manuals`
* Scanned books: `/1/Books/Scanned`
* Other kind of document: `{homefolder}/Documents`
* Scanned documents: `{homefolder}/Documents/Scanned`

#### 3D app (draft, outdated)

This folder isn`t yet very organized, as others. Suggestions and pull requests are welcome.

* Any kind of 3D files: `/1/3D`
* 3D objects: `/1/3D/Objects`
* 3D voxel objects: `/1/3D/Objects/voxels`
* 3D scenes: `/1/3d/scenes`

#### Browsers/code editors/compilers (draft, outdated)

Source-codes should be saved into `/1/sourcecode`.?

Web browsers would also ask to save `.tar.gz` in this folder instead of `{homefolder}/Downloads` folder.?

#### Imaging app (draft, outdated)

Normal images/graphics are stored in `{homefolder}/Pictures`.

* Photos: `/Pictures/Photos`
* Screenshots: `/Pictures/Printscreens`
* Draw: `/Pictures/Drawings`
* Scanned: `/Pictures/Scanned`
* Memes: `/Pictures/Memes`
* GIFs: `/Pictures/GIFs`

#### Video app (draft, outdated)

Normal videos are stored in `{homefolder}/Videos`.

* Series: `/Videos/Series`
* Movies: `/Videos/Movies`
* Documentaries: `/Videos/Documentaries`
* Animations: `/Videos/Animations`
* Animes: `/Videos/Animations/Animes`
* Memes: `/Videos/Memes`

#### Music app (draft, outdated)

Normal music are stored in `{homefolder}/Music`.

* Memes: `/Music/Memes`
* Effect sounds: `/Music/SFX`
* Background music: `/Music/Background`
* Voice notes/recording: `/Music/Voice`

#### Downloads app (draft)

Files that user is seeding are stored in `{homefolder}/Downloads/Seeding` folder.

## App developers

### Where to install it

If your app haves a install script, point it to `/1/apps`.

### Where to install app's user data

Put all app's user data in JSON files inside `/1/config/apps/{your-app-name}` folder.

## Game developers

### Introduction

You can develop games using the Floflis' built-in game engine: GDevelop. But you can use other if you prefer, althought GDevelop is the easiest.

Construct 2 proved to be useful not only for developing professional games, but also apps (Floflis Central is made in Construct 2).

### Where to install it (draft, outdated)

If your game haves a install script, point it to `/1/games`.

### Where to install game's user data

Put all game's user data in JSON files inside `/1/config/games/{your-app-name}` folder.

## .HTML5 file developers

To learn more about what is a HTML5 file, [click here](/floflisfiles/#html5).

Just create a text file with the `.html5` extension, and put its content.

To add a script, add its content inside a `<script>` tag.

To add a CSS is same as previous step, but with `<style>` tag.

<<<<<<< HEAD
Do the same with images, using `base64` format in `<img>` tag or use a inline `<svg>` tag.
=======
Do the same with images, using `base64` format in `<img>` tag or use the `<svg>` tag.
>>>>>>> 00eaafe8877adeef389e7acd16a565c6bb54398b

For `.HTML5` files, it isn't a recommended practice to load external script/css.

## Packaging your font

Floflis uses web format (woff, woff2) for fonts.

Take a inspiration look at `/1/Fonts` folder.

Each font is simply a folder containing the `WOFF` files and the `font.css` file, which looks like that:

```css
/* vietnamese */
@font-face {
  font-family: 'Cabin';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: local('Cabin'), local('Cabin-Regular'), url(cabinregular-vietnamese.woff2) format('woff2');
  unicode-range: U+0102-0103, U+0110-0111, U+1EA0-1EF9, U+20AB;
}
/* latin-ext */
@font-face {
  font-family: 'Cabin';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: local('Cabin'), local('Cabin-Regular'), url(cabinregular-latinext.woff2) format('woff2');
  unicode-range: U+0100-024F, U+0259, U+1E00-1EFF, U+2020, U+20A0-20AB, U+20AD-20CF, U+2113, U+2C60-2C7F, U+A720-A7FF;
}
/* latin */
@font-face {
  font-family: 'Cabin';
  font-style: normal;
  font-weight: 400;
  font-display: swap;
  src: local('Cabin'), local('Cabin-Regular'), url(cabinregular-latin.woff2) format('woff2');
  unicode-range: U+0000-00FF, U+0131, U+0152-0153, U+02BB-02BC, U+02C6, U+02DA, U+02DC, U+2000-206F, U+2074, U+20AC, U+2122, U+2191, U+2193, U+2212, U+2215, U+FEFF, U+FFFD;
}
```

You can simply distribute your fonts as compressed files, althought they aren't automatically installable yet.

## Soon, new developments

These will be available to develop:

* Screensavers
* Themes
* NFT backgrounds and themes (UniStore)
* others

And you will have the possibility to distribute your productions to a decentralized store.
Also, packagers for installing apps, games, fonts and others; and asking to install a .HTML5 file when clicking it.

## Play with

* [Sources](https://floflis.github.io/cli/source/)
