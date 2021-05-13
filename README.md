# Strapi + Nuxt Project Structure

Proof of concept for a project structure using Strapi Headless CMS as back-end and Nuxt, TypeScript, and Apollo as front-end.

## Running locally

Run the following commands:

 - `docker-compose up -d` to start Strapi and PostgreSQL
 - `cd frontend && npm run dev` to start Nuxt development environment

Now you can access:

 - [Strapi Admin](http://localhost:1337/admin/auth/login)
 - [GraphQL Playground](http://localhost:1337/graphql)
 - [Web app](http://localhost:3000/)

## Technologies

The following tools were used in the construction of the project:

 - [Strapi](https://strapi.io/)
 - [GraphQL](https://graphql.org/)
 - [Apollo](https://www.apollographql.com/)
 - [Nuxt](https://nuxtjs.org/)
 - [TypeScript](https://www.typescriptlang.org/)