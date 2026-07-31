沈玴興 (Yixing Shen)
============

Contact
---------

Email: kkman3651878@hotmail.com    
LINE ID: yixingshen    
WeChat: yixingshen_tw    
Teams: kkman3651878    

About
---------

- System Engineer
- Firmware and Software Development

Education
---------

- 2008 - 2010, MSc, Power Systems Engineering, Chung Yuan Christian University    
- 2004 - 2008, BSc, Electrical Engineering,  Chung Yuan Christian University     

Experience
---------

2022/04 - Present 奇景光電 (Himax Technologies, Inc), ASIC Design Division, System Engineer        

> Port TF-M, FatFs, RTX5, TinyUSB, UF2, Zephyr RTOS     
> Integrate SDK to CMSIS packs

- IC Utils 
  - USB Bridge Based on DAPLink
    - CMSIS DAP Debugger over SWD
    - Dual Virtual COM Port
    - Multipath Bridge to SPIM/SPIS/I2CM/UART
  - pyOCD FlashAlgo and FLM
    - Erase, Dump, Auto Produce
  - USB DFU
    - Download, Upload, Detach
  - USB Camera
    - DirectShow Capture uncompressed and mjpeg streams or still images
    - UVC Extension Unit commands 

2013/06 - 2022/04 義晶科技 (Avisonic Technology Corporation), System Integration & Design Division, System Engineer        

> Design and develop IC utils using C# .Net Framework and WIN32 API DLL for EVB.    
> Design and develop IC built-in MCU (DP8051) peripheral drivers, bootloader and application codebase.    
> Bring up demo board.   
> FPGA and IC function verification   

- IC Utils  
  
  - USB HID/CDC/UVC XU to I2C/SPI   
    - CYUSB3014 HID/UVC XU I2C/SPI
    - FT232R Bit-Bang I2C/SPI, FT232H MPSSE I2C/SPI
  - USB Camera Viewer
    - DirectShow Capture raw YUY2 Image from WebCam
  - Flash Programmer
    - Erase, Dump, Auto Produce, Block Protect
  - Script and Code Generator    
    - VIP, ISP, NR, SCLDN, Frame Buffer, SCLUP, DISP, TVEN
  - RAW/RGB/YCBCR Image Converter    
    - RAW Bayer
    - YCBCR444/422/420 Packed
    - YCBCR444/422/420 Planar
    - YCBCR422/420 Semi Planar
    - RGB565,RGB555,RGB32,RGB24
  - Edit OSD Font and Convert Bitmap to Binary for Avisonic Chip
  - Convert Dump Waveform to VCD Format for GTKWave Viewer 
  - RLE/RLD Converter    
  - ISP Tuning UI for AVS761x    

- Codebase
  
  - On-chip BootROM
  - Bootloader
    - Boot Application from Flash
    - Program Code Memory over UART/I2C
    - Update Firmware over UART/I2C 
  - Hardware Abstraction Layer
    - I2C, SPI, UART, PWM, Timer, CAP, IRQ
    - NOR Flash
    - CAN (MCP2515/10, SJA1000)
    - MPU I8080/M6800 LCD Display
  - Middleware
    - I2C/UART Bridge to Register/Ext Flash/Ext I2C
    - Graphic OSD, ePTZ, Xmodem, PcoleD/P, J1939

- Demo Board   
  
  - LVDS SerDes
  - HDMI Transmitter/Receiver 
  - HDMI Up/Down to LVDS/MIPI CSI-2
  - Fisheye Camera Module   

