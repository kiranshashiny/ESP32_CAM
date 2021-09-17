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

To put in Flash mode: ( Careful - DO NOT CONNECT THE VCC AND THE GND AS IT WILL COME UP AN ERROR ON THE MAC USB PORT )

Connect IO0 and GND - on the silk screen (next to each other ) 

Mine is NOT a AI-Thinker - as listed other documents - it's printed on the chip.

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


Programming Sketch

![image](https://user-images.githubusercontent.com/14288989/133602926-d5138ceb-1a7c-4c8b-9b3d-e07ea796dbdb.png)

Code to be set to Line 17 ( Don't do WRover - as you will get a Unsupported Camera error )


![image](https://user-images.githubusercontent.com/14288989/133603149-1c4ea3bc-9368-4bcf-a05c-76f0bea91300.png)

 To be added the libraries etc etc.
 
 
This is how the connections should show up once the module is connected.

![image](https://user-images.githubusercontent.com/14288989/133604506-83382af6-aa6e-47eb-9073-24f94e567f5f.png)

On a successful Upload

![image](https://user-images.githubusercontent.com/14288989/133604890-a54f889d-0ce9-4ee8-afdf-5d30db01f36f.png)
![image](https://user-images.githubusercontent.com/14288989/133605047-be073ac9-8f0f-4a59-9a89-d889a2106eb2.png)

At this point - Open the serial monitor, remove the Flash GND pin, press RST button.

Error during Upload

To resolve :
Change the ssid from JioFiber-702_5g to JioFiber-702 ( the 2.4Ghz ) in the sketch
Also does changing the laptop's JioFiber-702_5G to 2.4Ghz help ? ( I did and I was able to connect )

![image](https://user-images.githubusercontent.com/14288989/133605205-96f43a14-d824-4ad0-bf8f-42cf24baef36.png)



Error during Upload
If you get a continuous 'trying to connect' message on the Serial Monitor - then change from 5G to 2.4G connection.

On successful connection :

![image](https://user-images.githubusercontent.com/14288989/133606462-bd39cad5-7fab-455f-b01e-79ed44366e3e.png)

On successful connection:

![image](https://user-images.githubusercontent.com/14288989/133645434-20a32ef8-3569-4760-b350-24242ba9437a.png)


Diagram to connect the PIR sensor to ESP32CAM

![image](https://user-images.githubusercontent.com/14288989/133751199-4e153c66-ac79-4a4e-a370-deb6287457eb.png)
