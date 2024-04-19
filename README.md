Documentation
===
# MaterialTextureLoader
Documentation for Material Texture Loader for 3ds Max

Table of contents
---
---
- [Description](#description)
  - [Support](#support)
  - [Links](#links)
- [UI](#ui)
  - [Top Menu](#uitopmenu)
  - [Texture Channels](#uichannels)
  - [Map Settings](#uimaps)


## Description<a name="description"></a>
Material Texture Loader is a plugin for 3ds Max that creates advanced material setups from textures sets.
### Support <a name="support"></a>
- 3ds Max 2016-2024
- Vray(v3-6)
- Corona(v5-10)
- Redshift
- Arnold
- FStorm
- Octane
- Physical, PBR and Standard
### Links <a name="links"></a>
- [Youtube](https://youtu.be/HqMXw3Hht64?si=ejwyelh94iZaYcg1)
- [Gumroad](https://dmz.gumroad.com/l/ScriptBox)
- [Scriptspot](https://www.scriptspot.com/3ds-max/scripts/script-box)

<br></br>
## UI <a name="ui"></a>
### Top Menu <a name="uitopmenu"></a>
<img align="right" alt="Top Menu" src="images/TopMenu_001.jpg" width="400"></img>
<img align="right" alt="Top Menu" src="images/TopMenu_001.jpg" width="400"></img>

- **Load New Textures:** Opens a browser menu where you can multi-select image files to load into the Texture Channels dropdown list. Active Naming Filters will be used to automatically assign textures to Channels. 
- **Add extra Textures:** Opens a browser menu where you add image files to the Texture Channels dropdown list.
- **Use All Channels:** When checked, this will make all Texture Channel available for use. For materials that don't use a specific channel, the created map will be accedible by pressing Add Material to Compact / Add Material to Slate.   
- **Reset:** Reset's the whole UI. Clears all image files from Channel, Material and select 'Default' Preset.
- **Naming Filters:** Opens Texture Naming Filters menu, where you can activate existing Naming Filters. Up to 10 nameFilter files in 'nameFilters' directory will be listed. 
- **MTL Installer:** Opens the Installer menu for the Material Texture Loader. Contains Uninstall option and a list of all plugin directories.
- **Preset:** Dropdown list will all saved Presets. Switching Presets will change the settings directy.
- **Save Preset:** Opens a Preset Name menu, where you can save the Current Settings under the given name. If Preset name already is in use, will ask to overwrite existing Preset.
- **Dockable:** Switch between dockable and window dialog mode.
<br></br>



### Texture Channels <a name="uichannels"></a>
<img src="images/Channels_001.jpg" align="right" width="600" alt="Texture Channels"></img>
<img src="images/transparant.png" align="right" width="600" alt="Texture Channels"></img> 
<dl>
  <dt>Enabled/Disable Channel</dt>
  <dd>Disables a channel from creating maps, even when a texture is selected in the Texture Dropdown.</dd>
  <dt>Channel Texture</dt>
  <dd>Dropdown list where you can select a texture for the material channel.</dd>
  <dt>Channel Strenght</dt>
  <dd>Set the strength of the texures influence in the material channel.</dd>
  <dt>Channel Settings</dt>
  <dd>Button that displays the channel name. Click on the button to open channel specific settings.</dd>
  <dt>Show Channel</dt>
  <dd>When a material is created you can select which texture channel is displayed in the viewport.</dd>    
</dl>
<br></br>
<br></br>
<br></br>

### Maps Settings<a name="uimaps"></a>
<img align="right" alt="Texture Channels" src="https://github.com/DMZScripts/MaterialTextureLoader/blob/fbdf2e050fa9e27c72de5d739255001a87a4da4e/images/Maps_001.jpg" width="200"></img>
- **Map Type**: If the selected material class support it, choose between default 3ds Max Bitmaps or render specific texture maps. 
- **Blur**: Blur value being applied to each texture map.
- **Mapping Channel**: Sets the mapping channel for each texture map. 
- **Mapping Type**: Sets the mapping type for each texture map
  - Tiling: 
  - Real-world:
  - Tri-planar:
  - Spherical:
<br></br>
<br></br>
<br></br>


### Material Settings <a name="material"></a>
<img alt="Material" src="https://github.com/DMZScripts/MaterialTextureLoader/blob/fbdf2e050fa9e27c72de5d739255001a87a4da4e/images/Material_001.jpg" width="400"></img>

### Slot <a name="slot"></a>
<img alt="Texture Channels" src="https://github.com/DMZScripts/MaterialTextureLoader/blob/fbdf2e050fa9e27c72de5d739255001a87a4da4e/images/Slot_001.jpg" width="400"></img>
