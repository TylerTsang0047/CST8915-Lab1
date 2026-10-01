# CST8915 Lab 1: Algonquin Pet Store on Azure VM

**Student Name**: Tyler Tsang
**Student ID**: 041297555
**Course**: CST8915 Full-stack Cloud-native Development
**Semester**: Fall 2026

---

## Demo Video

[Watch Demo Video](https://youtu.be/m7wPVBIYPAw)

---

## Technical Explanations

### Order Service (Node.js)

This service is responsible for completing the order function on the website. It run once the order button is clicked and it calculates the amount the food costs based on the quantity requested and the selection of food the user would like to buy. This service uses node.js as its language and it uses this due to it requiring functionality to compute and output results to complete its service and node.js is a language capable of this and working with the other services. This fits into the microservice architecture by providing the service of the order button and giving the rabbit mq service the orders. This interacts with the other services by getting the quantity and users selection from the store front and computing the amount total from the product service.

### Product Service (Rust)

This service is responsible for providing the website with what options are available for order and the prices of each. This service uses Rust as its language and it is used because rust is a good language that works well with cloud services. It is a strong language that makes deployment easy and it is fast at retrieving data. This fits into the microservice architecture by retrieving the holding the information about what products are available and their prices and providing them when requested. This interacts with the other services by providing the store front the options the user can choose from and the prices to display for each in addition to providing the order service with the information to calculate the total amounts owed for the users selections. 

### Store Front (Vue.js)

This service is responsible for displaying the website for the user. This service uses uve.js as its language and it is used because it is a dynamic language that is able to update the website in real time. In addition to this, Vue.js is built to be used for small scale projects so it is a good choice for this. This fits into the microservice architecture by providing the user with the interface of the website and displaying the information to the user as well as letting the user interact with the system thorough selecting their items, quantity and sending their order in. This interacts with the other services by getting the information to display from the product services and then send the information to the order service to be processed.


---

## Resources

- https://bitfieldconsulting.com/posts/why-rust
- https://www.techmagic.co/blog/benefits-of-vuejs


