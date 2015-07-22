# tools/clipboard.lua - A Jumpcut Replacement


Inspired by the Caffeine replacement example, I wrote a Jumpcut replacement.

* It monitors the clipboard/pasteboard for changes, and stores the history of strings you copy to the transfer area.
* You can access this history on the menu (Unicode scissors icon).
* Clicking on any item will add it to your transfer area.
* If you open the menu while pressing option/alt, you will enter the Direct Paste Mode. This means that the selected item will be "typed" instead of copied to the active clipboard.
* The clipboard persists across launches (it is stored with hs.settings)

The code is a little bit crude, so I would appreciate suggestions on ways to improve it.

I think the crash report functionality could leak your clipboard to the developers / third-parties, so be a little bit careful (disable reporting).

Import this by including `require "tools/clipboard"` to your `.hammerspoon/init.lua` file.
