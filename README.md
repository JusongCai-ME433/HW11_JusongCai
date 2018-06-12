# HW11_JusongCai

In HW11, the gyroscope IMU was used to control the mouse cursor on my Mac via USB and HID (human interface device). Codes are included in "firmware/scr" folder: "ST7735.c/h" is LCD communication with PIC32 via SPI; "imu.c/h" is IMU communication with PIC32 via I2C; "i2c_master_noint.c/h" is the setup of I2C communication; "app.c/h" is USB communication with my Mac, which is the core code that sends IMU data (x and y acceleration control signal)to Mac to control the mouse cursor; "main.c" is the main function that controls app; "mouse.c/h" is the mouse control functions.

Result is shown in mp4 file named "demo video for HW11": while tilting the board up-and-down/left-and-right, the mouse cursor corresponds to move in the same direction. 