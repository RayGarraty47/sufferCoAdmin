This is a full-stack e-commerce dashboard plus CMS using Next.js 13 App Router, React, Tailwind, Prisma, and MySQL

It was made using the folowing [tutorial](https://www.youtube.com/watch?v=5miHyP6lExg)

Clerk is currently used as an Auth service with plans to replace this in the future

Cloudinary is used for image uploads and storage

## Getting Started

Clone the repo

```bash
git clone https://github.com/RayGarraty47/sufferCoAdmin.git
```

install packages

```bash
npm i
```

setup .env 

```bash
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=
NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/

# This was inserted by `prisma init`:
# Environment variables declared in this file are automatically made available to Prisma.
# See the documentation for more detail: https://pris.ly/d/prisma-schema#accessing-environment-variables-from-the-schema

# Prisma supports the native connection string format for PostgreSQL, MySQL, SQLite, SQL Server, MongoDB and CockroachDB.
# See the documentation for all the connection string options: https://pris.ly/d/connection-strings

DATABASE_URL=''
NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=""
STRIPE_API_KEY=
FRONTEND_STORE_URL=http://localhost:3001
STRIPE_WEBHOOK_SECRET=
```

Connect to PlanetScale and Push Prisma

```bash
npx prisma generate
npx prisma db push
```

Start the app

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.
