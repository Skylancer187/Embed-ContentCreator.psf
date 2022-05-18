# Embed-ContentCreator.psf
Create easy to copy-paste base64 embedded content for powershell.

Strictly developed to include/embed content with my powershell code to avoid dependancies or network locations.

1. Open the app
2. Browse to the file you want to embed (larger files can bloat your script or IDE)
3. Click Encode
4. Copy Text (Base64) into a variable on your script.
5. Ex.  $base64 = [System.Convert]::$Content
        $ext = "txt"
        Set-Content -Path $DestinationPath\$filename.$ext -Value $base64 -Encoding Byte
        
Example use cases were for deploying configs, software installers, software depenancies, DLLs, shortcuts, etc.
