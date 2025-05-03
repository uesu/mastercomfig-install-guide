<h1>
mastercomfig install
</h1>

<p> This guide should help people how to install mastercomfig.
</p>

<p> Big thanks to <a href="https://github.com/mastercoms">mastercoms</a> for making this.
</p>

[Video guide](https://youtu.be/JLrUDodt1sY)

**Note:**

* When updating mastercomfig (presets) you don't need to clean TF2 everytime, unless you have issues of course. If there is a new update on the website, you should take some time to read the changelog! there might be some adjustments that you need to change (the launch options would be an example). If you have any problems or concerns, you can ask questions on mastercoms [mastercomfig](https://discord.com/invite/CuPb2zV) discord server.

## Step 1:

Download [here](https://github.com/mastercomfig/mastercomfig/releases) or [here](https://comfig.app/)
 
* First, choose a preset, customize the preset and addons that you would like to use.

* Second, download it. Once downloaded, place the vpk files on your desktop, create a folder, name it **custom** and put the vpk files in the folder.
 
* Download the [overrides template](https://github.com/mastercomfig/mastercomfig/releases) (look for the most recent releases and download overrides template in assets), unzip and place the **overrides** folder on your desktop.

<table>
	<thead>
		<th>presets</th>
		<th>description</th>
	</thead>
	<tbody>
	<tr>
		<td>ultra</td>
		<td>
			absolute maximum quality, with even the slightest and most performance-intensive quality improvements included
		</td>
	</tr>
	<tr>
		<td>high</td>
		<td>
			enables all graphical features without making them extremely high quality
		</td>
	</tr>
		<tr>
		<td>medium high</td>
		<td>
			disables unoptimized features and optimizes the game without making the game look bad
		</td>
	</tr>
		<tr>
		<td>medium</td>
		<td>
			the maximum performance you can get while enabling a few effects that may give you a slight edge
		</td>
	</tr>
		<tr>
		<td>medium low</td>
		<td>
			the maximum performance you can get without making the game too hard to play because of awful visual quality and glitches
		</td>
	</tr>
		<tr>
		<td>low</td>
		<td>
			maximum performance without caring much about visibility or possible visual glitches
		</td>
	</tr>
		<tr>
		<td>very low</td>
		<td>
			negatively affects playability by a lot and disables very essential features like HUD elements in desperation for performance
		</td>
 	</tr>
		<tr>
		<td>none</td>
		<td>
			special preset which skips setting quality options
		</td>
	</tr>
	</tbody>
</table>

<table>
	<thead>
		<th>addons</th>
		<th>description</th>
	</thead>
	<tbody>
	<tr>
		<td>no footsteps</td>
		<td>
			no footstep sounds
		</td>
	</tr>
	<tr>
		<td>disable pyroland</td>
		<td>
			no pyroland map textures
		</td>
	</tr>
		<tr>
		<td>no soundscapes</td>
		<td>
			no ambient noises
		</td>
	</tr>
		<tr>
		<td>no tutorial</td>
		<td>
			no tutorial messages and other popups 
		</td>
	</tr>
		<tr>
		<td>low memory</td>
		<td>
			for those who have 4GB of ram and lower
		</td>
	</tr>
		<tr>
		<td>null - movement</td>
		<td>
			prevents you from pressing two opposite directions
		</td>
	</tr>
		<tr>
		<td>flat mouse</td>
		<td>
			flat, stable input, no accel, 1:1 zoom
		</td>
	</tr>
		<tr>
		<td>transparent viewmodels</td>
		<td>
			support for transparent viewmodels
		</td>
	</tr>
	</tbody>
</table>

**Note**: 

* If there is a new update, you should update your presets and addons. For instance, preset = low old version --> new version
* Addons are rarely updated, but if there is a new update, simply replace it.
 
## Step 2:
 
* Delete **cfg** & **custom** folder in tf folder.
 
* **Location** : `C:/Program Files (x86)/Steam/steamapps/common/Team Fortress 2/tf`
 
## Step 3:

Disabling **steam cloud** in `TF2` can help you reset it completely to it's original state.

* Disable **steam cloud on steam**.

		1. Go to the Steam Client Settings
		2. Select the cloud tab and uncheck the enable steam cloud synchronization
		
**Note:** This will disable all steam synchronization in your games. Enable it right away after completing the steps; alternatively, disable steam sync for TF2 only.

* Disable **steam cloud synchronization on TF2**.

		1. Right-click on Team Fortress 2 in your steam library and select properties
		2. In General, look for steam cloud text and uncheck "Keep game saves in the Steam Cloud for Team Fortress 2"
                
* Make all the files in `C:/Program Files (x86)/Steam/userdata/user_id/440/remote/cfg`
 
       remove everything inside the cfg, save and close but don't delete the cfg
                  
**Note:** 

* If the **remote folder** contains no cfg file, you have already disabled steam cloud.
 
## Step 4:
 
* Verify Game File Integrity:
 
		1. Right-click on Team Fortress 2 and select properties
		2. Select the installed files tab and click verify integrity of game files
		3. Wait for it to be done
 
## Step 5:
 
* After checking the integrity of the game files, go to the properties of TF2, copy and paste to the launch option.
  
`-novid -autoconfig -default +host_writeconfig config.cfg full +mat_savechanges +quit`

**Note:**

* Launch TF2, the game will launch and exit afterwards. remove these launch options after.
 
## Step 6:
 
* Go to TF2 properties again, copy and paste **(may change https://docs.comfig.app/latest/customization/launch_options/)**

`-novid -nojoy -nosteamcontroller -nohltv -particles 1 -precachefontchars`

## Step 7: Optional
 
* Select which dxlevel best performs for you:

<table>
	<thead>
		<th>dxlevels</th>
		<th>description</th>
	</thead>
	<tbody>
	<tr>
		<td>dxlevel 90</td>
		<td>
			directX 9, Pixel Shader 2.0b. Lower graphical quality while still using semi-modern rendering methods
		</td>
	</tr>
	<tr>
		<td>dxlevel 100</td>
		<td>
			directX 9+, Pixel Shader 3.0. Highest graphical quality
		</td>
	</tr>
	</tbody>
</table>

**Note:** 

* remove the `-dxlevel` launch option after the first launch as stated on the official documentation
* dxlevel 8 or 80 and 81 is not recommended, especially for competitive matches?
* more info about dxlevel 8: https://docs.comfig.app/latest/customization/launch_options/#directx-8

##
 
* **-w and -h** -> removed; instead you should change the resolution in the game.
 
With the in-game resolution settings, you can set your resolution to `mat_setvideomode 1920 1080 0` within the console. Change `1920 1080` to your desired resolution.
 
## Step 8: Installation of Custom/Own cfg, Mastercomfig Presets and Addons
 
* Place the **overrides** folder to `tf/cfg` and **vpk files** to `tf/custom`
 
* **Location** : 
  - `C:/Program Files (x86)/Steam/steamapps/common/Team Fortress 2/tf`
  - `C:/Program Files (x86)/Steam/steamapps/common/Team Fortress 2/custom`

* Launch **Team Fortress 2**
