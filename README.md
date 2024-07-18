# RL78_F24_CAN
 RL78_F24_CAN

udpate @ 2024/07/16

1. init UART , P15 , P16 for printf log , 

2. init CAN BUS : P1.0/CTXD0 , P1.1/CRXD0 , test on RL78 F24 EVB

3. refer to RL78/F24 RS-CANFD lite Module Software Integration System Rev.1.00 - Sample Code 

https://www.renesas.com/us/en/document/scd/rl78f24-rs-canfd-lite-module-software-integration-system-sample-code?r=1552481

https://www.renesas.com/us/en/document/apn/rl78f24-rs-canfd-lite-module-software-integration-system?language=en&r=1552481


4. below is CAN bus clock setting in smart config 


![image](https://github.com/released/RL78_F24_CAN/blob/main/smart_config_baud_rate.jpg)


 User’s Manual: Hardware , clocks
![image](https://github.com/released/RL78_F24_CAN/blob/main/User_Manual_clocks.jpg)


 High-Speed On-chip Oscillator
![image](https://github.com/released/RL78_F24_CAN/blob/main/smart_config_clocks.jpg)


 X1 Oscillator + PLL Circuit
![image](https://github.com/released/RL78_F24_CAN/blob/main/smart_config_clocks_X1.jpg)


5. below is baud rate/sampling setting in PCAN 

![image](https://github.com/released/RL78_F24_CAN/blob/main/PCAN_baud_rate.jpg)


6. below is MCU receive CAN bus data from PCAN 

![image](https://github.com/released/RL78_F24_CAN/blob/main/log_PCAN.jpg)


7. below is MCU transmit CAN bus data to PCAN 

press digit 1 , to single transmit one packet 

![image](https://github.com/released/RL78_F24_CAN/blob/main/digit_1.jpg)


press digit 2 , to continuous transmit packet , data increase 1 per packet

![image](https://github.com/released/RL78_F24_CAN/blob/main/digit_2_CAN_Send_TX_Data_Message_Buffer_polling1.jpg)


press digit 3 , to continuous transmit packet , data increase 0x10 per packet

![image](https://github.com/released/RL78_F24_CAN/blob/main/digit_3_CAN_Send_TX_Data_Message_Buffer_polling2.jpg)


