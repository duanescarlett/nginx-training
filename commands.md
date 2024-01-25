docker build -t webserver .
docker run -it --rm -d -p 8000:80 --name web webserver

docker compose build
docker compose up -d

nginx -s reload