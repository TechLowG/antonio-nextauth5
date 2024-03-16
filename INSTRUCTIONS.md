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
```

.package.json
```
"scripts": {
    "postinstall": "prisma generate"
  },
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