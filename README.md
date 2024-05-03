<h1 align ="center">Material Texture Loader</h1>
<div align="center">Advanced material creation plugin for 3ds max</div>
<div align="center"><a href="https://youtu.be/HqMXw3Hht64?si=ejwyelh94iZaYcg1">Youtube</a> - <a href="https://dmz.gumroad.com/l/ScriptBox">Gumroad</a> - <a href="https://www.scriptspot.com/3ds-max/scripts/script-box">Scriptspot</a></div>

***
### Table of contents
- [Support](#support)
- [Instalation](#instalation)
- [User Interface](#ui)
  - [Top Menu - Files](#ui_topmenu_files)
  - [Top Menu - Presets](#ui_topmenu_presets)
  - [Channels](#ui_channels)
  - [Channels - Channel Settings](#ui_channels_settings)
  - [Map Settings](#uimaps)

### Description <a name="description"></a>
Documentation for UI an maxScript API.  
Material Texture Loader is a plugin for 3ds Max that creates advanced material setups from textures sets.
***


# Support <a name="support"></a>
- 3ds Max 2016-2024
- Vray(v3-6)
- Corona(v5-10)
- Redshift
- Arnold
- FStorm
- Octane
- Physical, PBR and Standard

***
<h1>User Interface</h1><a name="ui"></a>
<h3>Top Menu</h3> <a name="ui_topmenu_files"></a>
<img src="images/TopMenu_001.jpg" alt="Top Menu" align="right" width="400"></img>
<details>
  <summary><b>Load New Textures</b>: Open texture file browser to select new files.</summary>
  
  > You can multi-select any 3ds max supported image files.  
  > Selected files will be place in the Texture Channels dropdown list.  
  > Previously loaded files will be removed.
  > Active Naming Filters will be used to automatically assign textures to Channels.
</details>

<details>
  <summary><b>Add Extra Textrues</b>:  Open texture file browser, to select additional files. </summary>

  > You can multi-select any 3ds max supported image files.  
  > Selected files will be added to the Texture Channels dropdown list.  
  > Active Naming Filters will be used to automatically re-assign textures to Channels.
</details>

<details>
  <summary><b>Use All Channels</b>: Activate all texture Channels.</summary>

  > When materials don't use every texture channel, this will make all Texture Channel available.  
  > Maps that are created in this way are accessable after pressing _Add Material to Compact_ / _Add Material to Slate_.  
  > Maps will be placed adjacent to the material that is created.  
</details>

<details>
  <summary><b>Reset</b>: Reset entire UI back to Deafult.</summary>

  > Selects Default as Preset  
  > Clears all image files from Texture Channels  
  > Clears Material Slot
</details>

<details>
  <summary><b>Naming Filters</b>: Select active Naming Filters.</summary>

  > Naming FIlters are used for automatic Texture Channel selection.  
  > You can activate any combination of listed Naming Filters.  
  > Up to 10 nameFilter files in _nameFilters_ directory will be listed.  
</details>

<details>
  <summary><b>MTL Installer</b>: Opens Installer menu.</summary>

  > Contains Uninstall option and a list of all plugin installation directories.
</details>

<details>
  <summary><b>Preset</b>: Dropdown list of all saved settings.</summary>  
  
  > Switching Presets will change all settings directy.  
  > When Update is active, you can still switch Presets. Material type will be locked to current Material.
</details>

<details>
  <summary><b>Save Preset</b>: Save current settings.</summary>

  > Opens a Preset Name menu, where you can save the Current Settings under the given name.
  > If Preset name already exists, menu will ask if you want to overwrite existing Preset.
</details>

<details>
  <summary><b>Dockable</b>:Switch between dockable and window dialog mode.</summary>
</details>


<h2> </h2>
<h3>Channels</h3><a name="ui_channels"></a>
<img src="images/Channels_001.jpg" alt="Texture Channels" align="right" width="400"></img>
<details>
  <summary><b>Enable/Disable Channel</b>: Disable or enabled a channel from creating maps. </summary>

  > Disabeling channels will disable all other Channel controls.  
  > When disabled no maps are created, even when a texture file is selected in the dropdown list.  
  > Channel will be disabled automatically when a material type does not support the channel.  
  > You can force every channel to be active by checking _Use All Channels_ (see: [Top Menu - Files](#uitopmenu)).  
</details>

<details>
  <summary><b>Channel Texture</b>: Select a texture file for the channel from the dropdownlist.</summary>

  > For selected tecxture files a texture map will be created and connected to the material.
  > Texture files will be available when loaded in with _Load New Textures_ or _Add Extra Textrues_.  
  > Select empty item to deselect any texture file. No map will be created for this channel.  
</details>

<details>
  <summary><b>Channel Strength</b>: Set the strength or influence of the texture image.</summary>

  > Control will be disabled when material type does not have support for Texture Strength.  
</details>

<details>
  <summary><b>Channel Settings</b>: Button that displays channel name and opens channel specific settings.</summary>

  > for Channel Settings see:[Channels - Settings](#ui_channels_settings).  
</details>

<details>
  <summary><b>Show Channel</b>: Show channels texture map in viewport.</summary>

  > Only 1 channel can be displayed. 
  > Only works when a material is created.
</details>
<br></br>

<h2> </h2>
<h3>Channels - Settings</h3><a name="ui_channels_settings"></a>
<details>
  <summary></summary>
</details>


<h2> </h2>
<img src="images/Maps_001.jpg" alt="Texture Channels" align="right"></img>
<h3>Map Settings</h3><a name="ui_maps"></a>
Not all renderers support every feature in the map settings. UI controls will be disabled if these options are not available.

<details>
  <summary><b>Map Type</b>: Choose between standard and render specific texture map</summary>

  > Render specific texture maps will be selected based of the material type selected.  
  > Not all renderers support standard Bitmaps.  
</details>
<details>
  <summary><b>Blur</b>: Blur value applied to each texture map</summary>

  > - Blur is applied to all channels equally. There is no option for channel specifc blur values.  
</details>
<details>
  <summary><b>Mapping Channel</b> Set mapping channel for all texture maps.</summary>
</details>
<details>
  <summary><b>Mapping Type</b>: Set the mapping type for each texture map.</summary>

  > Tile mapping:  
  > Real-world mapping:
  > Tri-planar mapping:
  > Spherical mapping:  
</details>
<details>
  <summary><b>Size</b>: set U and V mapping size.</summary>

  >  
</details>
<details>
  <summary><b>Non-Uniform Size</b>: Enable.</summary>

  >  
</details>


<h2> </h2>
<img src="images/Material_001.jpg" alt="Material" align="right"></img>
<h3>Material Settings</h3><a name="material"></a>
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


<h2> </h2>
<img src="images/Slot_001.jpg" alt="Texture Channels" align="right"></img>
<h3>Material Slot</h3><a name="material"></a>
