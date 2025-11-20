# InputHandler

- **Namespace:** Core
- **Implemented in:** `Core.InputSystem`

ScriptableObject that centralises player input callbacks. Reference it to access every gameplay and UI input event in one place. Events can be reassigned and remapped without touching the consuming code.

## Events

| Event | Description |
| --- | --- |
| `MovementEvent` | Gameplay input. Invoked when the player provides movement input. Carries a `Vector2`. |
| `LookEvent` | Gameplay input. Invoked when the mouse or right stick moves. Carries a `Vector2`. |
| `MainUsageEvent` | Gameplay input. Invoked when the main usage button is pressed. |
| `MainUsageCanceledEvent` | Gameplay input. Invoked when the main usage button is released. |
| `SecondaryUsageEvent` | Gameplay input. Invoked when the secondary usage button is pressed. |
| `SecondaryUsageCanceledEvent` | Gameplay input. Invoked when the secondary usage button is released. |
| `InteractEvent` | Gameplay input. Invoked when the interact button is pressed. |
| `SprintEvent` | Gameplay input. Invoked when the sprint button is pressed or released. Carries a `bool` representing the sprint state. |
| `ReloadEvent` | Gameplay input. Invoked when the reload button is pressed. |
| `SlotsEvent` | Gameplay input. Invoked when a slot button is pressed. Carries an `int` identifying the selected slot. |
| `SlotsScrollEvent` | Gameplay input. Invoked when the scroll wheel changes slots. Carries a `Vector2`. |
| `BarkEvent` | Gameplay input. Invoked when the bark button is pressed. |
| `NavigateEvent` | UI input. Invoked when navigation input is performed. Carries a `Vector2`. |

## Example

```csharp
using UnityEngine;
using Core.InputSystem;
using Core.Shared.Utilities;

public class ExampleScript : MonoBehaviour
{
    // Reference to the input handler so this component can listen for inputs.
    [Required] public InputHandler playerInputs;

    private void OnEnable()
    {
        playerInputs.MovementEvent += OnPlayerMovement;
    }

    private void OnDisable()
    {
        playerInputs.MovementEvent -= OnPlayerMovement;
    }

    private void OnPlayerMovement(Vector2 move)
    {
        // TODO: react to player movement input.
    }
}
```

> Need help? Is something described here not working as you expect it to? Please contact [@Soramuele](https://discord.gg/78RjuqzQ) on Discord so we can work to fix it.
