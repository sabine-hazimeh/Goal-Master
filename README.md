<img src="./image/title1.svg"/>

<br><br>

<!-- project philosophy -->
<img src="./image/title2.svg"/>

> A web app designed to help users set and achieve their personal goals. The platform combines goal setting, personalized planning, emotional tracking, and consultant interactions to offer a holistic approach to personal development.
>
> GoalMaster empowers users to take control of their personal growth by integrating goal setting with emotional well-being.

### User Stories

- As a user, I want to specify my goals, such as learning new skills, or financial management and the app should help me in achieving it.
- As a user, I want to connect with consultants for personalized advice and guidance.
- As a user, I want to express my emotions using facial expression recognition technology, so that my emotions are recorded.

<br><br>

<!-- Tech stack -->
<img src="./image/title3.svg"/>

### Goal Master is built using the following technologies:

- The frontend is built using [React](https://legacy.reactjs.org/docs/getting-started.html), providing a dynamic and responsive user experience. React allows the app to render efficiently and scale across devices.
- [Laravel](https://laravel.com/docs/11.x/) serves as the backend framework, handling API requests, authentication, and server-side logic. It ensures the application is secure, scalable, and maintainable.
- A relational database [MySQL](https://dev.mysql.com/doc/) is used to store structured data. MySQL's efficient querying and indexing ensure the app performs well with large datasets.
- ML models are integrated to predict both health and education goals. The models analyze user inputs (such as health metrics or learning preferences) and suggest personalized recommendations.
- [OpenAI](https://platform.openai.com/docs/introduction) is used to predict financial goals. Based on user inputs like income, savings, and target date, the system generates savings plans to help users meet their financial objectives.
- [Pusher](https://pusher.com/docs/) is used to implement real-time messaging, enabling live chat functionality between users. The system supports instantaneous communication for a seamless user experience.

<br><br>

<!-- UI UX -->
<img src="./image/title4.svg"/>

> We designed Goal Master by creating detailed wireframes and mockups to visualize the structure and user flow. Throughout the design process, we focused on ensuring easy navigation and an intuitive user experience. After several iterations, incorporating feedback and improvements, we arrived at the final design that offers seamless interaction and effortless goal management for users.

Our goal was to craft a clean, functional interface that helps users focus on achieving their goals without unnecessary distractions.

- Project Figma design [figma](https://www.figma.com/design/1KpW6Me6gTjkifuRnBAuV9/Final-Project?node-id=0-1&node-type=CANVAS&t=vPxHLN63RMYazSpM-0)

### Mockups

| Home screen                             | About Us Screen                           | 
| --------------------------------------- | ------------------------------------- | 
| ![Home](image/home.png) | ![About](image/about.png) | ![fsdaf](./readme/demo/1440x1024.png) |

<br><br>

<!-- Database Design -->
<img src="./image/title5.svg"/>

### Architecting Data Excellence: Innovative Database Design Strategies:

- ![ERDiagram](image/ER-Diagram.png)

<br><br>

<!-- Implementation -->
<img src="./image/title6.svg"/>

### User Screens (Web)

| Login screen                            | Profile screen                       | 
| --------------------------------------- | ------------------------------------- | 
| ![Login](image/Login.png) | ![profile](image/profile.png) | ![fsdaf](./readme/demo/1440x1024.png) |
| Live Chat                             | Education Goal                           | Order Screen                          |
| ![Live Chat](image/LiveChat.gif) | ![Education Goal](image/EducationGoal.gif) | ![fsdaf](./readme/demo/1440x1024.png) |

<br><br>

<!-- Prompt Engineering -->
<img src="./image/title7.svg"/>

### Mastering Personalized Learning: Harnessing Machine Learning for Tailored Course and Exercise Recommendations

- This project utilizes machine learning techniques to personalize learning experiences by recommending courses that align with the user's educational goals and unique conditions. By analyzing the user’s health status, the system also predicts and suggests appropriate exercises. This approach enables precise and efficient recommendations, optimizing both the user’s learning progress and physical well-being.

<br><br>

<!-- AWS Deployment -->
<img src="./image/title8.svg"/>

### Efficient AI Deployment: Unleashing the Potential with AWS Integration:

- This project leverages AWS deployment strategies to seamlessly integrate and deploy natural language processing models. With a focus on scalability, reliability, and performance, we ensure that AI applications powered by these models deliver robust and responsive solutions for diverse use cases.

<br><br>

<!-- Unit Testing -->
<img src="./image/title9.svg"/>

### Accuracy in Development: Leveraging Unit Testing's Power:

- Precise unit testing techniques are applied in this project to guarantee the quality and dependability of code components. We ensure a solid foundation by carefully examining each software unit, spotting and fixing any problems early on in the development cycle.

<br><br>

<!-- How to run -->
<img src="./image/title10.svg"/>

> To set up Goal Master locally, follow these steps:

### Prerequisites


- npm
  ```sh
  npm install npm@latest -g
  ```
- npm
  ```sh
  php -r "copy('https://getcomposer.org/installer', 'composer-setup.php');"
  php composer-setup.php
  php -r "unlink('composer-setup.php');"
  ```
- you can download PHP from [here](https://www.php.net/downloads)
- you can download MySQL from [here](https://dev.mysql.com/downloads/installer/)


### Installation


1. Clone the repo
   ```sh
   git clone https://github.com/sabine-hazimeh/goal-master
   ```
2. Install NPM packages
   ```sh
   npm install
   ```
3. Get an OpenAI Key 
4. Create new pusher app and add it's credentials to laravel .env file
   ```js
   PUSHER_APP_ID="enter your id"
   PUSHER_APP_KEY="enter your key"
   PUSHER_APP_SECRET="enter your secret"
   PUSHER_APP_CLUSTER="enter your cluster"
   BROADCAST_DRIVER=pusher
   ```
5. Enter OpenAI key and pusher credentials in react .env file
   ```js
    REACT_APP_OPENAI_API_KEY = "ENTER YOUR API";
    REACT_APP_PUSHER_KEY = "ENTER YOUR KEY";
    REACT_APP_PUSHER_CLUSTER = "ENTER YOUR CLUSTER";
   ```
6. - Install Tymon JWT package via Composer:
     ```sh
     composer require tymon/jwt-auth
     ```
   - Publish the configuration file:
     ```sh
     php artisan vendor:publish --provider="Tymon\JWTAuth\Providers\LaravelServiceProvider"
     ```
   - Generate a JWT secret key:
     ``` sh
     php artisan jwt:secret
     ```
     


Now, you should be able to run Goal Master locally and explore its features.
