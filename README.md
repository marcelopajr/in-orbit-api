# 🪐 in.orbit API

Goal management app built with Node.js, TypeScript, Docker, PostgreSQL, Drizzle ORM, Fastify, Day.js, Zod and Biome.

## Running

This project depends on Docker to setup database. With Docker installed, clone the project, install  dependencies, setup Docker containers and run the application.

> You must also run migrations to create database tables and run the seed to populate the database with fake data.

First you must create a .env file using the same content as .env.example. Then follow the commands bellow.

```sh
npm i
docker compose up -d
npx drizzle-kit generate
npx drizzle-kit migrate
npm run seed
npx drizzle-kit studio
npm run dev
```

## Features

> The **summary** of the features are listed below.

- it should be able to register a new goal
- it should be able to get the list of all previous goal
- it should be able to manage weekly goals
- it should be able to track the frequency of goal completion
- it should be able to view progress metrics for each goal