# Setup Raycast & Karabiner Elements for Window Management

## Karabiner Elements

### Install

### [Karabiner Elements](https://karabiner-elements.pqrs.org/)

### Setup

1. Install Karabiner Elements.

2. Grant all required permissions (Follow on-screen instructions)

3. Open Karabiner Elements.

4. Go to `Karabiner Elements` > `Preferences` > `Complex Modifications`.

5. Click on `+` button to add new complex modification.

6. Add "Change Caps lock to Hyper Key" rule -

```
{
    "description": "Change caps lock to hyper key",
    "manipulators": [
        {
            "from": {
                "key_code": "caps_lock",
                "modifiers": { "optional": ["any"] }
            },
            "to": [
                {
                    "key_code": "left_shift",
                    "modifiers": ["left_command", "left_control", "left_option"]
                }
            ],
            "type": "basic"
        }
    ]
}
```

7. Add "Change Double Tap Right Shift to Caps Lock" rule -

```
{
    "description": "Change double tap right ⇧ key to caps lock",
    "manipulators": [
        {
            "conditions": [
                {
                    "name": "right_shift pressed",
                    "type": "variable_if",
                    "value": 1
                }
            ],
            "from": {
                "key_code": "right_shift",
                "modifiers": { "optional": ["any"] }
            },
            "to": [{ "key_code": "caps_lock" }],
            "type": "basic"
        },
        {
            "from": {
                "key_code": "right_shift",
                "modifiers": { "optional": ["any"] }
            },
            "to": [
                {
                    "set_variable": {
                        "name": "right_shift pressed",
                        "value": 1
                    }
                },
                { "key_code": "right_shift" }
            ],
            "to_delayed_action": {
                "to_if_canceled": [
                    {
                        "set_variable": {
                            "name": "right_shift pressed",
                            "value": 0
                        }
                    }
                ],
                "to_if_invoked": [
                    {
                        "set_variable": {
                            "name": "right_shift pressed",
                            "value": 0
                        }
                    }
                ]
            },
            "type": "basic"
        }
    ]
}
```

## Raycast

### Install

### [Raycast](https://www.raycast.com/)

1. Disable Command + Space shortcut which used to show Spotlight search.

    a. Go to System Settings -> Keyboard -> Change "Press Globe key to" -> "Change input source"

    b. Go to System Settings -> Keyboard -> Keyboard Shortcuts -> Spotlight -> UNCHECK "Show Spotlight Search"

2. Update RayCast Default Keybinding to Command + Space.

3. Under RayCast Extension Settings, add the application shortcuts with Hyper key as the trigger.

<code>

a. Google Chrome - `Hyper + b`

b. Notion - `Hyper + n`

c. Cursor - `Hyper + e`

d. iTerm - `Hyper + t`

e. Postman - `Hyper + p`

f. Notes - `Hyper + o`

g. Finder - `Hyper + f`

h. Apple Music - `Hyper + m`

i. Books - `Hyper + r`

j. Adobe Reader - `Hyper + a`

k. Visual Studio Code - `Hyper + v`

l. Whatsapp - `Hyper + w`

m. Zoom - `Hyper + z`

n. Super Whisper - `Hyper + s`

4. Under RayCast Extension Settings, under "Window Management" tab, add the following rules -

<code>

a. Move to Top Half - `Option + k`

b. Move to Bottom Half - `Option + j`

c. Move to Left Half - `Option + h`

d. Move to Right Half - `Option + l`

e. Maximize - `Option + m`

</code>
