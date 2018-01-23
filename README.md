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
