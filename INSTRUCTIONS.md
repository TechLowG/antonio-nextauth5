### Initial Setup

`npx create-next-app@14.0.4 antonio-nextauth5-clone`
```
√ Would you like to use TypeScript? Yes
√ Would you like to use ESLint? Yes
√ Would you like to use Tailwind CSS? Yes
√ Would you like to use `src/` directory? No
√ Would you like to use App Router? (recommended) Yes
√ Would you like to customize the default import alias (@/\*)? No
```
`cd folder`

### Environment Setup

`npx shadcn-ui@latest init`
```
√ Which style would you like to use? » New York
√ Which color would you like to use as base color? » Slate
√ Would you like to use CSS variables for colors? ... yes
```

`npx shadcn-ui@latest add button`

### Routing 

...

### Home page

...

### Card Wrapper

```
npx shadcn-ui@latest add card
npm i react-icons@4.12.0
```

### Login Form

`npx shadcn-ui@latest add form input label`

### Register Form

...

### Database & Prisma Setup

NeonDB: https://neon.tech/ - login - create service

```
npm i -D prisma
npm i @prisma/client
npx prisma init
npx prisma generate
npx prisma db push
npx prisma studio
npm i @auth/prisma-adapter@1.0.12
```

.env
```
DATABASE_URL=
DIRECT_URL=
AUTH_SECRET="secret"
```

.package.json
```
"scripts": {
    "postinstall": "prisma generate"
  },
```

### Register Functionality

```
npm i bcrypt@5.1.1 bcryptjs@2.4.3
npm i -D @types/bcrypt@5.0.2 @types/bcryptjs@2.4.6
localhost - create an user
```

### Middleware

Update Guide (v5): https://authjs.dev/guides/upgrade-to-v5

```
npm i next-auth@beta
- check http://localhost:3000/api/auth/providers work
- login with user email & password
- signOut
- create new account called test - login
```

### Deployment

foreach
```
git add .
git commit -m "XX: message"
git push
validate deployment succeed
```

once
```
github.com/new - create repo
use second option - "push an existing repo"
.
vercel.com/new - import - deploy
settings - environment variables - add from .env
```