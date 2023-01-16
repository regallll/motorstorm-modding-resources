# Game Config
The game will not boot without ms2_config.cfg, a renamed XML file.\
\
There are a few different types of game config. These must be specified in the `type` tag (except races). Some templates can be found below:
- BACK2BACK_TICKETS
- BENCHMARK
  ```xml
  <?xml version="1.0" encoding="UTF-8"?>
  <Config type="BENCHMARK" xmlns="http://tempuri.org/boost1.xsd">

      <World name=""/> <!-- Track name -->
      <Environment name=""/> <!-- Sky name -->
      <CameraPath file="" path="" animDurationSeconds=""/>
      <!-- <CameraPath file="" path="" animDurationSeconds=""/> -->
      <!-- <CameraPath file="" path="" animDurationSeconds=""/> -->
      <!-- <CameraPath file="" path="" animDurationSeconds=""/> -->
      <!-- Uncomment the above according to how many viewports you want (choice of 1, 2 or 4) -->
      <!-- file is written like path/to/camera/path/file.cam and can usually be found in data/benchmarkcameraanims/ -->
      <!-- path is the camera path name, leaving it blank selects the first path in the path file -->
      <!-- animDurationSeconds is self-explanatory and can be a decimal -->
      <Review enabled=""/> <!-- Performance review at the end, boolean (0 or 1) -->

  </Config>
  ```
- DEVGHOSTCOPIER
- GUI (Default)
  ```xml
  <?xml version="1.0" encoding="UTF-8"?>
  <Config type="GUI" xmlns="http://tempuri.org/boost1.xsd">
    
      <GUIFile name=""/> <!-- Initial GUI filename including the extension e.g. filename.gui -->

  </Config>
  ```
- MPSTRESS
- SOAK_TEST_ONLINE_HOST
- SOAK_TEST_RANDOM
- SOAK_TEST_REPEAT
- SOAK_TEST_SEQUENTIAL
- SOAK_TEST_SPLIT_SCREEN

The Includes section of the game config doesn't do anything.
