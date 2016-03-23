#Instructions to set up CanaryMod and Scriptcraft
The ultimate easy to follow guide to get started with CanaryMod and Scriptcraft

Thanks to the CanaryMod team and Walter Higgins for their great resources that allow kids to learn to build mods in Minecraft with Javascript code. The origin tutorial to get started with developing mods in Javascript using CanaryMod and Scriptcraft is here: https://github.com/walterhiggins/ScriptCraft/blob/master/docs/YoungPersonsGuideToProgrammingMinecraft.md

However, the tutorial skips over some crucial steps to setup CanaryMod and Scriptcraft that will get almost anybody running into several roadblocks. This is my version that adds a few extra steps to the original installation guide. 

##Installation

1. Download Java from the Java website and install it on your computer. This will allow you to run CanaryMod and Scriptcraft.

2. Once installation is complete, open your terminal by searching for `terminal` if you are on Mac or `cmd` if you're on Windows. The terminal is where your CanaryMod server will run while playing Minecraft. Type the command
`java` and hit the return key.
  
If you see the response below, it means Java has been installed successfully in your computer and the terminal can now recognize Java based commands.

3. Download CanaryMod from the following link http://scriptcraftjs.org/download/latest/
and Scriptcraft from the following link http://scriptcraftjs.org/download/latest/scriptcraft-3.2.0/. After downloading the files, rename the CanaryMod file as `canary.jar` (Trust me, this will make your life much easier in the future). 

4. Create a folder called `Canary` and copy your `canary.jar` and `scriptcraft.jar` files into the folder. 

5. While in your new `Canary` folder, double click your `canary.jar` file. This will initialize all the necessary folders and files to run CanaryMod on your computer. Move your `scriptcraft.jar` file to the plugins folder that has been created.


Start the CanaryMod server, then once it has started up, stop it by typing 'stop'. If you go to the CanaryMod folder (see step 1) you should see some new files and subfolders.

Download the latest version of the ScriptCraft Mod. Then copy the ScriptCraft.jar file to the plugins folder (This folder won't be created until you run CanaryMod for the first time (see previous step).

Start up the CanaryMod server again (see instructions for starting the server).

In the CanaryMod command window type op {your_username} and hit enter, replacing {your_username} with your own minecraft username. This will give you operator access meaning you can perform more commands than are normally available in Minecraft. You should make yourself a server operator (Server operators have full privileges for the server) permanently by editing the ops.txt file and adding your username (one username per line).

In the CanaryMod command window type js 1 + 1 and hit enter. You should see > 2 .

... Congratulations! You just installed your own Minecraft Server with the ScriptCraft Mod and are now ready to begin programming in Minecraft.



