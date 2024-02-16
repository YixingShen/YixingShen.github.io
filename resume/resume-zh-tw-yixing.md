沈玴興 (Yixing Shen)
============

https://yixingshen.github.io 

Contact
---------

Email: kkman3651878@hotmail.com    
LINE ID: yixingshen    
Skype: kkman3651878    

About
---------

- System Engineer
- Board Bring Up
- Firmware and Software Development

Education
---------

- 2008 - 2010, MSc, Power Systems Engineering, 中原大學電機工程研究所    
- 2004 - 2008, BSc, Electrical Engineering, 中原大學電機工程學系     

Experience
---------

2022/04 - Present 奇景光電 (Himax Technologies, Inc), ASIC設計處, 系統應用工程師    

> Port TF-M, FatFs file system, RTX5 RTOS    
> Integrate SDK to CMSIS packs

- IC Utils 
  - USB Bridge Based on DAPLink
    - CMSIS DAP Debugger over SWD
    - Dual Virtual COM Port
    - Multipath Bridge to SPIM/SPIS/I2CM/UART
  - pyOCD FlashAlgo and FLM
    - Erase, Dump, Auto Produce

2013/06 - 2022/04 義晶科技 (Avisonic Technology Corporation), 系統整合及設計處, 系統應用工程師    

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
  - RAW (CFA)/RGB/YCBCR Image Converter    
    - RAW Bayer (CFA)
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
    修改GPIF設定, 接收YUV422 16bit/8bit影像資料, 加入HID和UVC Extension Unit (XU)控制I2C/SPI, 電腦透過USB存取I2C/SPI裝置和擷取影像輸入  
  - MDIN340/325A/270 (Macro Image Tech, Video Display Processor, MDK-ARM):     
    從LM3S1607移植到Renesas MCU (RL78/G13), 加入OSD顯示, 修改韌體流程    
  - EJ511 (eEver Tech, USB Controller, Keil C51):    
    修改韌體支援MJPG/YUY2各種解析度組合,修改I2C控制外部裝置流程和客製化設定
  - PR2000 (Pixelplus, Analog HD Video Decoder, MDK-ARM):    
    修改STM32F103韌體流程加入AVS7610控制, 加入I2C Slave功能, 電腦可透過UART/I2C介面調整AVS7610 
  - KL520/KL720  (Kneron, AI Chip, ARM Cortex-M4, CMSIS RTOS, MDK-ARM):    
    修改KL520韌體Host Mode支援MIPI DPI, 修改Flash讀寫API, 加入一些客製化功能, 修改KL720韌體HICO Mode支援MIPI DPI和Host Mode, 配合Kneron Plus軟體加入一些測試功能    

- Projects    
  
  - 4CH HDMI Video Wall
  - HDMI 1.4 Grabber USB
  - 3G-SDI Grabber USB
  - CVBS Grabber USB
  - HD Analog CCTV Grabber USB
  - [HDMI Interface Camera for Tesla Model S/X](https://www.youtube.com/watch?v=toqY03yc2Kc)
  - [AI Camera for ADAS](https://www.kneron.com/tw/news/blog/118/)
  - [AI Camera for Electric Bus BSD](https://www.bnext.com.tw/article/62534/kneron-kl720)

2011/12 - 2013/06 華晶科技 (Altek Corporation), 軟體驅動部, 韌體工程師    

> Developed and maintained lens controller firmware and calibration for ARCtangent-A5 and MQX RTOS platform.     
>  Lens device driver (Zoom/Focus/Iris/Shutter)    

- Nikon Digital Camera COOLPIX S02
- Nikon Digital Camera COOLPIX L28    

2008/09 - 2010/07 中原大學電機工程研究所    

- 應用人工智慧和訊號處理於電力系統    
  - 以機率神經網路,時頻分析及最佳化演算法建立一套特徵選取機制於電力品質干擾自動辨識[1]     
  - 運用Matlab/Simulink做為演算法開發及永磁式同步風力機最大功率追蹤控制[2]    
- 碩士論文    
  [1] 沈玴興, ["電力品質問題之特徵選取與分類," 中原大學電機工程研究所, 2010.](https://hdl.handle.net/11296/qw737z)
- 期刊論文    
  [1] C.-Y. Lee and **Y.-X. Shen**, [“Optimal Feature Selection for Power-Quality Disturbances Classification,” IEEE Transactions on Power Delivery, Vol. 26, No. 4, pp. 2342-2351, Oct. 2011.](https://doi.org/10.1109/TPWRD.2011.2149547) (SCI; ISSN:0885-8977)    
  [2] C.-Y. Lee, P.-H. Chen and **Y.-X. Shen**, [“Maximum Power Point Tracking (MPPT) System of Small Wind Power Generator Using RBFNN Approach,” Expert Systems with Applications, Vol. 38, No. 10, pp. 12058-12065, Sept. 2011.](https://doi.org/10.1016/j.eswa.2011.02.054) (SCI; ISSN:0957-4174)    

Knowledge
---------

- Embedded System, RTOS 
- I2C, SPI, UART, I2S
- USB Video/Audio/HID Class
- CMOS Sensor DVP, HD/SDTV Parallel Interface, CVBS, HDMI, ITU-R BT656/BT601/BT1120, EIA/CEA-861  
- Digital Camera Lens (Motor) Driver    

Skills and Tool
---------

- C, C# .NET, Python, QT, Matlab, STM32Cube, GNU Make, RTL Verilog    
- Keil MDK-ARM/C51, Microsoft Visual Studio, Renesas CS+, Intel (Altera) Quartus Prime    
- Logic Analyzer, Oscilloscope, Vectorscope    

ICs
---------

- AVS7610, AVS7150 (義晶, Fisheye Correction)
- CYUSB3014, EJ511 (USB Controller)
- MDIN340/325A/270 (Video Display Processor)
- IT6801/6604/66121 (HDMI), TC358743XBG (HDMI Bridge to MIPI CS-2)  
- GV7601/7600 (SDI), TVP5150 (CVBS Video Decoder), PR2000 (Analog HD Video Decoder)
- DS90UB913/914 (LVDS), WM8960 (Audio Codec)
- R5F1007E, R5F100GG, STM32F103, STM32F030
- KL520 (AI Chip), KL720 (AI Chip)
