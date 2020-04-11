#### Command prompt
In an elevatated  prompt run either:
- ```wmic path Win32_OperatingSystem get LastBootUpTime ```
- ```systeminfo | find "System Boot Time" ```

#### PowerShell

```(get-date) - (gcim Win32_OperatingSystem).LastBootUpTime ```