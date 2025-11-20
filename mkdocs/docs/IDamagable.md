# IDamagable

- **Namespace:** Gameplay.HealthSystem

Interface for components that can receive damage.

## Members

| Member | Description |
| --- | --- |
| `DamageEvent` | UnityEvent that fires whenever damage is applied. Use this to chain custom reactions. |
| `TakeDamage(float amount)` | Handles incoming damage. Call to inflict damage on the implementer. |

> Need help? Is something described here not working as you expect it to? Please contact [@Soramuele](https://discord.gg/78RjuqzQ) on Discord so we can work to fix it.
