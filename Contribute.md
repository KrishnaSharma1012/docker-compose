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
 -start POStgres
  - docker run -e POSTGRES_PASSWORD=mysecretpassword -d -p 5432:5432 postgres

   - Build the image - `docker build -t user-project .`
   -Start the image - `docker run -p 3000:3000 user-project`



 ## docker compose installation steps
 - install docker ,docker-compose
 -Run `docker-compose up`