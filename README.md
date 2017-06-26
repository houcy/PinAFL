# PinAFL - AFL Fuzzer with Pin running on Windows!

-  Thanks for the great work: [AFL](http://lcamtuf.coredump.cx/afl/), [WinAFL](https://github.com/ivanfratric/winafl). I am planting AFL fuzzer to Windows with Pin, Intel's instrumentation tool.Before you are starting using this tool, I strongly advised you to learn [AFL fuzzer](http://lcamtuf.coredump.cx/afl/) first.

# Version

- 1.0.1

# Usage

- afl-fuzz [afl options] -- [Pin instrumentation options] -- target_cmd_line

**e.g.** afl-fuzz.exe -i input -o out -f input.txt -t 5000+ --  -coverage_module notepad.exe -cpukill -- notepad.exe @@

- Options for AFL:

  -i dir        - input directory with test cases

  -o dir        - output directory for fuzzer findings

  -t msec       - timeout for each run

  -f file       - location read by the fuzzed program


- Options for Pin:

  -coverage_module module     -  module for which to record coverage

  -cpukill                    - cpukill or not 



# Depends:

- None

# Change Log

- To be continued.


# Notes

- For now, it supports only 32-bit targets.


# UI

- <p align="center"><img src ="https://github.com/majinxin2003/PinAFL/blob/master/PinAFL.png" /></p>
