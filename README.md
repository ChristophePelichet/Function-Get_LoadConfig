# Function Get_LoadConfig

## Description 
- Simple function to load a variable configuration file external to the script.

## Use Function 
- Before you can load your external configuration file, you must add these 2 lines at the beginning of your script before the code to execute.

$MYFunctionPath  = $MyScriptPath + "\Functions"
$MyConfPath      = $MyScriptPath + "\Config\config.xml"

- You can change the variable name and the path if you want.  

- After adding this 2 line you can load your configuration with this code 

$MyLoadConf = $MYFunctionPath +"\"+ "Get_LoadConfig.ps1"
	. $MyLoadConf
	Get_LoadConfig -path $MyConfPath

## Changelog
- V1.01 - 03.10.2020 - Update Information and clean code
- V1.00 - 03/10/2020 - Initial version
