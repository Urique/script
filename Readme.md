Info
----
This script obtains links from Microsoft's API and then writes them to file.<br>
Currently it is based on cUrl and Bash (on Windows it uses BusyBox).

tbdump.sh 			- Shell script version of TechBench dump. Obtains links from API, and then writes them to formatted file<br>
techbench.cmd		- Runs shell script on Windows and configures it to generate HTML file<br>
techbench_md.cmd	- Runs shell script on Windows and configures it to generate Markdown file (GitHub paste format)

Usage
-----
### Windows
Simply run desired cmd script, it will generate everything automatically.<br>

Command line usage:
```
<script.cmd> [first_id] [last_id]
```

Example command to create HTML file with products from range between 242 and 247:
```
techbench.cmd 242 247
```

### Everything else with bash support
Give execute permission to file and run it with desired parameters.<br>

Command line usage:
```
<./script.sh> generator [first_id] [last_id]
```

Example command to create HTML file with products from range between 242 and 247:
```
./tbdump.sh html 242 247
```

Test packages [![build status](https://gitlab.com/techbench-dump/script/badges/master/build.svg)](https://gitlab.com/techbench-dump/script/commits/master)
-------------
If you want to test newest version of script you can download test package from [GitLab](https://gitlab.com/techbench-dump/script/builds/artifacts/master/browse?job=package).

TechBench dump website
----------------------
Website: https://mdl-tb.ct8.pl/<br>
Markdown: https://mdl-tb.ct8.pl/dump.md<br>
GitHub: https://github.com/techbench-dump/website

Credits
-------
WzorNET - finding out that TechBench contains more than Windows 10.<br>
Ron Yorston - BusyBox port for Windows. https://frippery.org/busybox/<br>
Marc Hörsken - curl binaries for Windows. https://dl.uxnr.de/build/curl/<br>
