# Game Config
The game will not boot without ms3_config.cfg, a renamed XML file.\
\
There are a few different types of game config. These must be specified in the `type` tag (except races). Some templates can be found below:
- AITESTBED
- BENCHMARK
- CINEMATICS
- COMMANDLINE_RACE
- DEMO (Default)
- GUI
  ```xml
  <?xml version="1.0" encoding="UTF-8"?>
  <Config type="GUI" xmlns="http://tempuri.org/boost1.xsd">
    
      <GUIFile name=""/> <!-- Initial GUI filename including the extension e.g. filename.gui -->
      <!-- <DemoMode mode=""/> --> <!-- Demo mode, uncomment if needed (choices are E3, Leipzig or PSN) -->

  </Config>
  ```
- GUI_FOCUSDAYTESTING
- HOME_GAME_LAUNCH
- NPCTESTBED
- PREVIEW
- RACE