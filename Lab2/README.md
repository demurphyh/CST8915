# CST8915 Lab 2

## Youtube Walkthrough Link

[Youtube Video](https://www.youtube.com/watch?v=X4CL2tWR63g)

## Reflection Questions

### What changes did you make to the order-service and product-service to comply with the Configurations and Backing Services factors of the 12-Factor App methodology?

- We changed the variables from being hardcoded to declaring them in .env files and then refrencing them in order to be more in line with 12-Factor app methodology.

### Why is it important to use environment variables instead of hard-coding configurations in your application?

- It's important to use environment variables in order to make our code more readable and easier to alter in the future. With hard coded variables it can be easy to make mistakes in code and hard to find what you need to change if the URL for example changes. with environment variables you just need to change where the variable points if a URL changes and the rest of your code stays the same. Environemnt variables allow or code more readable and adaptable to changes.

### Why is it important to have separate repositories for each microservice? How does this help maintain independence and scalability of each service?

- Seperate repositories for each microservice is important because it allows allows us to have seperate codebases for each service so when a change is made in one microservice it won't introduce bugs or break another microservice. This helps maintain independence because it allows different teams to work on different parts of the application without intefereing with eachother. It also allows different services within the application to be coded in different languages, for our application thats node.js, rust and vue. When we seperate the repos for every microservice it allows us to scale the different microservices based on needs instead of having to scale the entire application if its all in a single repo.

## Github Links

[Store Front](https://github.com/demurphyh/store-front.git)

[Product Service](https://github.com/demurphyh/product-service)

[Order Service](https://github.com/demurphyh/order-service)
