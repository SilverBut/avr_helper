# AVR Helper
Some helpful things for AVR. Submit new scripts if you find they are useful.

## Contributing Guildelines
Considering this project is involved with some different types of file, a better way to organize the PRs is to submit one type of changes within one PR. 

For example, if you are adding a lot of scripts for ATXmega128, including those for IDA, avr-gdb or radare2, you'd better submit them in one PR with the title "balabala script bundle for xx,yy,zz". And if you are submitting several different chip config files for IDA, you may want to submit a PR with the title "IDA config files for blabla, tadiyada".

## File list

### Debugger Scripts
* `AVRContext.txt`: A group of commans for giving a better context view using avr-gdb.

### Processor Descriptions
* `ATmega328P.cfg`: IDA processor configurement file for ATMega328/328P. Test on IDA 7.0
* `ATxmega128A4U.cfg`: IDA processor configurement file for ATxMega128A4U. Test on IDA 7.0

## Notice
* For `ATxmega128A4U`, a bug exists. IDA wrongly added another 0x20 before our register map. According to document from [ATMEL](http://ww1.microchip.com/downloads/en/DeviceDoc/Atmel-8331-8-and-16-bit-AVR-Microcontroller-XMEGA-AU_Manual.pdf), "The register file is located in a separate address space, and so the registers are not accessible as data memory.". This is not same from most AVR processors like ATmega328P. Waiting for a fix from IDA team. **But I will NOT add a workaround in our config file**, and you are required to patch the processor module of AVR by yourself, in order to fix it. You can contact Hexrays for a updated processor module, if they have.

* * *

## Legal Statement
IDA, ATMEL, AVR and all other trademarks cited herein are the property of their respective owners.

Copyright of this repo is belonging to the original author of those code.

Unless otherwise stated, you are requested to follow GPLv3 to use code in this repo.

The following related parts are NOT allowed to use this code, unless a statement is signed and published by the author:

* Humensec (http://www.humensec.com)
* Network Behaviour Research Center (NBRC) in Xidian University (http://nbrc.xidian.edu.cn)
* School of Cyber Engineering of Xidian University (http://ce.xidian.edu.cn)
* Leaders, researchers, students and any other people or entity sharing common benefits with entities above

According to the relevant laws, including the *Cybersecurity Law of the People's Republic of China*, the author and other related entities will resort to legal measures if you are not complying this license.
