# DogBark

- **Namespace:** Team1
- **Implemented in:** `Gameplay.Dog`

Manages the dog's bark, exposing hooks so other systems can react to bark triggers.

## Members

| Member | Description |
| --- | --- |
| `onDogBark` | Event invoked whenever the dog barks. Subscribe to react to bark actions. |
| `TryBark()` | Attempts to trigger a bark. When successful, scares all nearby [`IScareable`](IScareable.md) instances and invokes `onDogBark`. |

> Need help? Is something described here not working as you expect it to? Please contact [@Soramuele](https://discord.gg/78RjuqzQ) on Discord so we can work to fix it.
