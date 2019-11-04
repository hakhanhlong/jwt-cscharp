
####### parameters run under CLI ########################
/*
* 
* jwt-csharp.
* Usage:
* jwt-csharp.exe [--key=<str>] [--issuer=<str>] [--username=<str>]
* jwt-csharp.exe (-h | --help)
* Options:
*  --key=<str>       path to private key
*  --issuer=<str>    issuer id from api connsole
*  --username=<str>  username if generating user token
*  -h --help         Show this screen.
*
*/



###### Project jwt-csharp #######################################

- Program write on Visual studio 2017, Console App
- Used net framework 4.6.1
- Package Library use to program:
	BouncyCastle 1.8.5 target net461
	jose-jwt 2.4.0 target net461
	Newtonsoft.Json 12.0.2 target net461

##### Project jwt-csharp-netcore ################################
- Program write on Visual studio 2017, Console App (Core)
- Used .net core 3.0
- Package Library use to program:
	BouncyCastle 1.8.5
	jose-jwt 2.4.0

How to build with Visual Studio Code:
    #1 Download .net core 3.0 (https://dotnet.microsoft.com/download/dotnet-core)
	#2 Download Visual Studio Code (https://code.visualstudio.com/)
	#3 Install Extension C# for VS Code (Extension: C# for Visual Studio Code (powered by OmniSharp).
	#4 From VS Code Open Folder jwt-csharp-netcore
	#5 Click View -> Terminal
	#6 Type for Build
	   dotnet build
	#7 Type for Run
		dotnet run --key=e:/jwtprivate.key --issuer=0098bef0-c3644110-9a8f-4021-b361-c3060de235f6
		or
		dotnet run --key=e:/jwtprivate.key --issuer=0098bef0-c3644110-9a8f-4021-b361-c3060de235f6 --username=hklong
	#8 Build to .exe 
	   dotnet publish -c Debug -r win10-x64 (debug build)
	   or
	   dotnet publish -c Release -r win10-x64 (release build)
	    







	   

	


