# bwa
Forked https://github.com/jshank/bwalink.git

## SPA Bath

Compiled for raspberry <br>

	1. git clone https://github.com/jshank/bwalink.git
 	2. docker buildx build --platform linux/arm/v7 -t rogerbwa:v3 .
  	3. docker save ...
   	4. sftp to linux and add image
	5. docker load …..	<br>
	6. Modify docker-compose .... see docker-compose in this repo
		a. Mqtt
		b. Ser2net server according to below




1. Connect "RS485" cable - https://github.com/jshank/bwalink?tab=readme-ov-file#connection-cable
2. EWLINK config - https://github.com/jshank/bwalink?tab=readme-ov-file#serial-to-ip-device
3. docker-compose -f docker-compose.yml up -d
4. check that you get messages; `mosquitto_pub -t homie/#`
5. HOME ASSISTANT - MQTT->entities->BWA


## Notes
mosquitto_pub -t "homie/bwa/spa/pump2/set" -m "true"

## Todo:
Add my docker compose file<br>
![image](https://github.com/user-attachments/assets/0eba698a-2dbf-4516-b92e-f40b6d9b3996)
