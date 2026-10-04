# Start here

You are going to recover ten flags from files in the `incident/` folder. Every flag is wrapped as `Intern_Pro_Max{...}`. The characters inside the braces are different for each task. The exact pattern is on that task's page. An example of the wrapper only:

```
Intern_Pro_Max{flag}
```

You have 48 hours from the invitation. Work on your own computer. Stay inside this folder.

This repository is the whole exercise. Everything you need is under `incident/`.

## Set up (about 5 minutes)

1. Install Python 3. On macOS or Linux it is often already there. In a terminal:

```bash
python3 --version
```

You want version 3.9 or newer. If the command is not found, install Python 3 from [python.org](https://www.python.org/downloads/).

2. Open a terminal in this repository (the folder that contains this file).

```bash
cd /path/to/this/repo
python3 -c "print('ready')"
```

You should see `ready`. Every task can be finished with Python from the standard library. You do not need to `pip install` anything.

3. Optional tools, if you already have them:

- A hex viewer or `xxd` helps you look at binary files.
- Wireshark can open the Wi-Fi capture in task 3.
- Audacity can play the audio in task 6.

If you do not have those tools, stay with Python.

## Words that show up a lot

| Word | Plain meaning |
| --- | --- |
| Byte | One number from 0 to 255. Files are a long row of bytes. |
| Hex | Bytes written in base 16. `0x17` is the same number as 23. |
| uint8 | One byte. |
| uint16 little-endian | Two bytes. The smaller one is stored first. |
| ASCII | Bytes that are ordinary letters and digits. |
| Checksum / CRC | A small number computed from the bytes. If it does not match, the chunk is damaged or should be ignored. |
| XOR | Combine two bytes bit by bit. In Python that is `byte ^ mask`. |
| Flag | The short answer for one task, in the form above. |

## The ten tasks

Do them in this order if you are new to this. The numbers below are the numbers you must use when you submit. They are not the order of difficulty.

| Do this | Task | What you hand in | Folder |
| --- | --- | --- | --- |
| First | 5 | A flag that looks like `fm-` plus a whole number | `incident/05-link-budget` |
| | 1 | A short lowercase phrase from a flight log | `incident/01-flight-log` |
| | 6 | Two lowercase words joined by a hyphen, heard in audio | `incident/06-morse-audio` |
| | 3 | A lowercase airframe name from a Wi-Fi beacon | `incident/03-wifi-beacon` |
| | 2 | The text inside one radio message | `incident/02-radio-messages` |
| | 8 | The text a tiny program prints | `incident/08-gimbal-program` |
| | 7 | A phrase rebuilt from a memory dump | `incident/07-memory-dump` |
| | 4 | A frequency in kHz, digits only | `incident/04-channel-hops` |
| | 9 | Launch point, route waypoints, and landing point | `incident/09-border-track` |
| Last | 10 | The mission codeword from the flight computer | `incident/10-mission-codeword` |

Open `TASK.md` inside each folder.

## How to submit your flags

Submit each flag in the CTF portal at <https://13-200-126-136.sslip.io>. Enter the whole flag, including the `Intern_Pro_Max{...}` wrapper.

Shortlisted candidates will be asked to explain their actions in a live online interview. Keep notes as you work: `incident/SUBMISSION.txt` is a sheet for recording each flag and how you recovered it.
