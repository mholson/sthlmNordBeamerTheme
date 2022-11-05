# sthlmNord BeamerTheme

<p align="center">
        <a href="https://github.com/mholson/sthlmNordBeamerTheme/raw/main/sthlmNordDarkDemo.pdf">
        <img src="https://img.shields.io/badge/DownloadDarkTheme-pdf-red.svg"/>
</a>
<a href="https://github.com/mholson/sthlmNordBeamerTheme/raw/main/sthlmNordLightDemo.pdf">
        <img src="https://img.shields.io/badge/DownloadLightTheme-pdf-red.svg"/>
</a>
<img src="https://img.shields.io/badge/Compiler-XeLaTeX-blue.svg"/>
<img src="https://img.shields.io/badge/WIP-WorkInProgress-orange.svg"/>
</p>

<p align="center">
    <img src="images/dark/Page 02.png" width="800" max-width="90%" alt="Background" />
</p>

## Other Nord Beamer themes

Maybe you were looking for another Nord Beamer theme?
- [https://github.com/junwei-wang/beamerthemeNord](https://github.com/junwei-wang/beamerthemeNord)

## Light and Dark Mode Available

<p align="center">
    <img src="images/dark/Page 01.png" width="45%" max-width="90%" alt="Background" /> <img src="images/light/Page 01.png" width="45%" max-width="90%" alt="Background" />
</p>

By default, theme will be displayed using dark mode; however, this can easily be toggled to the light version of the theme by providing an option to the `\usetheme{sthlmnord}` command,
```latex 
% > > > Choose Theme
\usetheme[mode=light]{sthlmnord}
%\usetheme{sthlmnord}
```

## Major Features

<p align="center">
    <img src="images/dark/Page 06.png" width="45%" max-width="90%" alt="Background" /> <img src="images/light/Page 06.png" width="45%" max-width="90%" alt="Background" />
</p>

## Nord Color Palette

<p align="center">
    <img src="images/dark/Page 13.png" width="45%" max-width="90%" alt="Background" /> <img src="images/light/Page 13.png" width="45%" max-width="90%" alt="Background" />
</p>

<p align="center">
    <img src="images/dark/Page 14.png" width="45%" max-width="90%" alt="Background" /> <img src="images/light/Page 14.png" width="45%" max-width="90%" alt="Background" />
</p>

<p align="center">
    <img src="images/dark/Page 15.png" width="45%" max-width="90%" alt="Background" /> <img src="images/light/Page 15.png" width="45%" max-width="90%" alt="Background" />
</p>

<p align="center">
    <img src="images/dark/Page 17.png" width="45%" max-width="90%" alt="Background" /> <img src="images/light/Page 17.png" width="45%" max-width="90%" alt="Background" />
</p>

## Block Environments

<p align="center">
    <img src="images/dark/Page 19.png" width="45%" max-width="90%" alt="Background" /> <img src="images/light/Page 19.png" width="45%" max-width="90%" alt="Background" />
</p>

## Lists

<p align="center">
    <img src="images/dark/Page 20.png" width="45%" max-width="90%" alt="Background" /> <img src="images/light/Page 20.png" width="45%" max-width="90%" alt="Background" />
</p>

<p align="center">
    <img src="images/dark/Page 21.png" width="45%" max-width="90%" alt="Background" /> <img src="images/light/Page 21.png" width="45%" max-width="90%" alt="Background" />
</p>

<p align="center">
    <img src="images/dark/Page 22.png" width="45%" max-width="90%" alt="Background" /> <img src="images/light/Page 22.png" width="45%" max-width="90%" alt="Background" />
</p>


## Source Code Syntax Highlighting powered by Listings (default) and Minted

By default, source code printing is done using the listings package.  The reason is that it will be easier to style the code using Overleaf.com in the future.

However, if you would like to use the minted package styled with nord, then just pass the `codeminted` option to the documentclass command.  While minted should work out of the box, this theme includes the custom nord color  palette [https://github.com/sbrisard/nord_pygments](https://github.com/sbrisard/nord_pygments), that needs to be installed (see github repository for instructions).

If you do not want to install the pygements nord color theme, you can choose one of the installed themes by changing the beamerthemesthlmnord.sty file 
```latex
\RequirePackage{minted}
% > > > Nord style Requires custom install: https://github.com/sbrisard/nord_pygments
\usemintedstyle{nord}  <====== Change to a default style 
```

## Libertinus fonts compiled with XeLaTeX

<p align="center">
    <img src="images/dark/Page 28.png" width="45%" max-width="90%" alt="Background" /> <img src="images/light/Page 28.png" width="45%" max-width="90%" alt="Background" />
</p>

## Mathematics

<p align="center">
    <img src="images/dark/Page 30.png" width="45%" max-width="90%" alt="Background" /> <img src="images/light/Page 30.png" width="45%" max-width="90%" alt="Background" />
</p>

<p align="center">
    <img src="images/dark/Page 31.png" width="45%" max-width="90%" alt="Background" /> <img src="images/light/Page 31.png" width="45%" max-width="90%" alt="Background" />
</p>

<p align="center">
    <img src="images/dark/Page 32.png" width="45%" max-width="90%" alt="Background" /> <img src="images/light/Page 32.png" width="45%" max-width="90%" alt="Background" />
</p>

<p align="center">
    <img src="images/dark/Page 33.png" width="45%" max-width="90%" alt="Background" /> <img src="images/light/Page 33.png" width="45%" max-width="90%" alt="Background" />
</p>

# Release Notes

## Version round(pi,5)
- initial Overleaf.com support

## Version round(pi,4)
- **breaking change!** The _codehl_ option has been renamed to _codeminted_.  The Listings pkg will now be the default code printer; however, if you would like to use the minted pkg, then you can provide the _codeminted_ option to the documentclass options.
- moving towards support for use with overleaf.com

## Version round(pi,3)
- removed document class boolean option `enumarabic` to toggle between enumerated lists using (arabic, arabic) and (alpha, roman), (default: alpha, roman)
- removed enumitem pgk as it does not play nicely with Beamer
- updated styles for list environments

## Version round(pi,2)
- enough decimal places to start rounding pi 
- added document class boolean option `bibref` to make bibliography optional (default: false)
- simplified title page commands 
- added release notes
- updating readme file 

## Version 3.1
- added working dark theme such that it works with light theme
- created demo *.tex files for both the light and dark theme (slides included in /0-slides directory) 
- included subfiles package into the theme
- simplified cover page image
- added document class boolean option `codehl` to include code highlighted blocks powered by the minted package and themed using nord pygments, [https://github.com/sbrisard/nord_pygments](https://github.com/sbrisard/nord_pygments) (default: false)
- added document class boolean option `enumarabic` to toggle between enumerated lists using (arabic, arabic) and (alpha, roman), (default: alpha, roman)
- added custom color commands for both text and highlighted text
- new title page inspired from [https://github.com/dennisog/beamer-purdue](https://github.com/dennisog/beamer-purdue) 
- breaking change! mhomath.sty renamed to mhomacros.sty 
- added example and theorem slides styled using awesomefont5 package
- references now working 

## Version 3.0
- color theme now NORD inspired [https://www.nordtheme.com](https://www.nordtheme.com)
- now complied using XeLaTeX as font changed to Libertinus using the libertinus-otf package
- moving towards a light and dark mode version of the deck 
  
