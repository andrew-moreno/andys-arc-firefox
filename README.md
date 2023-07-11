

https://github.com/andrew-moreno/andys-arc-firefox/assets/46725252/2c3b9cba-c097-4c24-8911-b1a799dd7be0

This Firefox theme draws heavily from [Firefox in the style of Arc Browser](https://www.reddit.com/r/FirefoxCSS/comments/11vjtat/firefox_in_the_style_of_arc_browser/) but features updated styling and added suport for hiding the sidebar.

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

## Customizing This Theme
### Changing Sidebar Orientation
Moving Sidebery from one side of the screen to the other must be done in two steps: moving the sidebar itself which is done within Firefox and updating certain theme components which is done by updating the imported styles in the `userChrome` file.
1. Disable the `chrome` folder by renaming it to anything else. This will disable the theme and revert Firefox back to it's default state.
2. Restart Firefox and click the dropdown at the top of the Sidebery sidebar. Here, you should find a menu item that switches the sidebar from one side of the screen to the other.
3. Re-enable the `chrome` folder by changing it's name back to "chrome".
---
4. Open `userChrome.css` in the `chrome` folder and, at the top of the file, adjust the sidebar and caption imports to reflect the side of the screen you want Sidebery to be on.
     - for example, if I wanted Sidebery on the right, I would change `@import url(sidebar-orientation/sidebar-left.css);` to `@import url(sidebar-orientation/sidebar-right.css);` and `@import url(captions/custom-captions-left.css);` to `@import url(captions/custom-captions-right.css);`
5. Restart Firefox to apply the changes. 

### Caption Customization
- I've included a handful of options that disable/enable the close, max, and min buttons as well adjust their appearance.
- The "custom-captions" options contain buttons that pair with [Dracula for Windows 10 by niivu](https://www.deviantart.com/niivu/art/Dracula-for-Windows-10-843182521).
- To apply any of these themes, adjust the imports within the `userChrome.css` file similar to changing the sidebar orientation.

### Panel Icons
I am using [Lumicons](https://www.deviantart.com/vantler/art/Lumicons-662277185) for the panel icons shown in the video above. Custom icons can be applied within the Sidebery settings under the "Navigation Bar" section. 
