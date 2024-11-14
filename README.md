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

docker-compose -f docker-compose.yml up -d ![image](https://github.com/user-attachments/assets/550842b8-79d0-4d68-ba28-b3f40d45682d)


1. EWLINK - config see
2. 


Notes
mosquitto_pub -t "homie/bwa/spa/pump2/set" -m "true"

Todo:
Add my docker compose file
