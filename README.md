# Wedding Planner Database Schema and Core Functions

EverAfter Planner is a desktop-first, B2B Wedding Planning Dashboard built using React, TypeScript, Tailwind CSS, and real-time data updates. It includes a complete client CRM, project management system, vendor directory, scheduling calendar, interactive wedding timeline builder, task manager, budget tracker, and lead pipeline — all inside a polished, modern admin interface.
  
<img width="1411" height="695" alt="image" src="https://github.com/user-attachments/assets/f8ef336b-15ec-474c-9fc3-424c257ff9e7" />

<img width="1897" height="931" alt="image" src="https://github.com/user-attachments/assets/0888ff1f-775c-46aa-a12d-b2b275fb01a6" />

<img width="1910" height="923" alt="image" src="https://github.com/user-attachments/assets/e2d4e95e-2c0b-4f9f-b953-fdf4d0900cb1" />

<img width="1907" height="933" alt="image" src="https://github.com/user-attachments/assets/a63102ed-53c2-4c25-9e1a-ef69c27acff4" />

<img width="1907" height="926" alt="image" src="https://github.com/user-attachments/assets/b6d7bab5-115e-4db0-92b0-055d2de8960e" />


This is a project built with [Chef](https://chef.convex.dev) using [Convex](https://convex.dev) as its backend.
 You can find docs about Chef with useful information like how to deploy to production [here](https://docs.convex.dev/chef).
  
This project is connected to the Convex deployment named [`mild-seal-554`](https://dashboard.convex.dev/d/mild-seal-554).
  
## Project structure
  
The frontend code is in the `app` directory and is built with [Vite](https://vitejs.dev/).
  
The backend code is in the `convex` directory.
  
`npm run dev` will start the frontend and backend servers.

## App authentication

Chef apps use [Convex Auth](https://auth.convex.dev/) with Anonymous auth for easy sign in. You may wish to change this before deploying your app.

## Developing and deploying your app

Check out the [Convex docs](https://docs.convex.dev/) for more information on how to develop with Convex.
* If you're new to Convex, the [Overview](https://docs.convex.dev/understanding/) is a good place to start

* Check out the [Hosting and Deployment](https://docs.convex.dev/production/) docs for how to deploy your app

* Read the [Best Practices](https://docs.convex.dev/understanding/best-practices/) guide for tips on how to improve you app further

## HTTP API

User-defined http routes are defined in the `convex/router.ts` file. We split these routes into a separate file from `convex/http.ts` to allow us to prevent the LLM from modifying the authentication routes.
