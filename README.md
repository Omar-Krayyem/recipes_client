<img src="./Readme/title1.svg"/>
<br><br>

<br><br>
<img src="./Readme/title7.svg"/>
<br><br>
- [Project Description](#project-description)
- [User Types](#user-types)
- [User Stories](#User-Stories)
- [Tech Stack](#Tech-stack)
- [Prototyping](#prototyping)
- [Demo](#Demo)
- [Backend](#Backend)
- [Performance](#Performance)
- [How to Run](#How-to-run)
 
  
<br><br>
<img src="./Readme/title2.svg"/>
<br><br>

<a name="project-description"></a>
> DishDiscovery is a comprehensive application designed to cater to the needs of food enthusiasts, home chefs, and meal planners. It's a platform where users can explore, share, and plan their culinary adventures. With a focus on user engagement and culinary delight, RecipeHub offers a wide range of features to enhance the cooking and meal planning experience.
>

### User Types 
1. User

### User Stories

As User: 

- I want to explore a wide variety of recipes by name, cuisine, or ingredients.
- I want to view recipe details, including ingredients and images.
- I want to like, comment on, and share recipes on social media.
- I want to search for recipes based on dietary preferences, such as vegetarian, gluten-free, or keto.
- I want to create shopping lists based on the ingredients of recipes I choose.

<br><br>
<img src="./Readme/title3.svg"/>
<br><br>

### Mockups 

>We designed Fatal Breath using wireframes and mockups, iterating on the design until we reached the ideal layout for easy navigation and a seamless user experience.

| Landing Page  | Login | Signup |
| ---| ---| ---|
| ![Landing](./Readme/mockups/Landing_page.svg) | ![Login](./Readme/wireframes/Signin.svg) | ![Signup](./Readme/mockups/Signup.svg) |
| Dashboard | Requests | Requests Form |
| ![Dashboard](./Readme/mockups/Dashboard.svg) | ![Requests](./Readme/mockups/Request.svg) | ![Requests Form](./Readme/mockups/Request_Form.svg) |
| Profile | Partners | Partners Form |
| ![Profile](./Readme/mockups/Profile.svg) | ![Partners](./Readme/mockups/Partners.svg) | ![Partners Form ](./Readme/mockups/Partners_Form.svg) |
| Workers | Workers Form | Stored Items |
| ![Workers](./Readme/mockups/Workers.svg) | ![Workers Form](./Readme/mockups/Workers_Form.svg) | ![Stored Items](./Readme/mockups/Stored_Items.svg) |
| Stored Items Form | Incoming Orders | Incoming Order Details |
| ![Stored Items Form ](./Readme/mockups/Stored_Items_Form.svg) | ![Placed Orders](./Readme/mockups/Incoming.svg) | ![Placed Order](./Readme/mockups/Incoming_Detail.svg) |
| Outgoing Orders | Incoming Order Details |
| ![Shipment Orders](./Readme/mockups/Outgoing.svg) | ![Shipment Order](./Readme/mockups/Outgoing_Detail.svg) |


<br><br>
<img src="./Readme/title5.svg"/>
<br><br>

### Tech-stack 
###  Storage Park is built using the following technologies:

- This project uses the [React Library](https://react.dev/) for the frontend development.
- This project uses [Laravel](https://laravel.com/), a PHP web application framework. Laravel simplifies web development by providing robust tools and an expressive syntax for building secure and scalable web applications.
- [MySQL](https://www.mysql.com/) for the database. It is an open-source relational database management system.
- Storage Park includes hardware integration with an ESP8266 microchip connected to a GPS sensor to get location.

<br><br>
<img src="./Readme/title4.svg"/>
<br><br>

### Demo
Using the wireframes and mockups as a guide, we implemented the Storage Park app with the following features:

| Landing Page  | Tracking Order | Login |
| ---| ---| ---|
| ![Landing](./Readme/demo/landing_page.gif) | ![Tracking Order](./Readme/demo/tracking_order.gif) | ![Login](./Readme/demo/login.gif) |
| Registration | View Stock | Add New Order |
| ![Registration](./Readme/demo/registration.gif) | ![Requests](./Readme/demo/view_stock.gif) | ![Add New Order](./Readme/demo/add_order.gif) |
| Change Password |
| ![Change Password](./Readme/demo/change_password.gif) |
<br><br>

<img src="./Readme/title10.svg"/>
<br><br>
### Backend
[Backend Repository](https://github.com/Omar-Krayyem/dishdiscovery_server.git)
<br><br>
<a name="Performance" ></a>
<img src="./Readme/title9.svg"/> 
> The following tests were conducted in Postman to assess the functionality of my application's primary APIs
<br><br>

URL: http://127.0.0.1:8000/api/MyRecipes

```sh 
PASS: Response time is within acceptable range //199 ms
PASS: Response content type is JSON
PASS: Response schema is valid
PASS: Response has the required field - message
PASS: Response content type is JSON

```

<br>
URL: http://127.0.0.1:8000/api/recipe/10

```sh 
PASS: Response time is within acceptable range //258 ms
PASS: Response content type is JSON
PASS: Response schema is valid
PASS: Response has the required field - message
PASS: Response content type is JSON
```

<br><br>
<img src="./Readme/title6.svg"/>
<br><br>
### How-to-run

> To set up Storage Park locally, follow these steps:

## Prerequisites
- MySQL
	1) Follow these instructions to setup MySQL: [MySQL Insrallation](https://www.w3schools.com/mysql/mysql_install_windows.asp)

## Installation

1) Clone the frontend repo

   ```sh
   git clone https://github.com/Omar-Krayyem/storage_park_client.git
   ```

2) Clone the backend repo

   ```sh
   git clone https://github.com/Omar-Krayyem/storage_park_server.git
   ```

3) Install Laravel dependencies by navigating to the Laravel project directory:

   ```sh
   cd laravel-backend
   composer install
   ```

4) Set up your Laravel environment and configure the .env file with your database settings.

   Run Laravel migrations to set up the database:

   ```sh
   php artisan migrate
   ```

5) Launch the server
	- Navigate to the server repo
	- Run this command	
	```sh
	php artisan serve
	```

6) Launch the frontend
	- Navigate to the frontend repo
	- Run this command	
	```sh
	npm start
	```
<br>

Now, you should be able to run **Storage Park** locally and explore its features
