# aframe-datguivr
A-Frame component for [datGUIVR](https://github.com/dataarts/dat.guiVR)

## Example

    <a-datgui name="settings" position="0 2 -1">
      <a-gui-slider id="scaleControl" name="scale" step="0.01" min="0.01" max="4"></a-gui-slider>
      <a-gui-dropdown name="options">
        <a-gui-option value="0">Item 0</a-gui-option>
        <a-gui-option value="1">Item 1</a-gui-option>
      </a-gui-dropdown>
      <a-gui-checkbox name="on or off" default="true"></a-gui-checkbox>
      <a-gui-button name="click me"></a-gui-button>
    </a-datgui>   

Currently supports "stateless" controllers only, meaning you can't attach controllers directly to JS objects, however you can listen to controller changes and update anything accordingly.

Each controller element will emit an "onChanged" event supplying the new value.    
