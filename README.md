<h1 align ="center">Material Texture Loader</h1>
<div align="center">Advanced material creation plugin for 3ds max</div>
<div align="center"><a href="https://youtu.be/HqMXw3Hht64?si=ejwyelh94iZaYcg1">Youtube</a> - <a href="https://dmz.gumroad.com/l/ScriptBox">Gumroad</a> - <a href="https://www.scriptspot.com/3ds-max/scripts/script-box">Scriptspot</a></div>

***
### Table of contents
- [Support](#support)
- [Instalation](#instalation)
- [User Interface](#ui)
  - [Top Menu](#uitopmenu)
  - [Texture Channels](#uichannels)
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
# User Interface <a name="ui"></a>
### Top Menu - Files <a name="uitopmenu"></a>
<img align="left" alt="Top Menu" src="images/TopMenu_1_001.jpg"></img><br clear="left"/>
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
</details><h2> </h2>


### Top Menu - Presets <a name="uitopmenu"></a>
<img align="left" alt="Top Menu" src="images/TopMenu_2_001.jpg"></img><br clear="left"/>
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
</details><h2> </h2>

### Texture Channels <a name="uichannels"></a>
<table>
  <tr>
    <td width="60%">
      <dl>
        <b><em>Enabled/Disable Channel</em></b>
        <dd>Disables a channel from creating maps, even when a texture is selected in the Texture Dropdown.</dd>
        <b><em>Channel Texture</em></b>
        <dd>Dropdown list where you can select a texture for the material channel.</dd>
        <b><em>Channel Strenght</em></b>
        <dd>Set the strength of the texures influence in the material channel.</dd>
        <b><em>Channel Settings</em></b>
        <dd>Button that displays the channel name. Click on the button to open channel specific settings.</dd>
        <b><em>Show Channel</em></b>
        <dd>When a material is created you can select which texture channel is displayed in the viewport.</dd>    
      </dl>
    </td>
    <td width="40%" valign="top">
      <img src="images/Channels_001.jpg" align="right" width="600" alt="Texture Channels"></img>
    </td>
  </tr>
</table>

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

### Settings - Map<a name="uimaps"></a>
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
