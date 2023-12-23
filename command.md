start server 
cd mc && java -jar paper-1.20.2-318.jar

install 
curl -s https://ngrok-agent.s3.amazonaws.com/ngrok.asc | sudo tee /etc/apt/trusted.gpg.d/ngrok.asc >/dev/null && echo "deb https://ngrok-agent.s3.amazonaws.com buster main" | sudo tee /etc/apt/sources.list.d/ngrok.list && sudo apt update && sudo apt install ngrok && ngrok authtoken 2ZkrzSf7zT26qliaAdVMcYPM5qa_2iHGbwncuasNJy2sE4JkC && ngrok tcp 25565

sudo nano /etc/hosts

127.0.0.1   caaqil

nano ~/.ssh/config
Host caaqil
    HostName serveo.net
    Port 25565  # your desired port
    User salaadma01


ssh -R caaqil:25565:localhost:25565 serveo.net
