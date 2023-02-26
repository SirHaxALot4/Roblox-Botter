# Roblox-Botter 
<img src="https://vignette.wikia.nocookie.net/roblox/images/4/47/GREEN_SCAMMER_BOT.png/revision/latest" style="height: 10%"> 
Make accounts join games and control what they do with chat commands! <br>
The instructions below are listed in order of steps so make sure to follow them!

<br><br>

<b>```! AUTO ATTACH IN EXPLOITS FOR MUTIPLE CLIENTS IS BECOMING UNSTABLE!``` <br>
```A V2 WILL BE MADE SOON AND SHOULD BE EASY TO GET WORKING ON LINUX```

```This means, the bots can only be used for spamming sadly but this should still work```</b>


<br>

# Requirements:
<ul>
  <li>  <a href="https://www.python.org/"> Python 3.8 > </a> </li>
  <li> <b> Python Packages: </b> time, requests, pathlib, urllib.parse, os, threading </li>
  <li> A Roblox exploit that supports Autoexec <b> (<a href="https://x.synapse.to/">Synapse</a>: Paid or <a href="https://krnl.dev/">Krnl</a>: Free) </b> </li>
  <li> <a href="http://www.editthiscookie.com/"> Edit this cookie </a> </li>
  <li> <a href="https://wearedevs.net/dinfo/Multiple%20Games"> Muitiple rbx </a> </li>
  <li> A python IDE, (I'd recomend <a href="https://www.jetbrains.com/pycharm/">Pycharm</a>) </li>
</ul>

<br>
<br>

# Installing Python
Go to https://www.python.org/ and install the latest version (3.11 recomended) and make sure to add it to Path! You may need to restart afterwards.

Check if python is installed by typing `python -h` in Commmand prompt.

Python should pip <b>(Python's package manager)</b> as well, so let's check if it installed as well. To do this run `pip -h` in Command prompt. <br>
If pip as installed sucessfully, run `pip install requests pathlib`. This will install the required packages.

<br>
<br> 

# Grabbing the Roblox account's cookie
For this you need <a href="http://www.editthiscookie.com/"> Edit this cookie </a> or simular to browse cookies.

Locate `.ROBLOSECURITY` and copy it's value <br>

<img style="width: auto; height: 600px" src="https://user-images.githubusercontent.com/86912923/203606748-0959fd14-50fa-4391-9df7-44897789b3d6.png"/>
<br><br>

**WARNING** If you log out of the account, the cookie will become invalid! Instead, set `.ROBLOSECURITY`'s value to ` `&nbsp;and click the green arrow icon on the bottom of the menu (Shown in picture above).

<br><br>

## Adding the cookie

In the cookie array, add the cookie's value as a string. <br>

<img src="https://user-images.githubusercontent.com/86912923/215582485-ad6504d4-3892-4381-869e-68ecba26e711.png" style="width: 70%"/>

<br>

To format muitple cookies, I have list an example below.

```
config = {
    "Cookies": [
        ".ROBLOSECURITY Here",
        ".ROBLOSECURITY Here",
        ".ROBLOSECURITY Here"
    ]
}
```
<b> The last line should not incude a `,` at the end of the line otherwise it will result in a syntax error. </b>

After this, change the `Bot` variable to the amount of bots you want! <b>(The max amount is how many cookies you provided)</b>

<br>
<br>

# Adding the bot controler

Locate your exploit's autoexec folder and drag n drop `BotControler.lua` into it. <br>

![image](https://user-images.githubusercontent.com/86912923/203608146-39e8323d-c0af-420c-9abb-56ad4e42f257.png)

<br>
<br>

# Botting a game

Once you have compleated the steps above, copy your Roblox's username `NOT DISPLAY NAME` to be added to the permission list in `BotControler.lua`.
Once copyied paste it into the table and save the file. <br>

<img src="https://user-images.githubusercontent.com/86912923/215581093-8534ab54-a4e8-4acd-8996-a76253582321.png" style="width: 70%"/>


Open your exploit and MuitRBX, join the game you would like to bot. Once in the game execute a script like <a href="https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source">Infinite Yield</a> and copy the game's Jobid and paste it into the python script and reduce it to the image shown below on line 3. <br>

<img src="https://user-images.githubusercontent.com/86912923/215581693-027b0dac-4007-4f19-a19d-7dc5ad762738.png" style="width: 70%"/>

Run the python script and enjoy.

# Commands

<b> NOTE: Player names can be shortened! </b>
Each argument is seperated by `, `

```
Unlock, (true/false) | Wether all players have permission to use the bots.
Come, (PlayerName) | Teleports all bots to a player | Stop `Come, `
Say, (Msg) | Make the bots say a message.
Say, loop, (Msg) | Make the bots spam a message. | Stop `Say, .`
chatmode, (Mode) | Change the Chat mode e.g `All, General`
Rejoin | Make the bots rejoin the game.
Follow, (Player name) | Make the bots follow a player. | Stop `Follow, `
```
