# mastercomfig install

This guide should help people how to install mastercomfig.
 
Big thanks to [mastercoms](https://github.com/mastercoms/) for making this config.

**Note:**
 
* When updating mastercomfig, you don't have to clean TF2. If there is a new update on the site, you should take some time to read what changes have been made and change if there are any changes `(the launch options would be an example)`. If you have any problems or concerns, you can ask questions on mastercoms (mastercomfig) discord server.

## Step 1:
 
https://github.com/mastercomfig/mastercomfig/releases
 
* First of all, download which preset and addons you want to use, it should be in the assets, click the file and it will be downloaded.

* Once downloaded, place the `vpk files` on your `desktop`, create a `folder`, name it `custom`, put the `vpk files` in the `folder`.
 
* Download the `cfg template`, place the `user folder` on your `desktop.`

[cfg template](https://mega.nz/file/RxcnVYyZ#7lXwIrEWpWOX2u7drC5Ua9kxj59LUXOFHS6oox5DKBY/)
 
## Step 2:
 
* Delete `cfg` & `custom` folder in `tf` folder.
 
* **Location** : `C:/Program Files (x86)/Steam/steamapps/common/Team Fortress 2/tf`
 
## Step 3:
 
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

* Start `TF2`, the game will launch and exit afterwards. remove these launch options after
 
## Step 6:
 
* Go to the TF2 properties again, `copy and paste` into the launch option: `(subject to change)`

`-novid -nojoy -nosteamcontroller -nohltv -particles 1 -console -dxlevel 81 -freq 144`
 
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
