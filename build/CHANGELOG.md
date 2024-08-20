# Changelog

All notable changes to this project will be documented in this file.

This project adheres to [Semantic Versioning](https://semver.org/).

## [Unreleased]


## [2.4.0] - 2024-08-19

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

## [2.2.0] - 2024-08-14

### Added
- New tab menu **Keep Tab Active**: Keep the tab active so it won't be automatically discarded.

### Changed
- Optimized performance and reduced bundle size.

## [2.1.0] - 2024-08-10

### Added
- Automatically save window, group, and tab snapshots. After restarting the browser, if only one window is open and fewer than 5 new tabs are opened, a toast will prompt to restore the last saved window and tab information when the sidebar is opened.

### Changed
- Optimized the storage data for quick access to speed up access time.

### Fixed
- Fixed other minor issues.

## [2.0.1] - 2024-08-09

### Fixed
- Fixed the message format for successful snapshot import.
- Fixed the issue where duplicate imports caused repeated quick access entries.

## [2.0.0] - 2024-08-08

### Changed
- Renamed the extension from "Colorful Side Panel Tabs" to **"VertiTab - Side Panel Vertical Tabs"**.

### Added
- Snapshots: Added a one-click save browser tab snapshot feature. You can save snapshots before closing the browser and quickly restore them the next time you open it. Currently, up to 50 snapshots can be saved.
- Enhanced Bottom Navigation Bar: Access more features from the bottom navigation bar, such as bookmarks, history, recently closed tabs, reading list, quick access, open new tab, create snapshot, search, collapse groups, etc.
- Updated Import/Export Functionality: Improved import and export options to better manage tabs across devices.

### Fixed
- Bug fixes and stability improvements.

## [1.3.3] - 2022-08-04

### Added
- **linkSettings**: Site settings now include a new option that allows you to add rules to control whether site links open in the current tab or a new tab.

## [1.3.2] - 2024-08-02

### Fixed
- Fixed the issue that clicking the middle mouse button to close the tab did not work.

## [1.3.1] - 2024-08-01

### Changed
- Optimized the layout of quick access and added support for drag-and-drop sorting.
- Improved the logic for expanding all groups and remembering their state.

### Fixed
- Fixed the issue where importing quick access data failed when the side panel was not open.
- Fixed the issue where icons were misaligned in the group view.
- Fixed other minor issues.

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

## [1.2.3] - 2024-07-23

### Fixed
- Fixed incorrect list scroll height calculation when pinned tabs and quick access icons exceed 1 row.

### Changed
- Changed discard inactive tabs to exclude pinned tabs.
- Changed closing all discarded tabs to exclude pinned tabs.
- Adjust the size of pinned and quick access icons.

## [1.2.2] - 2024-07-19

### Added
- Add quick access: You can set a tab to show up in Quick access so it'll be easy to find. Just right-click (or long-press) it and select Pin to Quick access. Unpin it when you don’t need it there anymore by right-clicking (or long-pressing) it and selecting Delete from Quick access. The difference from pinned tabs is that Quick Access saves the URL and opens a new tab every time it is clicked.

### Changed
- Pinned tabs only display icons to prevent them from being accidentally clicked and then unpinned.
- Modify the size of fixed tab icons.

## [1.2.1] - 2022-07-17

### Added
- Add new menu to bottom navigation: discard inactive tabs.
- Add new menu to bottom navigation: close all discarded tabs.

### Changed
- Changes to the bottom navigation menu "Group by site" only affect the current window.

### Fixed
- Fixed the issue where the UI would jump due to height inconsistency when switching active tabs in the list.

## [1.2.0] - 2024-07-16

### Added
- Add Site Configs: Customize site-specific settings, such as disabling Picture-in-Picture mode, disabling auto discardable mode, and more.

### Fixed
- Fix Auto Create or Join Same Domain Group: Resolved an issue where auto-creating or joining same domain groups was not working when a tab was updated.
- Fix Page Not Receiving Config Update Messages: Ensured that pages correctly receive configuration update messages.
- Fix Other Bugs: Addressed various other bugs to improve stability and performance.

### Changed
- Add Option to Show Close Button on Hover: Added an option to display the close button only when hovering over a tab.

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

## [1.0.4] - 2024-07-09

### Added
- Drag and Drop Sorting for Tabs: Easily rearrange your tabs with drag and drop functionality.

### Changed
- Optimize Page Loading Speed: Further enhanced page loading speed for an even smoother browsing experience.

## [1.0.3] - 2024-07-05

### Fixed
- Fix Mixed View Menu Error: Resolved an issue where the mixed view menu was displaying errors.

### Changed
- Optimize Tab Group Domain Menu: Enhanced the tab group domain menu for better organization and usability.
- Optimize Tab Padding: Adjusted tab padding for a more streamlined and visually appealing layout.

## [1.0.2] - 2024-07-04

### Added
- Current Active Tab Indicator: Easily identify the active tab with a new visual indicator.
- Custom Font Color: Personalize your interface by setting a custom font color.

### Changed
- Optimize Loading Speed: Improved loading speed for a faster and smoother user experience.

### Default Settings
- Set Default Not to Use Color Mode: The default setting now uses single color mode for a simplified appearance.

## [1.0.1] - 2024-07-02

### Added
- Complete History Record by Time Range: Access and manage your browsing history with detailed records sorted by time range.
- Single Color Mode for List: Introduce a single color mode for a simplified and consistent list appearance.

### Changed
- Complete Audio Progress Bar Update Timing: Enhanced the accuracy of audio progress bar updates for a smoother multimedia experience.
- Optimized List Icon Acquisition Method: Improved the method for acquiring list icons, resulting in faster and more reliable icon loading.

### Fixed
- Fix Incorrect Activation Status Display Issue in Multiple Windows: Resolved an issue where the activation status was incorrectly displayed when multiple windows were open.

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
