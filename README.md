# ESP32_CAM
Snippets from starting up ESP32 CAM. 

Parts needed :

1. ESP32 + Cam  ( I got 2 pieces separately, and I had to hook it up )
2. FTDI connector
Connections are as follows : See pin diagram diagram below on pin structure.

FTDI    ESP32
5v        5v
GND       GND
Tx        UORxD
Rx        U0TxD

![image](https://user-images.githubusercontent.com/14288989/133599732-61434002-5f70-427c-95b9-61a043aa9bf2.png)


Connecting the OV3620 Cam to the board.

https://www.youtube.com/watch?v=5XCb3t8J4Kg

![image](https://user-images.githubusercontent.com/14288989/133598895-ceae517a-40ea-4b57-8def-ae37d618876f.png)


Pin Diagram
![image](https://user-images.githubusercontent.com/14288989/133598973-7c7e27a0-d585-40b1-b855-559185748d6e.png)
