start server 
java -jar paper-1.20.2-318.jar

install 
curl -s https://ngrok-agent.s3.amazonaws.com/ngrok.asc | sudo tee /etc/apt/trusted.gpg.d/ngrok.asc >/dev/null && echo "deb https://ngrok-agent.s3.amazonaws.com buster main" | sudo tee /etc/apt/sources.list.d/ngrok.list && sudo apt update && sudo apt install ngrok && ngrok authtoken 2ZkrzSf7zT26qliaAdVMcYPM5qa_2iHGbwncuasNJy2sE4JkC && ngrok tcp 25565




