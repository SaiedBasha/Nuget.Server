# Nuget.Server

##To package a class library project and push to server:
1.	Download nugget.exe from https://www.nuget.org/downloads
2.	Add it’s path to system environment path
3.	From the project folder run this command “nuget pack <project name>.csproj -Properties Configuration=Debug”
4.	To push it to server “nuget.exe <generated package name>.nupkg <api key> -Source http://<server url>/nuget”


##To add the local server to nuget package sources
1.	Visual Studio > Tools > Options > NuGet Package Manager > Package Sources > New
2.	Give it a name and source http://<server url>/nuget
