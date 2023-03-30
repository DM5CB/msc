![Photo by Dominik Scythe on Unsplash](https://user-images.githubusercontent.com/2342458/206678153-044173ab-5203-429d-bd7a-2b0c5f309eea.png)
# Kinsta - Hello World - Static Site with VuePress
An example of how to deploy a static site built with **VuePress** on Kinsta App Hosting services.

---
Kinsta is a developer-centric cloud host / PaaS. We’re striving to make it easier for you to share your web projects with your users. Focus on coding and building, and we’ll take care of deployment and provide fast, scalable hosting. + 24/7 expert-only support.

- [Start your free trial](https://kinsta.com/signup/?product_type=app-db)
- [Application Hosting](https://kinsta.com/application-hosting)
- [Database Hosting](https://kinsta.com/database-hosting)

## Dependency Management

Kinsta automatically installs dependencies defined in your `package.json` file during the deployment process. 

## Web Server Setup

### Port

Kinsta automatically sets the `PORT` environment variable. You should **not** define it yourself and you should **not** hard-code it into the application. The `serve` package utilizes the port set by Kinsta automatically.

### Start Command

When deploying an application, Kinsta automatically creates a web process with `npm start` as the entry point. Make sure to use this command to run your server.

## Deployment Lifecycle

Whenever a deployment is initiated (through creating an application or re-deploying due to an incoming commit) the `npm build` command is run, followed by the `npm start` command.

## What is VuePress
VuePress is a static site generator that allows you to embed dynamic content within your Markdown files using Vue components to produce static HTML pages. More information is available on the [vuepress.github.io](https://vuepress.github.io) website.
