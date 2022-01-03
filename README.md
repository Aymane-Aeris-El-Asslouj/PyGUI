# PyGUI
Pygame Library for a layer/object-based Python GUI

### Main functionality
Supports creation of a window (gui.GUI) that can store layers (layer.Layer) which itself stores objects (layer.LayerObject) like buttons or drag-n-drop objects

### Secondary functionalities
+ The interaction loop (input_manager.activate(GUI)) maintains a constant refresh rate (constant fps) with layers drawn upon request at each frame
+ The interaction loop passes window events to layers which themselves pass them to layer-objects to respond to inputs
+ The GUI stores .json settings that can be loaded and saved. Certain Layer objects automatically create settings to save their state
+ Pre-built layer-objects (Label, Button, ToggleButton, InputButton, DragAndDrop, SettingToggleButton, SettingInputButton)
