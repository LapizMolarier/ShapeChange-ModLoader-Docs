In order to create a C# MOD yourself you, uhhhhhhh, well l use Visual Studio 2019 (my ram screams help) and l do this:

 - Open VS 2019
 - Press "Create a new project"
 - In there, choose "Class Library (.NET Framework) C#"
 - Name it whatever you want, just make sure to choose .NET Framework 4.7.x
 - Press "Create"
 - You will need to add References. In template will be explained which ones and what everything does.
 - You might want a template on which you will work on:

using ShapeChange.ModAPI; //Inside Shape Change folder find Unity_Original or Unity_Older (depending on which version you want) and go into Shape Change_Data/DG_Shape_Change_Data folder, Managed, and find ModAPI.dll. Add it as a reference.

using UnityEngine; //Same thing but with UnityEngine.dll.

public class YourModName : Mod

{

    public override string Name => "MOD NAME";
    
    public override string Description => "MOD DESCRIPTION";
    
    public override int[] SceneUsage => new int[] { }; // leave it empty if you want your mod on every scene, put numbers in {} to start mod on set scenes. For example {0,4} will run mod on Scene 0 and 4.
   
    
    public override void OnLoad() // Starts on... Load! Shocking l know.
    
    {

        
    
    }

    
    public override void OnUpdate() //Does stuff repeatedly.
    
    {


   
    }
    
}
 - You can add other references from Managed folder OR, add from internet. Make sure to put reference file inside .zip of mod.
 - After you finished your project press Build - Build Solution.
 - If you did everything right, project will build properly.
 - Now, put it into .zip folder.
 - Create icon for it. (Or not. It will be white square tho.)
 - Put the icon as icon.png.
 - You are ready to go!
 - Go into APIReference.md because you can't properly mod without it.

All you need is Python.
Here's example script:
MOD_NAME = "Example"
MOD_DESCRIPTION = "Runs only on build index 0."
ALLOWED_SCENES = ["0"]  # can use names or build indexes

from UnityEngine import Debug
Debug.Log(f"[{MOD_NAME}] Running in allowed scene!")
You'll figure out everything else yourself, good luck! :)
(i lack a bit of instructions)

Lua, C mods are currently lacking ModCreation instructions. I have limited time, sorry.
