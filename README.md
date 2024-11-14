# bwa
SPA Bath

Compiled for raspberry
	1. git clone https://github.com/jshank/bwalink.git
	2. docker buildx build --platform linux/arm/v7 -t rogerbwa:v3 .
	3. Docker save
	4. sftp till linux och lägg dit imagen
	5. Docker load …..	
	6. Modify docker-compose ....
		a. Mqtt
		b. Ser2net servern




1. Connect "RS485" cable
2. EWLINK config - https://github.com/jshank/bwalink?tab=readme-ov-file#serial-to-ip-device
3. docker-compose -f docker-compose.yml up -d
4. check that you get messages @ mosquitto_pub -t homie/#
5. HOME ASSISTANT - MQTT->entities->BWA


Notes
mosquitto_pub -t "homie/bwa/spa/pump2/set" -m "true"

Todo:
Add my docker compose file
