# IState

- **Namespace:** Core.Shared.StateMachine

Interface for states used by state managers.

## Members

| Member | Description |
| --- | --- |
| `OnStart()` | Called when the state becomes active. |
| `OnStop()` | Called when the state is exited. |
| `OnUpdate()` | Runs after `OnStart()` every frame until `OnStop()` is invoked. |

> Need help? Is something described here not working as you expect it to? Please contact [@Soramuele](https://discord.gg/78RjuqzQ) on Discord so we can work to fix it.
