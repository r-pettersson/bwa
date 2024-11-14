# bwa
SPA Bath

Compiled for raspberry <br>

	1. git clone https://github.com/jshank/bwalink.git<br>
 	2. docker buildx build --platform linux/arm/v7 -t rogerbwa:v3 .<br>
  	3. Docker save<br>
   	4. sftp till linux och lägg dit imagen<br>
	5. Docker load …..	<br>
	6. Modify docker-compose ....<br>
		a. Mqtt<br>
		b. Ser2net servern<br>




1. Connect "RS485" cable
2. EWLINK config - https://github.com/jshank/bwalink?tab=readme-ov-file#serial-to-ip-device
3. docker-compose -f docker-compose.yml up -d
4. check that you get messages @ mosquitto_pub -t homie/#
5. HOME ASSISTANT - MQTT->entities->BWA


Notes
mosquitto_pub -t "homie/bwa/spa/pump2/set" -m "true"

Todo:
Add my docker compose file
