memscan
=======

`memscan` is a command line utility for scanning a process's memory. It is compatible with 64-bit Windows, and will not work on 32-bit Windows. 

### Usage

Start a memory scan for a process with 

`memscan -cmd <processName>`

That will start a memory scan for the process with default settings.

If you want to specify a value to scan for, enter

`memscan -cmd <processName> -v <value>`

You can also specify the combination of memory units you want to scan for (e.g., bytes, words (16-bits), dwords (32-bits), and quadwords (64-bits)). The flags `-b`, `-w`, `-d`, and `-q` correspond to memory unit byte, word, dword, and quadword respectively. Simply combine the flags and add them to the end of the command line statement to scan for these memory units. E.g., 

`memscan -cmd <processName> -dq`

Would scan the process for dwords and quadwords.
