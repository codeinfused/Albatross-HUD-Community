<div id="top"></div>
<!--
*** Thanks for checking out the Best-README-Template. If you have a suggestion
*** that would make this better, please fork the repo and create a pull request
*** or simply open an issue with the tag "enhancement".
*** Don't forget to give the project a star!
*** Thanks again! Now go create something AMAZING! :D
-->



<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![Twitch][twitch-shield]][twitch-url]



<!-- PROJECT LOGO -->
<br />
<div align="center">
  <a href="https://github.com/codeinfused/Albatross-HUD-Community">
    <img src="images/albatross-logo-wide.png" alt="Logo" style="width:600px; max-width:80%;">
  </a>

  <h3 align="center">Albatross HUD Community Edition</h3>

  <p align="center">
    A customizable piloting HUD skin for Dual Universe!
    <br />
    <a href="https://twitch.tv/codeinfused">Watch a Demo</a>
    ·
    <a href="https://github.com/codeinfused/Albatross-HUD-Community/issues">Report Bug</a>
  </p>
</div>



<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li><a href="#about-albatross-hud">About the HUD</a></li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#file-install">File Install</a></li>
        <li><a href="#linking-elements">Linking Elements</a></li>
        <li><a href="#activating-the-hud">Activating the HUD</a></li>
      </ul>
    </li>
    <li>
      <a href="#usage">Usage</a>
      <ul>
        <li><a href="#learning-the-keys">Learning the Keys</a></li>
        <li><a href="#changing-default-settings">Changing Default Settings</a></li>
        <li><a href="#recommended-hud-colors">Recommended HUD Colors</a></li>
        <li><a href="#grouping-fuel-types">Grouping Fuel Types</a></li>
      </ul>
    </li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
  </ol>
</details>



<!-- ABOUT ALBATROSS HUD -->
## About Albatross HUD
![HUD Screenshot][product-screenshot]

This piloting HUD for Dual Universe is designed for players of all experience levels. It's a visual improvement over the default, adding new features and flight controls to assist both new players and veterans. Our goal with this release is make sure everyone has access to an easy-to-use HUD and make their Dual Universe experience a little better.

_Some Key Features:_
* Visible key mappings for controls, which reflect your actual key maps
* Condensed improved visual with all the most relevant flight data in one spot
* Automatic planet/moon detection with data on braking time needed and atmo entrance
* Groupable fuel gauges, assign custom categories to your fuel types
* Navball display in atmo for pitch and roll
* Customizable colors and opacity

_What This HUD Isn't:_
* Not an autopilot; I recommend SagaHUD or ArchHUD for autopilot controls
* Not advanced; this hud is designed with new players in mind to help support DU
* Not pvp; while you can link weapons, the HUD does not support them natively

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

_This HUD is delivered by "autoconf", a feature supported by Dual Universe for custom scripts. You will need to download a file as instructed below to add this HUD to your game's list._

### File Install

Download the zipped autoconf file from this repo, (right-click this link and "Save link as") [ais_albatross_hud][download-url]

Unzip this, and move the `.conf` file into the game's autoconf custom folder below. The "ProgramData" folder may be hidden, but if you copy this path and paste it into a File Explorer window, that will still open the folder.

For Steam's game client:
`C:\Program Files (x86)\Steam\steamapps\common\Dual Universe\data\lua\autoconf\custom`

