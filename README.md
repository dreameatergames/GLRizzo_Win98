# GLRizzo_Win98

This is the Windows 98 port of Rizzo Island. It uses a modified version of GLQuake compiled on Visual Studio 6.0 for Windows 98SE running on era appropriate hardware, and as such compiling instructions are for the VS 6.0 Source. It's more of a mod than a proper source port since only superficial things are modified like menus and sbar stuff, so it uses all the original GLQuake sources, and so far nothing from any other source port, though that is subject to change.

## Compiling Using Windows 98 and Visual Studio 6.0

### Pre-Requisites:

- Installed Visual Studio 6.0

- Windows 98SE Machine (or Virtual Machine)

- 98DDK.rar (The device driver sdk for Windows 98)

- 7-zip

### Compiling:

1. Use 7-zip to extract 98DDK.rar

2. Use 7-zip to open "Cabs\i386\BINS_DDK.CAB" and extract BINS_WIN98_ML.ERR and BINS_WIN98_ML.EXE

3. Change the names of BINS_WIN98_ML.ERR to ML.ERR and BINS_WIN98_ML.EXE to ML.EXE

4. Place them in the folder: C:\Program Files\Microsoft Visual Studio\VC98\Bin

5. Open up WinQuake.dsw in Visual Studio 6.0

6. Go into Build->Set Active Configuration and set it to gas2masm - Win32 Debug and press ok

7. Compile the gas2masm project

8. Once it's done compiling, go back to Build->Set Active Configuration and set it to winquake - Win32 GL Release and press ok

9. Compile the WinQuake project

If all goes well, you should have a working executable of Rizzo98 in the release_gl folder!