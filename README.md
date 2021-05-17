# docker-getting-started
learning from Docker docs
clone the repo

# inside dockerfile location
docker build -t getting-started .

docker run -dp 3000:3000 getting-started


docker rm -f <>

docker ps
docker stop <>

#browse localhost:3000

#share App

docker tag getting-started lijoj/getting-started

docker push lijoj/getting-started

#try opening in Play with Docker, add instance and run:
docker run -dp 3000:3000 lijoj/getting-started


docker volume create todo-db

docker run -dp 3000:3000 -v todo-db:/etc/todos getting-started


docker volume inspect todo-db
