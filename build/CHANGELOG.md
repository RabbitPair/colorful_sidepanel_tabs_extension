# Changelog

All notable changes to this project will be documented in this file.

This project adheres to [Semantic Versioning](https://semver.org/).

## [Unreleased]


- Fixed the issue where danmaku (bullet comments) would stop or disappear on some websites after switching pages (page hide event)
- hide HTML5 video controls

----
## [2.10.1] - 2024-10-05

### Fixed
- Fixed the issue where shortcut events were triggered repeatedly when playing multiple videos consecutively
- Fixed an issue where the player failed to restore in certain situations
- Fixed the issue where the playback progress bar did not work properly when using Picture-in-Picture mode
- Fixed the issue where switching tabs would trigger a Picture-in-Picture detection toast after navigating from a page with a video to a page without a video in the same tab.
- Fixed the issue where the Picture-in-Picture window did not close when exiting Picture-in-Picture mode using jwPlayer
- Fixed the issue where an incorrect address caused the page to crash when setting a background image

----

----
## [2.10.0] - 2024-10-01

### Added
- **Document Picture-in-Picture**: Introducing Advanced Picture-in-Picture, available for free trial before the official release of the extension's premium version. When enabled, it takes precedence over the standard Picture-in-Picture. If the current page does not support it, the standard mode will be used. Advanced Picture-in-Picture features a custom video player with functionalities such as:
  * **Play/Pause video** (Space or K)
  * **Adjust volume** (Up/Down Arrow)
  * **Mute/Unmute video** (M)
  * **Fast forward/Rewind video** (Left/Right Arrow or Mouse Wheel)
  * **Fast forward/Rewind video 5 seconds** (Left/Right Arrow)
  * **Fast forward/Rewind video 10 seconds** (J/L)
  * **Play the next video** (Shift + N)
  * **Play the previous video** (Shift + P)
  * **Display subtitles** (supported on some websites like youtube.com, vimeo.com, tver.jp, etc.) (C)
  * **Display barrage** (supported on some websites like nicovideo.jp, bilibili.com, etc.) (D)
  * **Exit Picture-in-Picture** (Esc)
  * **Toggle hide/show video and play/pause** (Q)
  * **Toggle fullscreen** (F)
  * **Adjust playback speed** ( > or <)
  * **Seek to start/end of video** (Home/End)
  * **Seek to percentage of video** (0-9)
  * **Adjust window to fit video size** (W)
  * **Toggle Picture-in-Picture from main page** (Alt + P)
  
  > If the websites you frequently visit support subtitles or barrage, you can submit an [issue: Advanced Picture-in-Picture](https://github.com/RabbitPair/colorful_sidepanel_tabs_extension/issues/new?assignees=&labels=&projects=&template=Advanced-Picture-in-Picture.md&title=), and we will adapt it as soon as possible. Please note that some websites may have regional restrictions, requiring additional information.
- **Shortcut for Picture-in-Picture**: A new keyboard shortcut Alt+P has been added to quickly toggle Picture-in-Picture mode. This allows users to easily switch videos to Picture-in-Picture view without using the mouse, enhancing productivity and multitasking capabilities.
- **Switch Picture-in-Picture in Bottom Navigation Bar**: You can now add a Picture-in-Picture toggle option to the bottom navigation bar. This can be configured in the appearance settings under "Show bottom navigation bar" - "Configure".
- **Sort Tabs by URL**: A new menu option "Sort Tabs by URL" has been added to the "More" menu.
- **Tab Group Collapse Behavior**: A new option "Tab Group Collapse Behavior" has been added to the "Advanced Tab Group" menu. You can modify the behavior of tab group collapsing in the browser. The options include: 'Show current group and collapse other groups', 'Expand all groups', and 'Use browser default settings'.
- **Site Settings**: Three new options have been added to the site settings:
  * **Picture-in-Picture Restriction Action**: Configure the action for Picture-in-Picture restrictions.
  * **Auto-enter Picture-in-Picture**: Automatically enter Picture-in-Picture mode when a video is present upon entering the page.
  * **Caption Settings**: Configure the CSS selectors for the caption element and its parent on the page.

### Changed
- When the side panel tab is not open, if "Picture-in-Picture on Tab Switch" is enabled (enabled by default), it will automatically enter Picture-in-Picture mode (Important reminder: User interaction is required, such as clicking on the page playing the video to activate user interaction).
- When closing the page sidebar, it is now removed instead of hidden. It will reappear only after refreshing the page.

### Fixed
- Fixed the issue where the Quick Access list did not handle multiple URLs.

----

## [2.9.0] - 2024-09-15

- Added **Clear Tabs**: Save a snapshot and close all tabs except the active one. Restore them from recently closed tabs or snapshots.
- Added **Auto Activate Tab Grouping**: Automatically create a new group when opening a new tab. Subsequent tabs opened from this tab will join the group.
- Added **List Vertical Spacing**: New option in Advanced Tab Group settings to adjust vertical spacing for list items.
- Added **Add Multiple URLs to Quick Access**: Allows adding groups and selecting multiple tabs to save to Quick Access.
- Added **Quick Access Item Spacing**: Set vertical/horizontal spacing for Quick Access items in the options page.



---
## [2.8.0] - 2024-09-12
### Added
- Added **Tab History**: Now you can easily see which websites have been opened under the same tab. Left-click to open the website in the current tab, middle-click or Ctrl+left-click to open the website in a new tab. For more details, please check the options page.
- Added **Custom group names**: In the options page - Advanced Tab Group,You can add some pre-defined groups here, so you can quickly select them when you need to add tabs to a group. We have already preset some group names, which you can modify or delete according to your needs.
- Added **Use bookmark folder name as group name**: In the options page - Advanced Tab Group, a new option has been added. If the opened website is a bookmark, it will be automatically added to the group, and the group name will use the bookmark directory name.
- Added **Tab Index**: In the options page,When enabled, the tab index will be displayed next to the title, making it easy to active tab using [Ctrl+number] on Windows or [cmd+number] on Mac. Example: 1. stackoverflow.com 2. youtube, so that it's easy to do Ctrl + 2 on Windows or cmd + 2 on Mac to go to youtube
- **Optimized site settings**: Improved the option to set Background color and Font color for sites.

### Changed
- When checking bookmarks, allow updating redirected URLs. If the URL is not accessible, display error codes: Successful responses (200 – 299), Redirection messages (300 – 399), Client error responses (400 – 499), Server error responses (500 – 599). For more details, please see: https://developer.mozilla.org/en-US/docs/Web/HTTP/Status

### Fixed
- Fixed the issue where the bookmark modification popup did not disappear

---

## [2.7.0] - 2024-09-05

### Added

- Added **bookmark management**: Added full-featured bookmark management functionality
- Added **Tab navigation bar**: options in appearance, displaying: tabs, bookmarks, history, recently closed tabs, reading list, and quick access on the side panel
- Added **Add tab to group** menu: add tabs to a new group or an existing group
- Added search keyword highlighting
- Added Premium Edition reservation

### Changed

- Adjusted Cookie, ReadingList, and bookmarks permissions to optional permissions, requiring user authorization for use

### Deprecated

- **Options Page - History - Show in side panel**: This option has been replaced by _Tab navigation bar_ and will be deprecated soon

### Fixed

- Fixed the issue where the expand group button would not appear when first clicking the sidebar
- Fixed the issue where reopening the browser and clicking the extension icon required reselecting between popup or sidebar
- Fixed the issue where the pinned tab icon and quick access icon sizes were inconsistent

---

## [2.6.1] - 2024-08-30

### Changed

- Optimized menu display method, improved error prompts
- Added more compatibility for Chromium-based browsers

---

## [2.6.0] - 2024-08-28

### Added

- Added **Tab Menu Zoom**: A zoom feature has been added to the tab menu, allowing you to freely adjust the zoom level from 1% to 1000%.

### Changed

- Quick Access has been moved to a separate menu item.
- Optimized drag-and-drop sorting

### Fixed

- Fixed an issue where some areas did not change after altering the font color.

### Deprecated

- **Quick Access in Tabs Menu**: Quick Access has been moved to a separate menu item. The option in the tab menu will be deprecated soon (the functionality remains the same).

### Removed

- Removed the zoom option from site settings because adjusting the zoom in the menu did not provide an intuitive preview of the changes. The zoom feature has been moved to the tab menu for real-time preview.

---

## [2.5.2] - 2024-08-27

### Fixed

- Fixed the issue where saved background images were lost after restarting the application
- Fixed the issue where closing all tabs from the same site in all windows failed
- Fixed crash when disabling DnD

---

## [2.5.0] - 2024-08-25

### Added

- Support drag-and-drop sorting of tabs and groups in tab order, and sync with Chrome
- Sync group expansion state with Chrome

### Fixed

- Fixed the issue where uploading a background image file that is too large causes a QUOTA_BYTES quota exceeded error
- Fixed the issue where displaying all window tabs caused an error and grouping by site failed

---

## [2.4.0] - 2024-08-20

### Added

- add **Upload Background Image**: You can upload an image from your local device to use as a background.
- add **Custom Background Color**: Now supports custom background colors, and you can also choose a color to generate a beautiful gradient

### Changed

- **font color**: The font color will automatically change to black or white based on the dominant color of the background or background image. If the image is large, it may take some time to apply the background, which is normal.

### Fixed

- Fixed the issue where some areas did not change after changing the font color

### Deprecated

- **List background style**: This feature sets the background style for each list, with some built-in gradient colors. However, with the release of custom background colors, its mission has been completed and it will be removed soon.

---

## [2.3.0] - 2024-08-16

### Added

- add **Sidebar On Pages**:The page sidebar allows you to inject a sidebar into the web pages you are browsing without opening the browser sidebar to manage tabs. This is a very useful feature for users with smaller screen resolutions who find the browser sidebar too wide and unadjustable. However, due to some restrictions, the page sidebar only offers very limited functionality. When this feature is enabled, you can use the mouse to hover over the edge of the window to bring out the sidebar.

### Removed

- remove **Float ball**

---

## [2.2.0] - 2024-08-14

### Added

- New tab menu **Keep Tab Active**: Keep the tab active so it won't be automatically discarded.

### Changed

- Optimized performance and reduced bundle size.

---

## [2.1.0] - 2024-08-10

### Added

- Automatically save window, group, and tab snapshots. After restarting the browser, if only one window is open and fewer than 5 new tabs are opened, a toast will prompt to restore the last saved window and tab information when the sidebar is opened.

### Changed

- Optimized the storage data for quick access to speed up access time.

### Fixed

- Fixed other minor issues.

---

## [2.0.1] - 2024-08-09

### Fixed

- Fixed the message format for successful snapshot import.
- Fixed the issue where duplicate imports caused repeated quick access entries.

---

## [2.0.0] - 2024-08-08

### Changed

- Renamed the extension from "Colorful Side Panel Tabs" to **"VertiTab - Side Panel Vertical Tabs"**.

### Added

- Snapshots: Added a one-click save browser tab snapshot feature. You can save snapshots before closing the browser and quickly restore them the next time you open it. Currently, up to 50 snapshots can be saved.
- Enhanced Bottom Navigation Bar: Access more features from the bottom navigation bar, such as bookmarks, history, recently closed tabs, reading list, quick access, open new tab, create snapshot, search, collapse groups, etc.
- Updated Import/Export Functionality: Improved import and export options to better manage tabs across devices.

### Fixed

- Bug fixes and stability improvements.

---

## [1.3.3] - 2022-08-04

### Added

- **linkSettings**: Site settings now include a new option that allows you to add rules to control whether site links open in the current tab or a new tab.

---

## [1.3.2] - 2024-08-02

### Fixed

- Fixed the issue that clicking the middle mouse button to close the tab did not work.

---

## [1.3.1] - 2024-08-01

### Changed

- Optimized the layout of quick access and added support for drag-and-drop sorting.
- Improved the logic for expanding all groups and remembering their state.

### Fixed

- Fixed the issue where importing quick access data failed when the side panel was not open.
- Fixed the issue where icons were misaligned in the group view.
- Fixed other minor issues.

---

## [1.3.0] - 2024-07-30

### Added

- **Import/Export**: Export user preferences, quick access, website settings, and recently closed tabs data, and import them into another browser to synchronize extension data.
- **Select quick access from history**: You can search the most frequently visited websites from the history and add them to the quick access.
- **Toolbar more options**: Add more options to the toolbar. You can hide the label on the toolbar and control which icons are displayed on the toolbar.

### Changed

- **Search Box**: The search box now supports the Enter key to search keywords in a new tab. If there is no matching tab or history after entering the keyword, you can press Enter to search using the default search engine.
- **Data Initialization**: Adjust the timing of data initialization and optimize repeated rendering caused by data modifications.
- **Changelog URL**: Update the changelog URL to the release URL on GitHub.
- **Layout Optimization**: Optimize layout changes when the window size changes.
- **Error logs recording**: Use Sentry to collect error logs. Rest assured, this feature will not collect your private data.

### Fixed

- **Tooltip position error**: Fix the issue where the tooltip flashes when switching themes and views in the toolbar.
- **Bottom Navigation**: Fix the issue where the bottom navigation blocks the list when many tabs are open.

---

## [1.2.3] - 2024-07-23

### Fixed

- Fixed incorrect list scroll height calculation when pinned tabs and quick access icons exceed 1 row.

### Changed

- Changed discard inactive tabs to exclude pinned tabs.
- Changed closing all discarded tabs to exclude pinned tabs.
- Adjust the size of pinned and quick access icons.

---

## [1.2.2] - 2024-07-19

### Added

- Add quick access: You can set a tab to show up in Quick access so it'll be easy to find. Just right-click (or long-press) it and select Pin to Quick access. Unpin it when you don’t need it there anymore by right-clicking (or long-pressing) it and selecting Delete from Quick access. The difference from pinned tabs is that Quick Access saves the URL and opens a new tab every time it is clicked.

### Changed

- Pinned tabs only display icons to prevent them from being accidentally clicked and then unpinned.
- Modify the size of fixed tab icons.

---

## [1.2.1] - 2022-07-17

### Added

- Add new menu to bottom navigation: discard inactive tabs.
- Add new menu to bottom navigation: close all discarded tabs.

### Changed

- Changes to the bottom navigation menu "Group by site" only affect the current window.

### Fixed

- Fixed the issue where the UI would jump due to height inconsistency when switching active tabs in the list.

---

## [1.2.0] - 2024-07-16

### Added

- Add Site Configs: Customize site-specific settings, such as disabling Picture-in-Picture mode, disabling auto discardable mode, and more.

### Fixed

- Fix Auto Create or Join Same Domain Group: Resolved an issue where auto-creating or joining same domain groups was not working when a tab was updated.
- Fix Page Not Receiving Config Update Messages: Ensured that pages correctly receive configuration update messages.
- Fix Other Bugs: Addressed various other bugs to improve stability and performance.

### Changed

- Add Option to Show Close Button on Hover: Added an option to display the close button only when hovering over a tab.

---

## [1.1.0] - 2024-07-13

### Added

- Add Performance Options: Introduce new performance settings to customize and enhance your browsing experience.
- Add Scroll to Active Tab Icon: Easily navigate to the active tab with a new scroll-to-active tab icon.
- Add Sort Tabs by Domain: Organize your tabs by domain with a new sorting feature.
- Mute All Tabs Making Sounds: Quickly mute all tabs that are playing sounds for a quieter browsing experience.

### Changed

- Remove Restore Icon: The restore icon has been removed and replaced with list text opacity set to 0.5 for a cleaner look.

### Deprecated

- Remove Drag-and-Drop Sorting: The current solution for drag-and-drop sorting has performance problems and has been temporarily removed.

---

## [1.0.4] - 2024-07-09

### Added

- Drag and Drop Sorting for Tabs: Easily rearrange your tabs with drag and drop functionality.

### Changed

- Optimize Page Loading Speed: Further enhanced page loading speed for an even smoother browsing experience.

---

## [1.0.3] - 2024-07-05

### Fixed

- Fix Mixed View Menu Error: Resolved an issue where the mixed view menu was displaying errors.

### Changed

- Optimize Tab Group Domain Menu: Enhanced the tab group domain menu for better organization and usability.
- Optimize Tab Padding: Adjusted tab padding for a more streamlined and visually appealing layout.

---

## [1.0.2] - 2024-07-04

### Added

- Current Active Tab Indicator: Easily identify the active tab with a new visual indicator.
- Custom Font Color: Personalize your interface by setting a custom font color.

### Changed

- Optimize Loading Speed: Improved loading speed for a faster and smoother user experience.

### Default Settings

- Set Default Not to Use Color Mode: The default setting now uses single color mode for a simplified appearance.

---

## [1.0.1] - 2024-07-02

### Added

- Complete History Record by Time Range: Access and manage your browsing history with detailed records sorted by time range.
- Single Color Mode for List: Introduce a single color mode for a simplified and consistent list appearance.

### Changed

- Complete Audio Progress Bar Update Timing: Enhanced the accuracy of audio progress bar updates for a smoother multimedia experience.
- Optimized List Icon Acquisition Method: Improved the method for acquiring list icons, resulting in faster and more reliable icon loading.

### Fixed

- Fix Incorrect Activation Status Display Issue in Multiple Windows: Resolved an issue where the activation status was incorrectly displayed when multiple windows were open.

---

## [1.0.0] - 2024-06-29

### Added

- Light/Dark Mode Toggle: Choose between light and dark display modes to match your preferences.
- Customizable Font Size: Adjust the font size for a more comfortable reading experience.
- Customizable Interface Layout: Personalize the interface layout according to your usage habits.
- Personalization Options: Add colorful backgrounds and background images to make your side panel unique.
- Advanced Tab Management: Thumbnail previews, rich sorting and display options, and a comprehensive action menu for efficient tab management.
- Search Functionality: Quickly search for recently closed tabs or browse your history to find what you need.
- Picture-in-Picture Mode: Seamlessly switch to Picture-in-Picture mode when changing tabs or scrolling through pages.
- Automatic Grouping: Automatically create or join groups based on the same domain for better organization.
- Reading Progress Bar: Track your reading progress in real-time to know how far you've read.
- Playback Progress Bar: Control multimedia playback with options for fast-forward, rewind, volume control, and playback speed adjustment.
