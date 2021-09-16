# ESP32_CAM
Snippets from starting up ESP32 CAM. 

Parts needed :

1. ESP32 + Cam  ( I got 2 pieces separately, and I had to hook it up )
2. FTDI connector
3. Magnifying glass 

Connections are as follows : 

FTDI    ESP32

 5v        5v
 
 GND       GND
 
 Tx        UORxD
 
 Rx        U0TxD

![image](https://user-images.githubusercontent.com/14288989/133599732-61434002-5f70-427c-95b9-61a043aa9bf2.png)


Connecting the OV2640 Cam to the board.

![image](https://user-images.githubusercontent.com/14288989/133601044-65aef107-2eba-4168-bdfd-402c56ad121c.png)

2:42 - tells how to lift the connector.

![image](https://user-images.githubusercontent.com/14288989/133601171-6410c6a1-3197-47d4-89e6-f5a49b4be11b.png)

https://www.youtube.com/watch?v=5XCb3t8J4Kg

![image](https://user-images.githubusercontent.com/14288989/133598895-ceae517a-40ea-4b57-8def-ae37d618876f.png)



![image](https://user-images.githubusercontent.com/14288989/133598973-7c7e27a0-d585-40b1-b855-559185748d6e.png)

![image](https://user-images.githubusercontent.com/14288989/133601776-66c20307-e6f1-4baa-8e52-c331e9c62243.png)
![image](https://user-images.githubusercontent.com/14288989/133601882-2266dc5e-b101-47a1-ba22-8f66cb4d2b87.png)


![image](https://user-images.githubusercontent.com/14288989/133601726-52ca9f57-e4c5-4370-8757-00a6dd7d3dc6.png)


Flashing mode / programming the board 

Connect IO0 and GND during flashing. Disconnect and press RESET to start running the sketch

![image](https://user-images.githubusercontent.com/14288989/133602185-9d12e5b9-26a9-4043-8719-178b87500c1a.png)

