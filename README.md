AGS-wrapper-scrollbars
======================

> [AutoIt Gui Skeleton](https://autoit-gui-skeleton.github.io/) package for wrapping the library [Scrollbars](https://www.autoitscript.com/forum/topic/113723-scrollbars-made-easy-bugfix-version-2-may-21/) created by Melba23. See this package on [npmjs.com](https://www.npmjs.com/package/@autoit-gui-skeleton/ags-wrapper-scrollbars/)



<br/>

## Scrollbars

**GUIScrollbars_Ex.au3** - This gives you scrollbars sized to your GUI in one simple command - with no other includes or commands needed. The UDF is designed for those who would not normally use scrollbars because the whole process looks too complicated. It also includes a command to enable you to scroll page by page, thus making it easy to scroll to anywhere on the GUI with only simple calulations based on the values you used to create the GUIs. New ability to have recalculated scrollbars on resizeable GUIs.

**GUIScrollbars_Size.au3** - This calculates the Page and Max numbers for the user to feed into the _GUIScrollbar_SetScrollInfoPage/Max commands. The UDF is aimed at the more experienced user and is particularly useful when you have a GUI with a dynamic scroll size (i.e. adding or subtracting controls to the scrollable area as the script runs).

<br/>

## How to install AGS-wrapper-wrapper-scrollbars ?

We assume that you have already install [Node.js](https://nodejs.org/) and [Yarn](https://yarnpkg.com/lang/en/), for example by taking a [Chocolatey](https://chocolatey.org/). AGS framework use Yarn for manage dependencies.

To add this package into your AutoIt project, just type in the root folder of your AGS project where the `package.json` is stored. You can also modify the `dependencies` property of this json file and use the yarn [install](https://yarnpkg.com/en/docs/usage) command. It is easier to use the add command :

```
λ  yarn add @autoit-gui-skeleton/ags-wrapper-scrollbars --modules-folder vendor
```

The property `dependencies` of the  `package.json` file is updated consequently, and all package dependencies, as well as daughter dependencies of parent dependencies, are installed in the `./vendor/@autoit-gui-skeleton/` directory. Note that with an AGS project, it is not necessary to explicitly write this option `--modules-folder vendor` on the command line, thanks to the `.yarnrc` file stored at the root of the project. Yarn automatically use `.yarnrc` file to add an additional configuration of options.

```
 #./.yarnrc
 --modules-folder vendor
 ```

Finally to use this library in your AutoIt program, you need to include this library in the main program. There is no need for additional configuration to use it.


```autoit
#include './vendor/@autoit-gui-skeleton/ags-wrapper-scrollbars/GUIScrollBars_Ex.au3'
#include './vendor/@autoit-gui-skeleton/ags-wrapper-scrollbars/GUIScrollBars_Size.au3'
```

Or you can add `Scrollbars.au3` to add this two libraries simultaneous :
```autoit
#include './vendor/@autoit-gui-skeleton/ags-wrapper-scrollbars/Scrollbars.au3'
```


<br/>

## What is AGS (AutoIt Gui Skeleton) ?

[AutoIt Gui Skeleton](https://autoit-gui-skeleton.github.io/) give an environment for developers, that makes it easy to build AutoIt applications. To do this AGS proposes to use conventions and a standardized architecture in order to simplify the code organization, and thus its maintainability. It also gives tools to help developers in recurring tasks specific to software engineering.

> More information about [AGS framework](https://autoit-gui-skeleton.github.io/)

AGS provides a dependency manager for AutoIt library. It uses the Node.js ecosystem and its dependency manager npm and its evolution Yarn. All AGS packages are hosted in npmjs.org repository belong to the [@autoit-gui-skeleton](https://www.npmjs.com/search?q=autoit-gui-skeleton) organization. And in AGS you can find two types of package :

- An **AGS-component** is an AutoIt library, that you can easy use in your AutoIt project built with the AGS framework. It provides some features for application that can be implement without painless.
- An **AGS-wrapper** is a simple wrapper for an another library created by another team/developer.

> More information about [dependency manager for AutoIt in AGS](https://autoit-gui-skeleton.github.io//2018/07/10/ags_dependencies_manager_for_AutoIt.html)


<br/>

## About

### Acknowledgments

Acknowledgments for [Melba23](https://www.autoitscript.com/forum/topic/113723-scrollbars-made-easy-bugfix-version-2-may-21/) and contributions from rover, czardas, MrCreatoR, Malkey and KaFu for this scrollbars librairies.

### Contributing

Comments, pull-request & stars are always welcome !

### License

Copyright (c) 2018 by [v20100v](https://github.com/v20100v). Released under the MIT license.
