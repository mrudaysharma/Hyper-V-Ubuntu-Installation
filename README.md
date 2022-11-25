# Hyper-V-Ubuntu-Installation
## Make Window Full Screen 
  - sudo gedit /etc/default/grub
    GRUB_CMDLINE_LINUX_DEFAULT="quiet splash" to GRUB_CMDLINE_LINUX_DEFAULT="quiet splash video=hyperv_fb:1920X1080"
## Activate Gedit 
  Error :  (gedit:1952): Gtk-WARNING **: 14:36:43.829: cannot open display: :10.0
  - sudo nano /etc/sudoers 
  Add this line -> Defaults env_keep="DISPLAY" 
  (Save and Exit)
 - xhost +si:localuser:root
    output -> localuser:root being added to access control list 
 now try
 - sudo gedit (It works)
