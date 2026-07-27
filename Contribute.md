## Manual installation
 -Install nodejs locally()
 -cloner the repo
 -install dependencies (npm install)
 -start the DB locally
 -docker run -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres
 -go to neon.tech and get yourself a new DB
 -change the .env file and update your DB credentials
 -npx prisma migrate
 -nps prisma generate
 -npx run build
 -npm run start


 ## docker installation

 -install docker
 start a new network -`docker network create user_project`
 
 -start POStgres
  - docker run --network user_project --name postgres -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres

   - Build the image - `docker build --network=host -t user_project .`
   -Start the image - `docker run -e DATABASE_URL=postgresql://postgres:mysecretpassword@postgres:5432/postgres  --network user_project -p 3000:3000 user_project`



 ## docker compose installation steps
 - install docker ,docker-compose
 -Run `docker-compose up`