# Required

- **Namespace:** Core.Shared
- **Implemented in:** `Core.Shared.Utilities`

Attribute that enforces object references in the inspector. Attach `[Required]` to fields that must be set before entering play mode. Unity warns the editor and blocks play mode until all required references are assigned, preventing `NullReferenceException` at runtime.

## Example

```csharp
using UnityEngine;
using Core.Shared.Utilities;

public class ExampleScript : MonoBehaviour
{
    // Optional configuration value.
    public float number = 20f;

    // Must be assigned for this component to work in play mode.
    [Required] public Health healthScript;

    private void OnCollisionEnter(Collider collider)
    {
        healthScript.Damage(number);
    }
}
```

> Need help? Is something described here not working as you expect it to? Please contact [@Soramuele](https://discord.gg/78RjuqzQ) on Discord so we can work to fix it.
