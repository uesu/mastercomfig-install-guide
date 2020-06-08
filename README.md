<h1 align="center">
mastercomfig install
</h1>

<p align="center">This guide should help people how to install mastercomfig.
</p>

<p align="center">Big thanks to
	<a href="https://github.com/mastercoms">mastercoms</a> for making this config.
</p>

**Note:**
 
* When updating mastercomfig, you don't have to clean TF2. If there is a new update on the site, you should take some time to read what changes have been made and change if there are any changes `(the launch options would be an example)`. If you have any problems or concerns, you can ask questions on mastercoms (mastercomfig) discord server.

## Step 1:

Download [here](https://github.com/mastercomfig/mastercomfig/releases) or [here](https://mastercomfig.com/download)
 
* First, download which preset and addons you want to use, it should be in the assets, click the file and it will be downloaded.

* Once downloaded, place the `vpk files` on your `desktop`, create a `folder`, name it `custom` and put the `vpk files` in the `folder`.
 
* Download the `user template`, place the `user folder` on your `desktop.`

[user template](https://mega.nz/file/ows0nAqY#jpgJKNTbbRo2tkhbacO84oisfuXu7Ip3KhkuCGSnrE0/)

<table>
	<thead>
		<th>presets</th>
		<th>description</th>
	</thead>
	<tbody>
	<tr>
		<td>ultra</td>
		<td>
			absolute maximum quality
		</td>
	</tr>
	<tr>
		<td>high</td>
		<td>
			high quality
		</td>
	</tr>
		<tr>
		<td>medium high</td>
		<td>
			higher medium preset nearly equal with high
		</td>
	</tr>
		<tr>
		<td>medium</td>
		<td>
			medium quality with adjustable effects
		</td>
	</tr>
		<tr>
		<td>medium low</td>
		<td>
			medium low quality 
		</td>
	</tr>
		<tr>
		<td>low</td>
		<td>
			maximum performance
		</td>
	</tr>
		<tr>
		<td>very low</td>
		<td>
			same as low but disabled parts of hud elements and visibility
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
		<td>bad gpu</td>
		<td>
			for those who have weak graphics cards 
		</td>
	</tr>
		<tr>
		<td>low memory</td>
		<td>
			for those who have 4GB of ram and lower
		</td>
	</tr>
	</tbody>
</table>
 
## Step 2:
 
* Delete `cfg` & `custom` folder in `tf` folder.
 
* **Location** : `C:/Program Files (x86)/Steam/steamapps/common/Team Fortress 2/tf`
 
## Step 3:

* Disable **steam cloud on steam**.

		1. Go to the Steam Client Settings
		2. Select the cloud tab and uncheck the enable steam cloud synchronization

* Disable **steam cloud synchronization**.

		1. Right-click on Team Fortress 2 and select properties
		2. Select the updates tab and uncheck the enable steam cloud synchronization
                
* Make all the files in `C:/Program Files (x86)/Steam/userdata/user_id/440/remote/cfg`
 
       remove everything inside the cfg, save and close but don't delete the cfg
                  
**Note:** 

* If the **remote folder** contains `no cfg` file, you have already `disabled steam cloud`.
 
## Step 4:
 
* Verify Game File Integrity:
 
		1. Right-click on Team Fortress 2 and select properties
		2. Select the local files tab and click verify integrity of game files
		3. Wait for it to be done
 
## Step 5:
 
* After checking the integrity of the game files, go to the properties of TF2, `copy and paste` into the launch option:
  
`-novid -autoconfig -default +host_writeconfig config.cfg full +mat_savechanges +quit`

**Note:**

* Start `TF2`, the game will launch and exit afterwards. remove these launch options after.
 
## Step 6:
 
* Go to the TF2 properties again, `copy and paste` into the launch option: `(subject to change)`

`-novid -nojoy -nosteamcontroller -nohltv -particles 1 -console -dxlevel 81 -w 1366 -h 768 -freq 144`
 
* Select which dxlevel best performs for you:

<table>
	<thead>
		<th>dxlevels</th>
		<th>description</th>
	</thead>
	<tbody>
	<tr>
		<td>dxlevel 81</td>
		<td>
			DX8 with dynamic shadows
		</td>
	</tr>
	<tr>
		<td>dxlevel 100</td>
		<td>
			dxlevel 95 with unrestricted GPU feature level support (DX10 card support)
		</td>
	</tr>
	</tbody>
</table>

`dxlevel 81 disables sheens, skins and visual resulting to produce a lower quality graphics.`

**Note:** 

* Remove the `-dxlevel` after the first launch.

##
 
* **-freq x** : If you have a monitor with 144Hz, do **-freq 144**

`this applies only if TF2 does not automatically detect the refresh rate on your monitor`
      
##
 
* **-w and -h** : are removed; instead you should change the resolution in the game.
 
With the in-game resolution settings, you can set your resolution to `mat_setvideomode 1920 1080 0` within the `console`. Change `1920 1080` to your desired resolution.
 
[launch options](https://docs.mastercomfig.com/en/stable/customization/launch_options/)
 
## Step 7:
 
* Place the `user folder` to `tf/cfg` and `vpk files` to `tf/custom`
 
* **Location** : `C:/Program Files (x86)/Steam/steamapps/common/Team Fortress 2/tf`

* Launch **Team Fortress 2**
