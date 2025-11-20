# IPlayerTool

- **Namespace:** Core.Shared

Interface implemented by every player-usable tool.

## Members

| Member | Description |
| --- | --- |
| `HideTool()` | Hides the tool from the character. |
| `MainUsageStarted(Observable observable)` | Called when the main usage (typically left click) starts. Receives the relevant `Observable` context. |
| `MainUsageFinished()` | Called when the main usage input ends. |
| `Reload()` | Executes the tool's reload logic. |
| `SecondaryUsageStarted(Observable observable)` | Called when the secondary usage (typically right click) starts. Receives the relevant `Observable` context. |
| `SecondaryUsageFinished()` | Called when the secondary usage input ends. |
| `ShowTool()` | Makes the tool visible/active. |
| `TryBark()` | Triggers the dog bark from the tool when possible. |

> Need help? Is something described here not working as you expect it to? Please contact [@Soramuele](https://discord.gg/78RjuqzQ) on Discord so we can work to fix it.
