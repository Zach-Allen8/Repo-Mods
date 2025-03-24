# v2.1.0
- Scrollbar positions get updated when setting a page's mask padding
- Added cached pages
  - This prevents you from having to regenerate your menu constantly
    - You can only set this via the `MenuAPI.CreateREPOPage` method
- Added 'Action onClick' to REPOButton
- Added 'REPOAvatarPreview'
- Pressing escape goes back one page now

# ***v2.0.0 - THE REWRITE***
- You can now add buttons to the menu lobby
- Upgraded scroll boxes
  - Elements out of view will be disabled automatically to reduce lag
  - Fixed scroll boxes from not scrolling down all the way
  - Removed rebinding UI for keybinds (This could return later)
    - You can still change the keybind, it'll just be an option slider instead
- Switched to all custom monobehaviours
  - Introduces REPOLabel, REPOButton, & REPOSpacer
  - This gives you almost full control over your elements
- **Plus a lot more**

# v1.0.5
- Added new method `SetBarState` to REPOSlider
  - Changes the behavior of the background bar (UpdateWithValue, StaticMinimum, StaticMaximum)
  - This would typically be used for `Enum` types

# v1.0.4
- Changed slider increment buttons to only increment by 1
  - This depends on how precise your slider is

# v1.0.3
- Added keybind support (UnityEngine.InputSystem.Key)
- Made slider descriptions scroll
- Migrated OpenDialog from the `REPOButton` to the `MenuAPI`

# v1.0.2
- Fixed label size for toggles

# v1.0.1
- Added option support to sliders
  - Rather than displaying a number, words can be displayed

# v1.0.0 🔥
- Initial release