<h1 align ="center">Material Texture Loader</h1>
<div align="center">Advanced material creation plugin for 3ds max</div>
<div align="center"><a href="https://youtu.be/WaiYY6T3cwg?si=zFbhcXlvGxeUF19K">Youtube</a> - <a href="https://dmz.gumroad.com/l/MaterialTextureLoader">Gumroad</a> - <a href="https://www.scriptspot.com/3ds-max/scripts/material-texture-loader">Scriptspot</a></div>

***
### Table of contents
- [Support](#support)
  - [Renderers](#renderers)
  - [Installation](#installation)
  - [Add a button after installation](#button)
  - [Create custom Naming Filters](#namingFilters)
- [User Interface](#ui)
  - [Top Menu](#ui_topmenu)
  - [Channels](#ui_channels)
  - [Channel Settings](#ui_channelsettings)
  - [Maps](#ui_maps)
  - [Material](#ui_material)
  - [Slot](#ui_slot)
  - [Modifiers](#ui_modifiers)

### Description <a name="description"></a>
Documentation for UI an maxScript API.  
Material Texture Loader is a plugin for 3ds Max that creates advanced material setups from textures sets.
***

# Support <a name="support"></a>
- 3ds Max 2016-2025

### Renderers <a name="renderers"></a>
- Vray(v3-6)
- Corona(v5-10)
- Redshift
- Arnold
- FStorm
- Octane
- Physical, PBR and Standard
<h2> </h2>

### Installation <a name="installation"></a>
1. Drag and Drop the latest version of "MTL_v1.x install.mzp" into the 3ds max viewport.
    Or run the script inside 3ds max. Scripting > Run Script > select "MTL_v1.x install.mzp" > Open
2. On succesfull install, press Open MTL to start using the script.

### Add a button after installation <a name="button"></a>
1. Restart 3ds Max.
2. In 3ds Max go to Customize > Customize User Interface > Toolbars > Category > DMZ.
3. Drag "Material Texture Loader" into a toolbar. 
<h2> </h2>

### Create custom Naming Filters <a name="namingFilters"></a>
1. Go to your 3ds max userscripts folder, DMZ folder (eg: C:\Users\[Username]\AppData\Local\Autodesk\3dsMax\2018 - 64bit\ENU\userscripts\DMZ\MTL\namingFilters),
2. Any .ini file (eg. 'nameFilter_01 Default.ini') needs to be placed in that folder and must start with 'nameFilter_'.
3. Do not change the naming of the channels inside the file (eg. 'diffuse=', 'ambient=').
4. Add any word after the equal ('=') character, separated by a comma (','). These words are used to select textures for the right channel.
5. You can have up to 12 different .ini naming filter files, which all can be separately activated and combined in the MTL.

***
<h1>User Interface</h1><a name="ui"></a>
<img src="images/TopMenu_001.jpg" align="right" width="400"></img>
<h3>Top Menu</h3><a name="ui_topmenu"></a>
<details>
  <summary><b>Load New Textures</b>: Open texture file browser to select new files</summary>

  > You can multi-select any 3ds max supported image files.  
  > Selected files will be place in the Texture Channels dropdown list.  
  > Previously loaded files will be removed. Active Naming Filters will be used to automatically assign textures to Channels.  
  > Active Naming Filters will be used to automatically assign textures to Channels.  
</details>
<details>
  <summary><b>Add Extra Textrues</b>: Open texture file browser, to select additional files</summary>

  > You can multi-select any 3ds max supported image files.  
  > Selected files will be added to the Texture Channels dropdown list.  
  > Active Naming Filters will be used to automatically re-assign textures to Channels.  
  > Load New Textures: Open texture file browser to select new files.  
</details>
<details>
  <summary><b>Use All Channels</b>: Activate all texture Channels</summary>

  > When materials don't use every texture channel, this will make all Texture Channel available.  
  > Maps that are created in this way are accessable after pressing Add Material to Compact / Add Material to Slate.  
  > Maps will be placed adjacent to the material that is created.  
</details>
<details>
  <summary><b>Reset</b>: Reset entire UI back to Deafult</summary>

  > Selects Default as Preset  
  > Clears all image files from Texture Channels  
  > Clears Material Slot  
</details>
<details>
  <summary><b>Naming Filters</b>: Select active Naming Filters</summary>

  > Naming FIlters are used for automatic Texture Channel selection.  
  > You can activate any combination of listed Naming Filters.  
  > Up to 10 nameFilter files in nameFilters directory will be listed.  
</details>
<details>
  <summary><b>MTL Installer</b>: Opens Installer menu</summary>

  > Contains Uninstall option and a list of all plugin installation directories.  
</details>
<details>
  <summary><b>Preset</b>: Dropdown list of all saved settings</summary>

  > Switching Presets will change all settings directy.  
  > When Update is active, you can still switch Presets. Material type will be locked to current Material.  
</details>
<details>
  <summary><b>Save Preset</b>: Save current settings</summary>

  > Opens a Preset Name menu, where you can save the Current Settings under the given name.  
  > If Preset name already exists, menu will ask if you want to overwrite existing Preset.  
</details>
<details>
  <summary><b>Dockable</b>:Switch between dockable and window dialog mode</summary>

</details>
<h2> </h2>
<img src="images/Channels_001.jpg" align="right" width="400"></img>
<h3>Channels</h3><a name="ui_channels"></a>
<details>
  <summary><b>Enable/Disable Channel</b>: Disable or enabled a channel from creating maps</summary>

  > Disabeling channels will disable all other Channel controls.  
  > When disabled no maps are created, even when a texture file is selected in the dropdown list.  
  > Channel will be disabled automatically when a material type does not support the channel.  
  > You can force every channel to be active by checking Use All Channels (see: Top Menu - Files).  
</details>
<details>
  <summary><b>Channel Texture</b>: Select a texture file for the channel from the dropdownlist</summary>

  > For selected tecxture files a texture map will be created and connected to the material.  
  > Texture files will be available when loaded in with Load New Textures or Add Extra Textrues.  
  > Select empty item to deselect any texture file. No map will be created for this channel.  
</details>
<details>
  <summary><b>Channel Strength</b>: Set the strength or influence of the texture image</summary>

  > Control will be disabled when material type does not have support for Texture Strength.  
</details>
<details>
  <summary><b>Channel Settings</b>: Button that displays channel name and opens channel specific settings</summary>

  > (see: Channels - Settings.)  
</details>
<details>
  <summary><b>Show Channel</b>: Show channels texture map in viewport</summary>

  > Only 1 channel can be displayed in viewport.  
  > Only works when a material is created.  
</details>
<h2> </h2>
<img src="images/Channels_Settings_001.jpg" align="right"></img>
<h3>Channel Settings</h3><a name="ui_channelsettings"></a>
<details>
  <summary><b>Color Space</b>: Choose between different type of color space input for texture file.</summary>

</details>
<details>
  <summary><b>Auto linear-sRGB</b>: when sRGB Color Space is selected and 32bit images are loaded, load files as linear-sRGB.</summary>

</details>
<details>
  <summary><b>Gamma</b>: Gamma input value for texture file.</summary>

</details>
<details>
  <summary><b>Color Correction</b>: Inlcude a color correction map for the texture channel.</summary>

</details>
<details>
  <summary><b>Inver Color</b>: Invert the colors of the texture channel.</summary>

  > Will add an extra map to invert colors, or use existing map settings if possible.  
</details>
<details>
  <summary><b>Set</b>: Accepts the current settings for the texture channel.</summary>

  > Click the 'X' icon if you wish to cancel setting changes.  
</details>
<h2> </h2>
<img src="images/Maps_001.jpg" align="right"></img>
<h3>Maps</h3><a name="ui_maps"></a>
<details>
  <summary><b>Map Type</b>: Choose between standard and render specific texture map</summary>

  > Render specific texture maps will be selected based of the material type selected.  
  > Not all renderers support standard Bitmaps.  
</details>
<details>
  <summary><b>Blur</b>: Blur value applied to each texture map</summary>

  > Blur is applied to all channels equally. There is no option for channel specifc blur values.  
</details>
<details>
  <summary><b>Mapping Channel Set mapping channel for all texture maps</b>:</summary>

  > Tile mapping:  
  > Real-world mapping: Tri-planar mapping: Spherical mapping:  
</details>
<details>
  <summary><b>Mapping Type</b>: Set the mapping type for each texture map</summary>

</details>
<details>
  <summary><b>Size</b>: set U and V mapping size</summary>

</details>
<details>
  <summary><b>Non-Uniform Size</b>: Enable</summary>

</details>
<h2> </h2>
<img src="images/Material_001.jpg" align="right"></img>
<h3>Material</h3><a name="ui_material"></a>
<details>
  <summary><b>Active Render Material</b>: Set Material Type to active renderer.</summary>

  > When active automatically switches Material Type when renderer is changed.  
  > Will de-activate when activating Update and existing material is not compatible will active Renderer.  
</details>
<details>
  <summary><b>Material Type</b>: Select from dropdown list with any supported materials.</summary>

  > De-activates Active Render Material when you select other material type that is compatible with the active renderer.  
</details>
<details>
  <summary><b>Diffuse</b>: Set the materials base diffuse color</summary>

</details>
<details>
  <summary><b>Reflection</b>: Set the materials base reflection color</summary>

</details>
<details>
  <summary><b>Glossiness</b>: Set the materials base glossiness value</summary>

</details>
<details>
  <summary><b>Refl. IOR</b>: Set the Materials base IOR value</summary>

  > Uncheck checkbox will set IOR value to the materials max IOR value.  
</details>
<details>
  <summary><b>2-Sided</b>: Makes the material 2-sided</summary>

  > Depending on the Material Type an extra 2-sided material is created.  
  > With Update active you can switch between 2-sided and not 2-sided. Materials in material editors will be correctly updated.  
  > When Updating a material to being not 2-sided. The old 2-sided material is still applied to existing objects.  
</details>
<details>
  <summary><b>ID</b>: Set the materials ID Channel</summary>

</details>
<details>
  <summary><b>Create Material</b>: Create a material with selected textures and settings.</summary>

  > If Auto-accept Name (A) is un-checked, a Material Name window will open.  
</details>
<details>
  <summary><b>Auto-accept Name(A)</b>: Create material name derived from selected textures.</summary>

  > If Auto-accept Name is un-checked, a Material Name window will open when creating a material.  
  > Derived name is the common part of all selected texture files.  
</details>
<details>
  <summary><b>Update</b>: Lock and adjust created material with any changes to textures and settings</summary>

  > With Update active you cannot change Material Type.  
  > Loading New or Adding Extra Textures automatically re-assigns textures. With Update active, a message box will pop-up to confirm.  
</details>
<details>
  <summary><b>Clear</b>: Clears only the current created material.</summary>

  > Unlike Reset, textures and settings are kept as is.  
</details>
<h2> </h2>
<img src="images/Slot_001.jpg" align="right"></img>
<h3>Slot</h3><a name="ui_slot"></a>
<details>
  <summary><b>Material Button</b>: Created material can be dragged into objects, editors or material slots.</summary>

  > Shows a renderer preview of the material if Render Material Preview is on.  
</details>
<details>
  <summary><b>Show Material in Viewport</b>: Shows created material in viewport</summary>

  > When active no texture channel can be displayed in viewport.  
  > Only works when a material is created.  
</details>
<details>
  <summary><b>Render Material Preview</b>: Renders a small preview thumbnail</summary>

  > Preview image is taken from the Material Editor.  
</details>
<details>
  <summary><b>Render Preview Background</b>: Renders a checkpattern in the preview background.</summary>

  > Not all renderers support this feature.  
</details>
<details>
  <summary><b>Save Render Preview</b>: Opens a save file dialog, to save current render preview.</summary>

</details>
<details>
  <summary><b>Add Material to Selection</b>: Applies to current material to selected objects.</summary>

  > If Modifiers are checked, these will also be added to the selecte objects.  
</details>
<details>
  <summary><b>Add Material to Material Library</b>: Opens a file loading dialog, to select a material library in whhich to save current material.</summary>

</details>
<details>
  <summary><b>Add Material to Compact Editor</b>: Adds current material to Indicated Sample Slot of the Compact Material Editor </summary>

</details>
<details>
  <summary><b>Add Material to Slate Material Editor</b>: Adds current material to Indicated View of the Slate Material Editor </summary>

</details>
<h2> </h2>
<h3>Modifiers</h3><a name="ui_modifiers"></a>
<details>
  <summary><b>uvMap</b>: If checked and when using Add Material to Selection, add uv_map modifer to selected objects.</summary>

  > uv_map will be using real-world tiling, if this option is selected in Maps settings.  
</details>
<details>
  <summary><b>Displace</b>: If checked and when using Add Material to Selection, add render specific displacement modifer to selected objects.</summary>

</details>
<details>
  <summary><b>Height Value</b>: Height value of the displacement modifier.</summary>

</details>
<details>
  <summary><b>Center Point</b>: Sets the center point of the displacments height value.</summary>

</details>

