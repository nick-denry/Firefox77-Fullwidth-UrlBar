# Disable Firefox 77 megabar and enable fullwidth UrlBar dropdown

<img src="https://user-images.githubusercontent.com/1450983/83911524-172c1a80-a775-11ea-9ec9-da77c98b8a5e.png" alt="Full width address bar" width="600" />

## 1. Setup

#### 1.1. Enable user profile stylesheets

Open Firefox configuration editor by typing `about:config` in the address bar and press `Enter`

At  `search preference name` type-in `toolkit.legacyUserProfileCustomizations.stylesheets` and set the preference to `true`

![Enable user stylesheets](https://user-images.githubusercontent.com/1450983/83911597-375bd980-a775-11ea-9696-17a005c4398e.png)


#### 1.2. Create `chrome` directory under your Firefox profile

Follow this guide to open your profile directory https://support.mozilla.org/en-US/kb/profiles-where-firefox-stores-user-data or use default profile placement:

| Operation System | Path |
------------|--------------
| Windows | C:\Users\<username>\AppData\Roaming\Mozilla\Firefox\Profiles\xxxxxxxx.default |
| macOS | Users/<username>/Library/Application Support/Firefox/Profiles/xxxxxxxx.default |
| Linux | /home/<username>/.mozilla/firefox/xxxxxxxx.default |

#### 1.3. Place userChrome.css to Firefox profile `chrome` folder

Download stylesheet

| Operation System | Link |
------------|--------------
Windows     | [userChrome.css](https://raw.githubusercontent.com/nick-denry/Firefox77-Fullwidth-UrlBar/master/userChrome.css) |
Other       | [userChrome-linux-mac.css](https://raw.githubusercontent.com/nick-denry/Firefox77-Fullwidth-UrlBar/master/userChrome-linux-mac.css) |

**Note:** `userChrome-linux-mac.css` must be renamed to `userChrome.css` before placement to `firefox-profile/chrome` folder.


Done!

## 2. Possible preferences to change

Set `browser.urlbar.openViewOnFocus` to `false` at `about:config` for you want you address bar arrow back!

![Address bar arrow](https://user-images.githubusercontent.com/1450983/83912955-683d0e00-a777-11ea-92c7-d172a9912776.png)