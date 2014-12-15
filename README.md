# How to Recompile (Linux)

```
# Make modifications to .lua files in /src
vim /src/main.lua

# Zip up game files into a Love archive
cd src/
zip -9 -q -r ../01.love .

# Create 32-bit Windows executable
cat platforms/win32/love.exe 01.love > build/win32/01.exe

# Copy over DLLs and license
cp platforms/win32/*.dll build/win32/
cp platforms/win32/license.txt build/win32/
```