- Miscellaneous
  
  - CYUSB3014 (Cypress Semi, USB Controller, ThreadX, GNU ARM):    
    Modified GPIF II configurations to receive 16/8-bit YUV422 video data, and implemented HID and UVC Extension Unit (XU) controls over I2C/SPI interfaces to enable host access and video capture via USB.  
  - MDIN340/325A/270 (Macro Image Tech, Video Display Processor, MDK-ARM):    
    Ported display processing firmware from Stellaris LM3S1607 to Renesas MCU (RL78/G13), integrated customized OSD layers, and optimized firmware execution flow.    
  - EJ511 (eEver Tech, USB Controller, Keil C51):    
    Modified firmware to support various resolution combinations for MJPEG/YUY2; modified I2C control procedures for external devices and configured custom settings.
  - PR2000 (Pixelplus, Analog HD Video Decoder, MDK-ARM):    
    Modified STM32F103 firmware logic to integrate AVS7610 controller routines, implemented I2C Slave functionality, and enabled PC host parameter adjustment for the AVS7610 via UART/I2C interfaces. 
  - KL520/KL720 (Kneron, AI Chip, ARM Cortex-M4, CMSIS RTOS, MDK-ARM):    
    Modified KL520 firmware Host Mode to support MIPI DPI and revised Flash R/W APIs with custom features; modified KL720 firmware HICO Mode to support MIPI DPI and Host Mode, deploying hardware test validation with Kneron Plus software.    

- Projects    
  
  - 4CH HDMI Video Wall
  - HDMI 1.4 Grabber USB
  - 3G-SDI Grabber USB
  - CVBS Grabber USB
  - HD Analog CCTV Grabber USB
  - [HDMI Interface Camera for Tesla Model S/X](https://www.youtube.com/watch?v=toqY03yc2Kc)
  - [AI Camera for ADAS](https://www.kneron.com/tw/news/blog/118/)
  - [AI Camera for Electric Bus BSD](https://www.bnext.com.tw/article/62534/kneron-kl720)

2011/12 - 2013/06 華晶科技 (Altek Corporation), Software Driver Department, Firmware Engineer  

> Developed and maintained lens controller firmware and calibration for ARCtangent-A5 and MQX RTOS platform.     
> Lens device driver (Zoom/Focus/Iris/Shutter)    

- Nikon Digital Camera COOLPIX S02
- Nikon Digital Camera COOLPIX L28    

2008/09 - 2010/07 中原大學 (Chung Yuan Christian University)   

- Application of Artificial Intelligence and Signal Processing in Power Systems   
  - Established an automated feature selection and recognition framework for power quality disturbances utilizing Probabilistic Neural Networks (PNN), time-frequency analysis, and optimization algorithms[1]     
  - Utilized Matlab/Simulink for algorithm development and implemented Maximum Power Point Tracking (MPPT) control for permanent magnet synchronous wind turbines[2]    
- Master's Thesis    
  ["電力品質問題之特徵選取與分類," 中原大學電機工程研究所, 2010.](https://doi.org/10.6840/cycu201000431)
- [Journal Publications](https://scholar.google.com/citations?user=0Qv5ftMAAAAJ&hl=zh-TW&oi=ao)       
  [1] C.-Y. Lee and **Y.-X. Shen**, [“Optimal Feature Selection for Power-Quality Disturbances Classification,” IEEE Transactions on Power Delivery, Vol. 26, No. 4, pp. 2342-2351, Oct. 2011.](https://doi.org/10.1109/TPWRD.2011.2149547) (SCI; ISSN:0885-8977)    
  [2] C.-Y. Lee, P.-H. Chen and **Y.-X. Shen**, [“Maximum Power Point Tracking (MPPT) System of Small Wind Power Generator Using RBFNN Approach,” Expert Systems with Applications, Vol. 38, No. 10, pp. 12058-12065, Sept. 2011.](https://doi.org/10.1016/j.eswa.2011.02.054) (SCI; ISSN:0957-4174)    

Knowledge
---------

- Embedded System, RTOS 
- I2C, SPI, UART, I2S, USB
- Sensor DVP, CVBS, HDMI, BT656/BT601/BT1120, CEA-861  
- Lens Motor Driver    

Skills and Tool
---------

- C, C# .NET, Python, QT, Matlab, STM32Cube, GNU Make, RTL Verilog    
- Keil MDK-ARM/C51, Visual Studio, Renesas CS+, Quartus Prime    
- Logic Analyzer, Oscilloscope, Vectorscope   
