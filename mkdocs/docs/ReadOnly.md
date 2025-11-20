# ReadOnly

- **Namespace:** Core.Shared
- **Implemented in:** `Core.Shared.Utilities`

Attribute that makes inspector fields visible but not editable. Apply `[ReadOnly]` to serialised or public fields that should stay unchanged while remaining visible.

## Example

```csharp
using UnityEngine;
using Core.Shared.Utilities;

public class ExampleScript : MonoBehaviour
{
    // Editable from the inspector.
    public float modifier = 2.5f;

    [SerializeField] private int number = 2025;

    // Visible in the inspector but cannot be edited.
    [ReadOnly] public float hour;

    private void Update()
    {
        hour += (modifier / number) * Time.deltaTime;
    }
}
```

> Need help? Is something described here not working as you expect it to? Please contact [@Soramuele](https://discord.gg/78RjuqzQ) on Discord so we can work to fix it.
