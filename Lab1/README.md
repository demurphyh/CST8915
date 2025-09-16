# CST8915 Lab 1

## Youtube Walkthrough Link

[Youtube Link](https://www.youtube.com/watch?v=61JWR9mLQ4E)

## Technical Analysis

### Order Service

- The Order Service is responsible for raking orders from the storefront and sending them to RabbitMQ to manage and store them. The Order Service is written using Node.js. The Order Service package interacts with both our Store Front and RabbitMQ. It receives orders that are placed through the Storefront and sends them to RabbitMQ in order to save them.

### Product Service

- The Product Service package is a backend service responisble for maintaining the product catalog and provides an API which can be used to fetch the product list. It is written using the rust language and utilizing the Warp web framework to handle http requests. The Product Service provides an API that the Store Front can use to display the product list.

### Store Front

- The Store Front service is a front end service that allows users to see and select products and then place orders. Store Front is written using Vue.js. The Store Front service interacts with both the Order Service and Product Service. It interacts with the Product Service in order to fetch and display the product list on the front end and it interacts with the order service in order to handle orders placed on the front end.
