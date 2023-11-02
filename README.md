<p align="center">
  <a href="http://nestjs.com/" target="blank"><img src="https://nestjs.com/img/logo-small.svg" width="200" alt="Nest Logo" /></a>
</p>

# Run development environment

1. Clone repository
2. Run

```
yarn install
```

3. Install Nest CLI

```
npm i -g @nestjs/cli
```

4. Build the database

```
docker-compose up -d
```

5. Add env variables to **.env** file

6. Run the app in dev mode

```
yarn start:dev
```

7. Apply seed data to database

```
localhost:3000/api/v2/seed
```

# Stacks

- MongoDB
- Nest

# Production Build

1. Create the `.env.prod` file

2. Fill in the prod env variables

3. Create the new image

```
docker-compose -f docker-compose.prod.yaml --env-file .env.prod up --build
```
