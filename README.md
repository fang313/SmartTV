### SmartTV
## Tizen commands to deploy test app on device
  
  // Check connected devices and run sdb service  
  
  # C:\tizen-studio\tools\sdb devices
  
  // Setup connection to device  
  
  # C:\tizen-studio\tools\sdb connect 192.168.__.__  (device ip, look on device network settings)

  // Deploy and install app on SmartTV  
  // Enter the folder with app file  
  // -t (target ID) for example UE32T5300AUXRU
  
  # C:\tizen-studio\tools\ide\bin\tizen install -n c:\tizen-studio\khl_name.wgt -t UE32T5300AUXRU  
  
  // Delete app from SmartTV  
  // For a fisrt we nedd to know app_id from app_list on device (from device manager)  
  // Also app ID  we can see in progress of install app  
  // -p add_id  
  
  # C:\tizen-studio\tools\ide\bin\tizen uninstall -t UE32T5300AUXRU -p 31E0oQgxyL.KHL
