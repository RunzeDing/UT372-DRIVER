# UT372-DRIVER
A driver for tachometer UT372 writen in C# based on [HIDLibray](https://github.com/mikeobrien/HidLibrary), which can read the real time RPM and send it by UDP packets.
UT372 has an official windows interface but do not support real time data feedback. This driver will read packets from USB and decode it by its protocool.


## How to use
1. Build the solution(You may modify the IP addr and portal if you would like to send in UDP)
2. Plugin UT372
3. Run solution.exe
4. Run UT372's interface, and click "connect", and this will send a enable signal to UT372.
5. The RPM data would send in a 5 bytes string packet

## Protocool