For NQ's game client:
`C:\ProgramData\Dual Universe\Game\data\lua\autoconf\custom\`

After extracting the file, make sure the "ais_albatross_hud_#_#_#" conf file is in the `custom` folder directly, and not inside a subfolder! Next you'll just need to activate it in-game.

### Linking Elements

For the most part, you won't need link anything! Almost all needs become linked automatically, with the exception of optional radars. You can link multiple radars to your seat before activating the HUD. If you use "Rename Element" on each radar, the HUD will bring in their custom names.

### Activating the HUD

_If you add new links (like radars), you will need to re-activate the HUD again with these steps also._

1. Make sure you've installed the file from above ^
2. Right-click on your hoverseat, command seat, or whatever flight unit
3. Select "Advanced", then "Update custom autoconf list"
4. Select "Advanced", "Run custom autoconf"
5. Select Albatross HUD from the list
6. That's it! Hop in the seat and enjoy

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- USAGE -->
## Usage

### Learning The Keys

Albatross HUD mostly follows the same default key bindings. However, I still recommend taking some time and looking at the button controls of the HUD before you fly. For example, holding `ALT` with `CTRL` (brakes) will lock the brakes, so that you can release both keys and still have the brakes active. Pressing `G` will either raise you to hover height, or lower you back down to the ground.

`A:2` means Alt+2, and<br/>
`AS:2` means Alt+Shift+2

Other Hotkeys:

1. `AS:8` :: Enable/disable the burn speed and re-entry limiter
2. `AS:9` :: Hide/show the build helper bar
3. `S:L` :: Toggle headlights

#### Lua Tab Commands:
In the chat window, open the Lua tab and type `help` to get a list of commands you can run here, for example setting a specific AGG singularity, or setting a specific altitude to fly at. Some helpful examples:

1. `altitude 2200`
2. `agg 14000`
3. `time 152.8`
4. `align thades`
5. `align pro`
6. `align ::pos{0,0,13856701.7693,7386301.6554,-258251.0307}`

### Changing Default Settings

This HUD has several settings you can modify. Some are customizations like the HUD color, opacity, scale, and FPS rate. Others are key flight mechanics such as the Talent upgrade levels your ship has. If you're not familiar with talents yet, Then you can assume 0 for these (the default).

1. Right-click on your flight unit (seat)
2. Select "Advanced"
3. Select "Edit Lua Parameters"
4. Hover over the label to see a description of each option

### Recommended HUD Colors

Using the steps above, you can change the base color palette of the HUD. I've provided some suggestions below that look best with the HUD's format:

| Name              | Color Code | 
| ----------------- | ---------- |
| Default Albatross | '#4992CF'  |
| Dark Mode         | '#555555'  |
| Light Mode        | '#e9e9e9'  | 
| Tan               | '#736f72'  |
| Blue Steel        | '#546a7b'  |
| Browncoat         | '#bc6c25'  |
| Military          | '#656d4a'  |
| Pink              | '#b5838d'  |
| Mauve             | '#4a4e69'  |
| Plum              | '#706677'  |
| Royal             | '#8452B7'  |
| Nature            | '#6a994e'  |
| Hacker            | '#006400'  |
| Vampire           | '#590d22'  |
| Rose Gold         | '#846267'  |
| Sandstone         | '#ec7d10'  |

### Grouping Fuel Types

The HUD will automatically group your fuel tanks into single displays based on fuel type.. Atmo, Space, or Rocket. However, you can customize these groupings. For example, if you have some fuel tanks that are dedicated to just hover engines or vertical boosters, then you may want to see that in it's own grouping.

For this, you'll only need to rename the tanks you want to specifically group together. To rename, you'll first need to enter Build Mode `(B)`, and right-click to Rename. Most fuel tanks have a default that looks like:

`Space Fuel Tank s [52]`

The " s " stands for small, and is needed by the HUD in the current version. But here's an example of what we could rename to:

`Space Tank s (vboost) [52]`

By adding parethesis and a category, all fuel tanks with a matching parenthesis will be grouped, and you can create as many groupings as you like.



<!-- CONTACT -->
## Contact

_While I do love Dual Universe and its community, I also have very little free time typically. I will try to answer questions via Discord, or if you catch me online on Twitch. But keep in mind this is a free resource, and I've spent a good chunk of time on it, so please be constructive and kind :)_

Discord: [Albatross HUD on DU-OSI](https://discord.gg/EThSxMGXBg)

Twitch: [Watch CodeInfused on Twitch](https://twitch.tv/codeinfused)<br/>
_I go online at pretty random times, so if you'd like to catch my streams, just go here and hit Follow_

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- CONTRIBUTING -->
## Contributing

Contributions will be welcome in a future version of the HUD with more advanced features. This community version is intended to stay simple and support a new playerbase coming into the game for the first time, and for players who enjoy a condensed but rich HUD experience. New features will only be considered for this version if they stay in line with that concept.

Use the Discord above if you'd like to give feedback or suggest a simple feature addition.

<p align="right">(<a href="#top">back to top</a>)</p>



<!-- LICENSE -->
## License

Distributed under the GNU GPLv3 license. See `LICENSE.txt` for more information.

<p align="right">(<a href="#top">back to top</a>)</p>




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[download-url]: https://github.com/codeinfused/Albatross-HUD-Community/raw/main/ais_albatross_hud_2_2_0.zip
[contributors-shield]: https://img.shields.io/github/contributors/codeinfused/Albatross-HUD-Community.svg?style=plastic
[contributors-url]: https://github.com/codeinfused/Albatross-HUD-Community/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/codeinfused/Albatross-HUD-Community.svg?style=plastic
[forks-url]: https://github.com/codeinfused/Albatross-HUD-Community/network/members
[stars-shield]: https://img.shields.io/github/stars/codeinfused/Albatross-HUD-Community.svg?style=plastic
[stars-url]: https://github.com/codeinfused/Albatross-HUD-Community/stargazers
[issues-shield]: https://img.shields.io/github/issues/codeinfused/Albatross-HUD-Community.svg?style=plastic
[issues-url]: https://github.com/codeinfused/Albatross-HUD-Community/issues
[license-shield]: https://img.shields.io/github/license/codeinfused/Albatross-HUD-Community.svg?style=plastic
[license-url]: https://github.com/codeinfused/Albatross-HUD-Community/blob/master/LICENSE.txt
[twitch-shield]: https://img.shields.io/badge/twitch-live-red?logo=twitch&style=social
[twitch-url]: https://twitch.tv/codeinfused
[product-screenshot]: images/screenshot.png
