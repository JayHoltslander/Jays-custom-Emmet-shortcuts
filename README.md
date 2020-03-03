# Jays-custom-Emmet-shortcuts

Extend Sublime/Emmet's functionality with these useful Emmet abbreviations.

## How to install
In Sublime, select **Preferences** > **Package Settings** > **Emmet** > **Settings - User** and paste the contents of ``Emmet.sublime-settings`` in there. Or alternatively overwrite your `` ~/⁨Library/Application Support/Sublime Text 3⁩/⁨Packages/User/Emmet.sublime-settings`` file with this one.

## How to use
After installing simply type any of the below abbreviation triggers and press **tab**

## Includes:

### imglazy
An improvement over the standard ``img`` trigger. Includes [Chrome's native lazy loading](https://web.dev/native-lazy-loading/), width, and height attributes. Far more useful than the default ``img`` trigger.

``img[loading='lazy' width='256px' height='256px' src='https://placehold.it/256/jpg?text=JPG+256']``

### pic
Insert a picture element with multiple placeholder sources. Far more useful than the default ``picture`` trigger.

``picture>source[type='image/webp' srcset='https://placehold.it/256/webp' media='(min-width: $@100px)']*3+imglazy``

### webp
Insert a placeholder [.webp image](https://developers.google.com/speed/webp) (with jpg fallback) using the picture element.

``picture>source[type='image/webp' srcset='https://placehold.it/256/webp']+source[type='image/jpg' srcset='https://placehold.it/256/jpg']+imglazy``

### youtube
Instant embed code for [Paul Irish's Lite YouTube Embed](https://github.com/paulirish/lite-youtube-embed)

``c{LITE YOUTUBE EMBED - SEE: https://github.com/paulirish/lite-youtube-embed}+link[rel='stylesheet' href='node_modules/lite-youtube-embed/src/lite-yt-embed.css']+script[src='node_modules/lite-youtube-embed/src/lite-yt-embed.js']+lite-youtube[videoid='ogfYd705cRs']``

### columns
Creates a row with 1-4 nested column(s). Useful for Bootstrap or some other css framework.

#### columns1
``.row>.col.s12.m12``

#### columns2
``.row>.col.s6.m6*2``

#### columns3
``.row>.col.s4.m4*3``

#### columns4
``.row>.col.s3.m3*4``

## Shout out
Hat tip to [@OdatNurd](https://github.com/OdatNurd) for guiding me towards figuring out how to modify default autocompletion behavior.
