## <img alt="" width="25" src="https://user-images.githubusercontent.com/81589530/112990759-b1c37300-9166-11eb-9f6f-0dc6a8d60238.png"> Firefox  UI regression mending

Fix Firefox UI regressions with css and provide patches for adjusting the look and feel of the Firefox interface to your liking.

Tweaks include:
- Fixing megabar popout
- Bringing back the sweet error page illustrations
- Adding back icons to the hamburger and context menus
- Reverting some aspects of the Proton design change to Photon style

Overall I aim to make this a collection, so I may also include files from others, properly licensed. If you have any concerns over your work being used, please contact me.

*Note:* Stylesheets are currently only tested with Windows 10.

# How to use

#### 1. Set the preference to load stylesheets
Go to `about:config` and set the pref `toolkit.legacyUserProfileCustomizations.stylesheets` to **`true`**.

#### 2. Create the css files
Go to `about:support` and click on the button "Open folder" besides `Profile folder` .

In the profile folder, create a new folder called "chrome" and create two new files `userChrome.css` and `userContent.css` in there.

#### 3. Importing styles from this repository
You can import the stylesheets with an @-rule import like this:

:warning: Always place your imports on top of the css file


```css
@import url("path/filename.css");
```

Make sure to differentiate if the file was made for `userContent.css` or `userChrome.css`, I have seperated them in to their respective folders `chrome` and `content`.
