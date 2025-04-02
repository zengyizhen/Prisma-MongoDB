# Tutorial Steps

## 1. Set Up MongoDB & Prisma
- Create a MongoDB Atlas account: [MongoDB Atlas](https://www.mongodb.com/products/platform/atlas-database?tck=exp-815)
create cluster，add user and password
- Install MongoDB for VS Code.
In VS Code, open "Extensions" in the left navigation and search for "MongoDB for VS Code." Select the extension and click install.
- Run the following commands in terminal:
    ```bash
    npx create-next-app .
    npm i -D prisma
    npx prisma init
    ```
    This will create a new Next.js project and install Prisma.
- Create a MongoDB connection in the `prisma/schema.prisma` file:
    ```prisma
    datasource db {
      provider = "mongodb"
      url      = env("DATABASE_URL")
    }
    ```

## 2. Define Data Models
- Define your data models in the `prisma/schema.prisma` file.

- Create your Prisma schema and push this schema to MongoDB Atlas.
    ```
    npx prisma db push
    ```

## 3. Prisma Client
- create lib/pisma.ts


## 4. Creare API routes
- create app/actions.ts

## 5. Frontend Integration
- Connect your frontend to the API and display data.
```
npx shadcn@latest init
```
