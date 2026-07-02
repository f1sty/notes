---
date: 2026-06-30
tags: [note, avr, arduino]
id: r542
aliases: []
---

# avrdude

avrdude -v -patmega328p -cstk500v1 -P/dev/ttyACM0 -b19200 -Uflash:r:blink.ino.hex:i
