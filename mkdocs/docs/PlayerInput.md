# PlayerInput

- **Namespace:** Team1
- **Implemented in:** `Gameplay.Player`

Handles reading input actions and exposing them to gameplay systems. Initialises all player input actions and manages the cursor position in world space.

## Properties

| Property | Description |
| --- | --- |
| `Move` | Returns a `Vector2` with the player's movement input. |
| `Look` | Provides an `Observable` that tracks the cursor position in the world. |
| `Run` | Returns `true` while the sprint button is held, otherwise `false`. |
| `Reload` | `InputAction` for the reload button. Use the `started`, `performed`, and `canceled` callbacks. |
| `MainUsage` | `InputAction` for the primary usage button. Use the `started`, `performed`, and `canceled` callbacks. |
| `SecondaryUsage` | `InputAction` for the secondary usage button. Use the `started`, `performed`, and `canceled` callbacks. |
| `SlotsScroll` | `InputAction` for slot scrolling. Use the `started`, `performed`, and `canceled` callbacks. |
| `Slot_1` | `InputAction` for the slot 1 button. Use the `started`, `performed`, and `canceled` callbacks. |
| `Slot_2` | `InputAction` for the slot 2 button. Use the `started`, `performed`, and `canceled` callbacks. |
| `Slot_3` | `InputAction` for the slot 3 button. Use the `started`, `performed`, and `canceled` callbacks. |

> Need help? Is something described here not working as you expect it to? Please contact [@Soramuele](https://discord.gg/78RjuqzQ) on Discord so we can work to fix it.
