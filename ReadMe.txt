This project is very basic and doesn't perform any validation/checksum tests on the received data, but it does seem to be fairly reliable even with a small amount of background noise.

The default tones used in this project are listed below:

Transmission Start: 2000Hz
Data Bit 1: 600Hz
Data Bit 0: 800Hz
Transmission End: 1500Hz
Next Bit Confirmation: 1200Hz


The transmission speed is determined by the TONE_LENGTH_MS value in the sender program. The receiver program is able to automatically adjust to any transfer speed because consecutive tones are never equal by design. Each tone has a duration of 50ms by default - this seems to be reliable in my testing.
