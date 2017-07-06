

Start `Debugserver` and `LLDB`，attatch the process you want to debug.

## How to use

### 1. Import the scripts

`command script import ~/Path/To/breakpoint.py`

`command script import ~/Path/To/objc_msgSend.py`

Also, you can put these command above into the file `~/.lldbinit` 


### 2. Commands example


`(lldb) process interrupt`

`(lldb) help`

`(lldb) iaslr`

`(lldb) iaslr UIKit`

`(lldb) ibreak Foundation 0x00000001234567 `		`// 0x00000001234567 Copied from IDA/Hopper`

`(lldb) iobjc_msgSend`

`(lldb) idisassemble`


### 3. Tips

Full enter the commad characters is not necessary , use the `Tab` keyboard key. Take `iobjc_msgSend` as an example:

`(lldb) io + [Tab] + [Enter]`

or, if only one command with prefix `io` in lldb environment, just issue:

`(lldb) io + [Enter]`

