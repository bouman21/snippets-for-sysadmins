```
@echo off
for /F "usebackq tokens=1,2,3,4,5*" %%i in (`query user 2^>nul`) do (
    if "%%l" == "Active" ( echo A: %%i )
    if "%%k" == "Disc" ( echo D: %%i )
)
```