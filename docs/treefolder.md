**Note**: this documentation is yet a draft, as Floflis Core isn't available yet.

## Introduction
Maybe you know how the Windows folders are well organized; on contrary of Linux, MacOS and Android.

As root represents the complex structure of a tree, Floflis implemented the tree folder above the root.

**Let the root be used by nerds, and the tree for common users**.

## The tree folder

![](img/screen/treefolder/treeinroot.png)

Tree is a folder named "1" inside the root directory.

While root address is referred as `/`, the tree is `/1`.

Referring to Linux, tree is equivalent to `/home` folder, with write access granted to current user. But unlike on Linux, Floflis is made for personal device with a main user instead of multiple users. On newer versions Floflis will support multiple users with use of authorizations and pendrives.

**Why not to use `/home` folder instead**? Because it is a mess.

## Subfolders

![](img/screen/treefolder/thetree.png)

Some folders are original of tree, but others are symlinked (special shortcuts) from `/home` folder.

Also the root is accessible from tree, in the symlinked `Z-root` folder.

### /1/apps

![](img/screen/treefolder/treeapps.png)

`/1/Apps` folder contains all user apps.

Only HTML5 apps are added to this folder. Usually they are Electron apps.

### /1/programs

![](img/screen/treefolder/tree-apps-old.png)

This folder contains classical apps (that aren't in HTML5) and locally installable.

Other Linux/Debian/Ubuntu apps are also installable, without depending on this folder.

### /1/games

Contains HTML5 games.

### /1/html5

Contains HTML5 files. They can be simple applications or games.

### /1/personal

Subfolders:

#### profile

User's personal profile (Dat, Ethereum).

#### site

User's personal site.

#### blog

User's personal blog, using Hugo.

#### data

Contains `tasks` and `issues` subfolders.

#### badges

Contains user's open badges.

#### projects

User's personal projects.

#### token

User's personal token (Ethereum).

### /1/books

Contains user's books, in any format.

Subfolders:

* `/magazines`
* `/comics`
* `/manuals` (preferrably MkDocs format, but can have others such as PDF)
* `/scanned`

### /1/orgs

Contains user's organizations (Aragon).

### /1/3d

Contains 3D things from user. This folder isn't yet very organized, as others. Suggestions and pull requests are welcome.

Subfolder:

* `/objects`

### /1/libraries

Libraries that user will only use indirectly or sometimes.

Subfolders:

#### /1/libraries/fonts

Contains user's fonts to be used on sites, slide presentations and other writings.

These fonts are in web format (woff, woff2).

#### /1/libraries/replic

De-duplication of files, having only one symlinked in any place it need. Can be used by Dat and IPFS.

### /1/src

Contains downloaded source codes user want to compile.

### /1/config

![](img/screen/treefolder/treeconfig.png)

Contains all settings that Floflis and other HTML5 apps would need. `Apps` and `Games` subfolders contains these data.

A example of contents inside `dat.json`:

```json
{
"type":"config/os",
"url":{},
"lang":"en-us",
"title":"Floflis Settings - floflis",
"user":"floflis"
}
```

### /1/Floflis

![](img/screen/treefolder/treefloflisfolder.png)

It's system folder. Haves folders like the tree (`apps`, `html5`, `programs`, `fonts`), except its `/system` and `/libs` folder. There isn't `/games` folder because they should be easily uninstallable.

![](img/screen/treefolder/treeresources.png)

![](img/screen/treefolder/treeresources-sounds.png)

![](img/screen/treefolder/treeresourcesimg.png)

`/libs` folder contains [shared libs from Floflis](/dev/#reading-shared-libs) and system's `fonts` subdirectories.

## Symlinked folders

### /1/Z-root

Magic folder giving access to root from tree.

### /1/desktop

The same desktop displayed when you login, and as other symlinks, same from `/home` folder.

### /1/documents

Contains a new subfolder made by Floflis: `/scanned`.

### /1/images

Compared to Linux it contains new subfolders:

* `/photos`
* `/printscreens` (a friendly meaning for non-english languages)
* `/drawings`
* `/scanned`
* `/memes`
* `/gifs`
* `/icons`

### /1/music

New subfolders:

* `/memes`
* `/sfx`
* `/background`
* `/voice`

### /1/videos

New subfolders:

* `/series`
* `/movies`
* `/documentaries`
* `/animations` (contains the `/animes` subfolder)
* `/memes`

### /1/downloads

New subfolders:

* `/seeding` (downloaded files you're seeding on P2P network)

### /1/templates

Simple symlink, no added subfolders. Suggestions are welcome.

## Useful links

* <a href="https://github.com/Floflis/Floflis-linux_x86/issues/58" target="blank">Discussion that introduced tree folder</a>
