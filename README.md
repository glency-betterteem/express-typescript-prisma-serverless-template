# Express + TypeScript + Prisma + Serverless Template 📃

This is a template for a Express + TypeScript + Prisma + Serverless projects.

### Pre-requisites 📋

- [Node.js](https://nodejs.org/en/download/)
- [Yarn](https://classic.yarnpkg.com/en/docs/install)

### Getting started 🚀

1. Clone the repository
2. Install dependencies with `yarn`
3. Start the development server with `yarn dev`
### Supported ORMs ✅

- [Prisma](https://www.prisma.io/) (default ORM)
- [TypeORM](https://typeorm.io/#/)

### Supports Serverless Deployments 🚀

- [x] AWS Lambda
- [x] Vercel

### Additional Utilities 🛠

- [x] Permission Manager (Attribute-based access control)

### Steps to use TypeORM instead of Prisma 📝

By default, this template uses Prisma. If you want to use TypeORM, follow these steps:

1. `yarn orm:use-typeorm` - This will remove Prisma and install TypeORM
2. Uncomment TypeORM setup in `src/app.ts`

Note: You will need to manually import your entities into `src/entities/index.ts` to make them available during runtime. Path imports cannot be used in serverless environments.

### Why I made Prisma as the default ORM for this template 🤔

Prisma is a great ORM that is easy to use and has a lot of great features. However, it is not as mature as TypeORM. I made Prisma the default ORM because it can generates a client that can be used in serverless environments. This is not the case with TypeORM. If you want to use TypeORM, you will need to manually import your entities into `src/entities/index.ts` to make them available during runtime. Path imports cannot be used in serverless environments. This is a limitation of TypeORM and not this template. If you want to use TypeORM, you can use the steps above to switch to TypeORM. If you want to use Prisma, you can continue using this template as is.

### Feel free to file issues or make pull requests 🤝

If you find any issues or want to make a pull request, feel free to do so. I will try to respond as soon as possible. I am also open to suggestions for improvements. If you have any questions, feel free to ask. I will try to answer as soon as possible. If you want to support this project, feel free to star it. Thanks! 🙂

### References 📚

- [Prisma](https://www.prisma.io/)
- [TypeORM](https://typeorm.io/#/)
- [Serverless](https://www.serverless.com/)
- [Serverless Framework](https://www.serverless.com/framework/docs/)
- [AWS Lambda](https://aws.amazon.com/lambda/)
- [Vercel](https://vercel.com/)
- [Attribute-based access control](https://en.wikipedia.org/wiki/Attribute-based_access_control)

<!-- TODO: Document available commands -->
