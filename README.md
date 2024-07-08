<p align="center">
  <a href="https://www.medusajs.com">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://user-images.githubusercontent.com/59018053/229103275-b5e482bb-4601-46e6-8142-244f531cebdb.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://user-images.githubusercontent.com/59018053/229103726-e5b529a3-9b3f-4970-8a1f-c6af37f087bf.svg">
      <img alt="Medusa logo" src="https://user-images.githubusercontent.com/59018053/229103726-e5b529a3-9b3f-4970-8a1f-c6af37f087bf.svg" width=100>
    </picture>
  </a>
  <a href="https://railway.app/template/QvfPwp?referralCode=-Yg50p">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://railway.app/brand/logo-light.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://railway.app/brand/logo-dark.svg">
      <img alt="Railway logo" src="https://railway.app/brand/logo-light.svg" width=100>
    </picture>
  </a>
</p>

<h2 align="center">
  Devin-clothes e-commerce platform<br>
  <a href="https://railway.app/template/QvfPwp?referralCode=-Yg50p">one-click deploy on railway!</a>
</h2>

<h1 align="center">
  Welcome to Devin-clothes!<br>
  Your one-stop shop for all your clothing needs.
</h1>





<p align="center">
Combine Medusa's modules for your commerce backend with the newest Next.js 14 features for a performant storefront.</p>

<p align="center">
  <a href="https://github.com/medusajs/medusa/blob/master/CONTRIBUTING.md">
    <img src="https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat" alt="PRs welcome!" />
  </a>
  <a href="https://discord.gg/xpCwq3Kfn8">
    <img src="https://img.shields.io/badge/chat-on%20discord-7289DA.svg" alt="Discord Chat" />
  </a>
  <a href="https://twitter.com/intent/follow?screen_name=medusajs">
    <img src="https://img.shields.io/twitter/follow/medusajs.svg?label=Follow%20@medusajs" alt="Follow @medusajs" />
  </a>
</p>

## About Devin-clothes
Devin-clothes is a modern e-commerce platform designed to provide a seamless shopping experience for clothing enthusiasts. Built with Medusa.js and Next.js, Devin-clothes offers a robust backend and a performant storefront, making it easy to manage products, orders, and customers.

## Setup Instructions
### Railway Setup
1. Change the value of environment variables: `COOKIE_SECRET` and `JWT_SECRET`.
2. Add your `cloud_name`, `api_key`, and `api_secret` to the environment variables in the Railway dashboard to enable Cloudinary in production.

### Local Setup
1. Install dependencies: `yarn`
2. Rename `.env.template` to `.env`
3. To connect to your online database from local, copy the `DATABASE_URL` value that has been auto-generated on Railway and add it to your `.env`

### Requirements
- **Postgres database** (automatically generated if using Railway template)
- **Redis** (automatically generated if using Railway template)

### Optional
- **Cloudinary**: I highly recommend using a proper media service.
  1. Sign up for a free account with [Cloudinary](https://cloudinary.com/invites/lpov9zyyucivvxsnalc5/yhlpdo1vaw2mq1la0nks?t=default) and choose "developer API calls" type of user.
  2. Add your `cloud_name`, `api_key`, and `api_secret` to `.env.local` to enable Cloudinary as a file service on the local dev environment.
  3. Configure the same environment variables in your Railway dashboard to enable Cloudinary in production.
  4. If the steps above are confusing, visit [https://medusajs.com/plugins/medusa-file-cloudinary/](https://medusajs.com/plugins/medusa-file-cloudinary/) for more setup details.

### Commands
`cd medusajs-backend/`
`yarn build` will compile the app.
`yarn dev` will start the local admin dashboard app to manage products and orders, etc.
`yarn start` will start the backend server, needed for the storefront.
