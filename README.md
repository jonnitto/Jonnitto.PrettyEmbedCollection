[![Latest Stable Version](https://poser.pugx.org/jonnitto/prettyembedcollection/v/stable)](https://packagist.org/packages/jonnitto/prettyembedcollection)
[![Total Downloads](https://poser.pugx.org/jonnitto/prettyembedcollection/downloads)](https://packagist.org/packages/jonnitto/prettyembedcollection)
[![License](https://poser.pugx.org/jonnitto/prettyembedcollection/license)](https://packagist.org/packages/jonnitto/prettyembedcollection)
[![GitHub forks](https://img.shields.io/github/forks/jonnitto/Jonnitto.PrettyEmbedCollection.svg?style=social&label=Fork)](https://github.com/jonnitto/Jonnitto.PrettyEmbedCollection/fork)
[![Support development](https://img.shields.io/badge/Donate-PayPal-yellow.svg)](https://www.paypal.me/Jonnitto/20eur)
[![My wishlist on amazon](https://img.shields.io/badge/Wishlist-Amazon-yellow.svg)](https://www.amazon.de/hz/wishlist/ls/2WPGORAVYF39B?&sort=default)  
[![GitHub stars](https://img.shields.io/github/stars/jonnitto/Jonnitto.PrettyEmbedCollection.svg?style=social&label=Stars)](https://github.com/jonnitto/Jonnitto.PrettyEmbedCollection/stargazers)
[![GitHub watchers](https://img.shields.io/github/watchers/jonnitto/Jonnitto.PrettyEmbedCollection.svg?style=social&label=Watch)](https://github.com/jonnitto/Jonnitto.PrettyEmbedCollection/subscription)
[![GitHub followers](https://img.shields.io/github/followers/jonnitto.svg?style=social&label=Follow)](https://github.com/jonnitto/followers)
[![Follow Jon on Twitter](https://img.shields.io/twitter/follow/jonnitto.svg?style=social&label=Follow)](https://twitter.com/jonnitto)

# Jonnitto.PrettyEmbedCollection

The PrettyEmbed series are media player (Video/Vimeo/Youtube) for [Neos CMS](https://www.neos.io) - with nice options like high-res preview images, lightbox feature and advanced customization of embed options.

This package installs following packages:

- [PrettyEmbedVideo](https://github.com/jonnitto/Jonnitto.PrettyEmbedVideo)
- [PrettyEmbedVideoPlatforms](https://github.com/jonnitto/Jonnitto.PrettyEmbedVideoPlatforms)

If you install the PrettyEmbedCollection the video players get grouped into a own group in the node inspector, otherwise they will be in the default group.

## Installation

Most of the time you have to make small adjustments to a package (e.g. configuration in `Settings.yaml`). Because of that, it is important to add the corresponding package to the composer from your theme package. Mostly this is the site packages located under `Packages/Sites/`. To install it correctly go to your theme package (e.g.`Packages/Sites/Foo.Bar`) and run following command:

```bash
composer require jonnitto/prettyembedcollection --no-update
```

The `--no-update` command prevent the automatic update of the dependencies. After the package was added to your theme `composer.json`, go back to the root of the Neos installation and run `composer update`. Et voilà! Your desired package is now installed correctly.

## FAQ

**What are the differences from the PrettyEmbed series to [Jonnitto.Plyr](https://github.com/jonnitto/Jonnitto.Plyr)?**

|                                    | PrettyEmbed series |  Plyr  |
| ---------------------------------- | :----------------: | :----: |
| YouTube Video                      |         ✓          |   ✓    |
| YouTube Playlist                   |         ✓          |        |
| Vimeo                              |         ✓          |   ✓    |
| Native Audio                       |                    |   ✓    |
| Native Video                       |         ✓          |   ✓    |
| Advanced captions for native video |         ✓          |        |
| Preview image                      |         ✓          |        |
| Lightbox included                  |         ✓          |        |
| Preview image                      |         ✓          |        |
| Javascript API                     |                    |   ✓    |
| Filesize (JS & CSS)                |      smaller       | bigger |

All packages from the PrettyEmbed series have the benefit of a better frontend performance since the player gets only loaded on request. So, no iframe/video get's loaded until the user wants to watch a video.
