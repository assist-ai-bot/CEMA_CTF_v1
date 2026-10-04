# Exercise Night Kite

A hostile drone crossed India's western international border in the Barmer sector and was forced down by electronic-warfare jamming. The airframe was recovered on the ground with its recorder, radio captures, and companion computer still aboard. Those files are in `incident/`.

The detachment that recovered it needs ten flags before the intelligence report can be closed. Eight of them are short commissioning values from the onboard systems. The ninth is the track: launch point, route waypoints, and the place it came down. The tenth is the mission codeword still locked in the flight computer.

| Flag | What it is | Where to look |
| --- | --- | --- |
| 1 | The note left in the flight recorder | `incident/01-flight-log` |
| 2 | The last useful message on the control radio | `incident/02-radio-messages` |
| 3 | The name the aircraft announced over Wi-Fi | `incident/03-wifi-beacon` |
| 4 | The channel the link would have used on the next hop that was never recorded | `incident/04-channel-hops` |
| 5 | Whether the radio path still had enough margin | `incident/05-link-budget` |
| 6 | The name sent on the guard channel | `incident/06-morse-audio` |
| 7 | The line rebuilt from the companion computer's memory | `incident/07-memory-dump` |
| 8 | The line the gimbal program prints when it is run | `incident/08-gimbal-program` |
| 9 | Launch coordinates, route waypoints, and the final landing coordinates. The exact character pattern is in that task page | `incident/09-border-track` |
| 10 | The mission codeword still locked in the flight computer. The exact character pattern is in that task page | `incident/10-mission-codeword` |

This incident is fiction. Work only from this folder, on your own machine. You have 48 hours. Submit the ten flags, each as `Intern_Pro_Max{flag}`, in the CTF portal at <https://13-200-126-136.sslip.io>.

Shortlisted candidates will be asked to explain what they did for each flag in a live online interview, so keep notes as you work.

Setup and the submission shape are in **[START_HERE.md](START_HERE.md)**. Open each task's `TASK.md` for what that flag is.
