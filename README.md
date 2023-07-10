

https://github.com/andrew-moreno/andys-arc-firefox/assets/46725252/2c3b9cba-c097-4c24-8911-b1a799dd7be0

This Firefox theme draws heavily from [this theme](https://www.reddit.com/r/FirefoxCSS/comments/11vjtat/firefox_in_the_style_of_arc_browser/) but features updated styling and added suport for hiding the sidebar.

# Installation
## Firefox Styling
1. Enter `about:config` in the url bar and search for `toolkit.legacyUserProfileCustomizations.stylesheets`. Change the value to "True".
2. Enter `about:profiles` in the url bar. Open the root directory of the active default profile.
3. Copy the `chrome` folder from this repository into the above profile folder.
4. Restart Firefox to apply the theme.

## Sidebery Installation and Styling
1. Install [Sidebery Beta](https://github.com/mbnuqw/sidebery).
2. Open the Siderbery settings and scroll to the Help section. From here, import the `sidebery-data.json` file by clicking "Import addon data".
    - Alternatively, if this doesn't work, you can apply the custom styling directly by opening the Sidebery Styles Editor and copying the CSS from `sidebery-styles.css`

## Startpage Customization
1. Install [nightTab](https://addons.mozilla.org/en-CA/firefox/addon/nighttab/).
2. Open the nightTab settings and navigate to the "Data" header. import the `nightTab-data.json` file by clicking "Import from file".

### Changing the Startpage Video
- To add your own video to the startpage, you'll have to obtain a URL pointing to your video so that it can be added to nightTab. I uploaded my video to a Discord server to obtain the URL, but imgur or other online upload services would work fine as well.  
- Once you have a URL to your video, navigate to the "Background" section under the "Theme" header within the nightTab settings and paste the URL in the input box.
