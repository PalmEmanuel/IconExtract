# IconExtract

Quick and dirty implementation of the code at https://www.lluisfranco.com/extract-icons-win32/ to extract icons as images from files.

```PowerShell
# Example code
dotnet publish
Import-Module .\IconHelper\bin\Debug\net7.0\IconHelper.dll
$Bitmap = [IconHelper.IconHelper]::GetFileImageFromPath("C:\Temp\MyPowerShellModule.psd1", [IconHelper.IconHelper+IconSizeEnum]::ExtraLargeIcon)
$Bitmap.Save('C:\Temp\Psd1Icon.png', [System.Drawing.Imaging.ImageFormat]::Png)
```
