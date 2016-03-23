##Setting up CanaryMod and Scriptcraft
This the ultimate easy-to-follow guide to get started with CanaryMod and Scriptcraft. 

Thanks to the CanaryMod team and Walter Higgins for their great resources that allow kids to learn to build mods in Minecraft with Javascript code. The origin tutorial to get started with developing mods in Javascript using CanaryMod and Scriptcraft is here: https://github.com/walterhiggins/ScriptCraft/blob/master/docs/YoungPersonsGuideToProgrammingMinecraft.md

However, the tutorial skips over some crucial steps to setup CanaryMod and Scriptcraft that will get almost anybody running into several roadblocks. This is my version that adds a few extra steps to the original installation guide. 

##Installation

1. Download `Java` from the Java website and install it on your computer. This will allow you to run CanaryMod and Scriptcraft.

2. Once installation is complete, open your terminal by searching for `terminal` if you are on Mac or `cmd` if you're on Windows. The terminal is where your CanaryMod server will run while playing Minecraft. Type the command
`java` and hit the return key. If you see the response below, it means Java has been installed successfully in your computer and the terminal can now recognize Java based commands. <img width="827" alt="java" src="https://cloud.githubusercontent.com/assets/7483633/13989096/4ab4ef88-f128-11e5-925c-5b4c0a8bb35b.png">

3. Download CanaryMod from the following link http://scriptcraftjs.org/download/latest/
and Scriptcraft from the following link http://scriptcraftjs.org/download/latest/scriptcraft-3.2.0/. After downloading the files, rename the CanaryMod file as `canary.jar` (Trust me, this will make your life much easier in the future). 

4. Create a folder called `Canary` in your desktop and copy your `canary.jar` and `scriptcraft.jar` files into the folder. 

5. In your new `Canary` folder, double click your `canary.jar` file. This will initialize all the necessary folders and files to run CanaryMod on your computer. Move your `scriptcraft.jar` file to the `plugins` folder that has been created.

6. In `Canary` folder, open the `eula.txt` file with any text editor. Find the line that has the value `false` and change it to `true` and save the file.

##Final Steps
1. Back in your terminal, navigate to the `Canary` folder by typing in the following command `cd desktop/canary`. Now you are accessing your `Canary` folder in your terminal. 

2. Type the command `java -jar canary.jar` to start the CanaryMod server. Once the server is running you should see something similar to the output below <img width="804" alt="screen shot 2016-03-23 at 7 47 37 pm" src="https://cloud.githubusercontent.com/assets/7483633/13991087/2e09c928-f130-11e5-8d8b-0e1092e4b028.png">

3. Type the command `js 1+1` and it should return `2.0`. This means `scriptcraft` is now being recognized as a plugin by your CanaryMod server. 

4. Now this is when `Minecraft` comes into the picture. Open `Minecraft` and wait for the launcher. Click `Edit Profile` and select `1.8.9` for `Use Version` and then click `Save Profile`.

5. Click `Play`. Once the game menu appears, select `Multiplayer` and then click `Add Server`. 

6. Give your server a name and for your server address type `localhost` and click `Done`. Select your created server and click `Join Server` to join the game on our CanaryMod server.

7. While the game is running, back in your terminal, type `op YOURUSERNAME`. Finally, add permission to use `scriptcraft` in the game by typing the following command `groupmod permission add admins scriptcraft.evaluate`. 

8. And we're done! try typing `js 1+1` in the game and you should see `2.0`. To see what you can do with Scriptcraft start here https://github.com/walterhiggins/ScriptCraft/blob/master/docs/YoungPersonsGuideToProgrammingMinecraft.md#variables

##Configuring our CanaryMod server

In order to build our mods in peace, we want to configure our world to be flat and play in creative mode as well as not be bothered by creatures. Based on the original tutorial, I tried configuring the server file found in the `config` folder before ever running the server in the terminal and none of the changes I made were ever reflected. 

1. Now that we have the game running with CanaryMod server and Scriptcraft, we can disconnect from the game menu as well as stop the server running in the terminal by hitting `ctrl + c`.

2. In your `Canary` folder delete the `Worlds` folder. 

3. Go to `config/worlds/default` and open `default_NORMAL.cfg` and change values for the following lines as below:
```
# completely flat worlds are best for building from scratch
# bukkit/spigotmc
level-type=FLAT
# canarymod
world-type=FLAT
generate-structures=false

# creative mode
gamemode=1
pvp=false

# turns off authentication (for classroom environments)
online-mode=false
spawn-npcs=false
spawn-monsters=false

```
..and save the file.

Run the `java -jar canary.jar` command again in the terminal and you should be good to go!







