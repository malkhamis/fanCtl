1) i8kutils does not work with Dell T7500 Workstation out-of-the-box as it was meant for laptops.

2) CPU temperature monitoring and CPU fan adjustment is handled by software in the Dell T7500 Workstation.

3) If you are running a Linux machine and impressed by how quite the T7500, you later may not be impressed after your machine breaks down!

4) You need the following packages to be installed for this script to work: i8kutils, lm-sensors.

5) Do not change the "# Default-Stop" and "# Default-Start" parameters. If you let the script run at the OS run-level 0 & 6, your machine will no longer be able to shut down and restart normally since the script has an infinite loop.

6) Remember that you need to put this script in /etc/init.d and ensure that the script is executable so that it is loaded at boot time

7) a one second delay between temperature checks works fine with me, but feel free to adjust it to your needs, but setting it too short might defeat the purpose as you don't want to heat the CPU for checking its temperature :-)

8) Enjoy the noise if you haven't heard it yet :D
