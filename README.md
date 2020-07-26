# UnrealTopDownGame

Simple blueprint project from UE templates.

To build game outside the Unreal Editor you can use this pattern:
```c++
[UE4Path]/Engine/Build/BatchFiles/RunUAT.batBuildCookRun
-project=[projectPath].uproject
-platform=[Platform]
-clientconfig=[Configuration]
-archivedirectory=[archiveProjectPath]
-[buildArgs]
```

Example:
```c++
"c:/Epic Games/UE Binary/UE_4.25/Engine/Build/BatchFiles/RunUAT.bat" BuildCookRun
-project=c:/_Projects/_Jenkins/UnrealTopDownGame/UnrealTopDownGame.uproject
-platform=Win64 
-clientconfig=Development
-archivedirectory=c:/_Projects/_Jenkins/UnrealTopDownGame/Build
-cook -stage -archive -pak -package -allmaps
```
