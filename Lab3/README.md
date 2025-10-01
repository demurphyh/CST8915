# CST8915 Lab 3

## Youtube Walkthrough Link

[Youtube Link](https://youtu.be/btlJuNJuedE)

## Reflection Questions

### What challenges did you encounter when configuring environment variables in the GitHub Actions workflow?

- I wasn't able to deploy my store front on a static web app due to account policies so I don't have experiece configuring environment variables in Github Actions workflow.

### How does deploying microservices on Azure Web App Service differ from running them locally?

- When deploying an app locally or in a vm you need to configure the entire application yourself including downloading all the required dependencies, whereas with an Azure web service they handle everything themselves at runtime downloading all the dependencies and runtimes at runtime which means you just need to push your code and the app service can automatically configure it,

### Why is it important to use environment variables for configurations in a cloud environment?

- Environment variables in cloud are important because the application can be deployed in many different places and azure automatically decides on an address or ip for the app. So an environment variable means that you dont need to touch the code when its deployed to a new place, only the environment cariable settings need to change.

## Github Links

[Store Front](https://github.com/demurphyh/store-front.git)

[Product Service](https://github.com/demurphyh/product-service)

[Order Service](https://github.com/demurphyh/order-service)
