# Upload-cars 🚗
Upload fivem cars

![image](https://raw.githubusercontent.com/rstacruz/hicat/gh-pages/hicat.gif](https://cdn.discordapp.com/attachments/919988260170772591/962395189895381103/venomm.png)

`Upload Fivem Cars` without any issues and what to see if there are any errors

```sh
Requirements:

OpenIV: https://openiv.org/

GTA 5: https://www.rockstargames.com/gta-v?info=order

Any vehicle file donwloaded is fine but I recommed: 

GTA5-Mods: https://www.gta5-mods.com/

Addon cars is what you are trying to mostly look for
```

Make a new folder in your PC recommend it to be the name of the car  ex. `hellcat2022`.
Inside that folder make a new folder called `stream` it must be called that

```sh
Please then open up OpenIV

At the top please click on Enable Edit Mode 

From there please now drag the file you just downloaded from the website
```

Now there will be a `dlc.rpf` file and that is what you will open up.

```sh
After opening up the dlc.rpf file go into the x64 folder 

Please grab all the .ytf and .ytd files and drag them in your folder you created and drop these files into the stream folder

Vehicle Mods is also where all the custom parts will be if your vehicle model does include those. Drag those files also into the stream folder

```

## Meta Files

```sh
Go back to the dlc.rpf file you have opened up and now click on the common folder that contain files ending in .meta

Please grab all the .meta files and drag them in your folder you created but not into the stream folder

```

## Resource.lua

Please create or download the `__resource.lua`.

```sh
In the main folder you created drag that __resource.lua file you created into it.

please paste the following if it is not contained

resource_manifest_version '77731fab-63ca-442c-a67b-abc70f28dfa5'
 
files {

    'handling.meta',
	'vehiclelayouts.meta',
    'vehicles.meta',
    'carvariations.meta',
    'carcols.meta',
    '**.meta',

    
}

data_file 'HANDLING_FILE' 'handling.meta'
data_file 'VEHICLE_LAYOUTS_FILE' 'vehiclelayouts.meta'
data_file 'VEHICLE_METADATA_FILE' 'vehicles.meta'
data_file 'CARCOLS_FILE' 'carcols.meta'
data_file 'VEHICLE_VARIATION_FILE' 'carvariations.meta'
```

## Uploading

If home hosted jusr drag and drop the file into your resource folder and simply add `ensure yourvehiclename`.

Other wise upload the folder into your FiveM server resources folder using a file trasnfer host such as FileZilla. 

You can find the cars name in-game by looking at the name of the file ending with .yft

Example `hellcat.yft ` or `lambo.yft`

## Issues

Current fivem can't stream files on serverside above 16MB. It's already known that the 16Mb limit is problematic.

IF your cars are above this 16MB limit please reduce the texture sizes in the ytd

What I use and recommend to use is https://www.xnview.com/en/xnresize/

Open the ytd file and extract all images as pngs

From there create a new folder that will contain the resized textures 

Use the resize tool recommend 50%

After completed please use openiv

Then use texture editor to open the ytd file, and upload the resized photos and your done!

