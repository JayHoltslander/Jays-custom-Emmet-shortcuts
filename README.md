# Jays-custom-Emmet-shortcuts

Extend Sublime/Emmet's functionality with these useful Emmet shortcuts (abbreviations).

## How to install
In Sublime, select **Preferences** > **Package Settings** > **Emmet** > **Settings - User** and paste the contents of ``Emmet.sublime-settings`` in there. Or alternatively overwrite your `` ~/⁨Library/Application Support/Sublime Text 3⁩/⁨Packages/User/Emmet.sublime-settings`` file with this one.

## How to use
After installing simply type any of the below abbreviation triggers and press **tab**

## Includes:

### imglazy
An improvement over the standard ``img`` trigger. Includes [Chrome's native lazy loading](https://web.dev/native-lazy-loading/), width, and height attributes. Far more useful than the default ``img`` trigger.

![](img/imglazy.gif)

``img[loading='lazy' width='256px' height='256px' src='https://placehold.it/256/jpg?text=JPG+256']``

### pic
Insert a picture element with multiple placeholder sources. Far more useful than the default ``picture`` trigger.

![](img/pic.gif)

``picture>source[type='image/webp' srcset='https://placehold.it/256/webp' media='(min-width: $@100px)']*3+imglazy``

### webp
Insert a placeholder [.webp image](https://developers.google.com/speed/webp) (with jpg fallback) using the picture element.

![](img/webp.gif)

``picture>source[type='image/webp' srcset='https://placehold.it/256/webp']+source[type='image/jpg' srcset='https://placehold.it/256/jpg']+imglazy``

### youtube
Instant embed code for [Paul Irish's Lite YouTube Embed](https://github.com/paulirish/lite-youtube-embed)

![](img/youtube.gif)

``c{LITE YOUTUBE EMBED - SEE: https://github.com/paulirish/lite-youtube-embed}+link[rel='stylesheet' href='node_modules/lite-youtube-embed/src/lite-yt-embed.css']+script[src='node_modules/lite-youtube-embed/src/lite-yt-embed.js']+lite-youtube[videoid='ogfYd705cRs']``

## Bootstrap Shortcuts
Misc. bootstrap snippets have been included to make page building a task that takes seconds instead of minutes.

### Try:
* b4-boilerplate
* b4-container
* b4-jumbotron
* br-cols3

## Shout out
Hat tip to [@OdatNurd](https://github.com/OdatNurd) for guiding me towards figuring out how to modify default autocompletion behavior.
