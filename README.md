[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contact">Contact</a></li>
  </ol>
</details>



<!-- ABOUT THE PROJECT -->
## About The Project

<!-- [![Product Name Screen Shot][product-screenshot]](https://example.com) -->
I wanted to learn Python for the BACKEND and stumbled upon a course that would guide me in building a fully functioning REST API that can handle:
* User authentication
* Creating objects
* Filtering and sorting objects
* Uploading and viewing images
* Setting up a project with Docker and Docker-Compose
* Configure GitHub Actions to automatically run linting and unit tests
* Write unit tests using the Django Test Framework
* Apply best practice principles including Test Driven Development
* Handle uploading media files with Django
* Customize the Django admin
* Configure a Postgres database


<p align="right">(<a href="#readme-top">back to top</a>)</p>



### Built With


* ![Postgres](https://img.shields.io/badge/postgres-%23316192.svg?style=for-the-badge&logo=postgresql&logoColor=white)
* ![Docker](https://img.shields.io/badge/docker-%230db7ed.svg?style=for-the-badge&logo=docker&logoColor=white)
* ![Django](https://img.shields.io/badge/django-%23092E20.svg?style=for-the-badge&logo=django&logoColor=white)
* ![Swagger](https://img.shields.io/badge/-Swagger-%23Clojure?style=for-the-badge&logo=swagger&logoColor=white)
* ![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=for-the-badge&logo=githubactions&logoColor=white)





<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running follow these simple example steps.

### Prerequisites

* Install [Docker / Docker Compose](https://docs.docker.com/get-docker/)
* Verify docker-compose is installed by running this command in the terminal
  ```sh
  docker-compose --version
  ```


### Installation


Run the following commands in the terminal:
1. Clone the repo
    ```sh
    git clone https://github.com/dGarcia-NC/recipe-app-api.git
    ```
2. Change directories into the newly cloned repo
   ```sh
   docker-compose up
   ```
3. On a separate terminal run
   ```sh
   docker-compose run --rm app sh -c "python manage.py createsuperuser"
   ```
4. Visit [http://127.0.0.1:8000/api/docs](http://127.0.0.1:8000/api/docs) in your browser

### Make some requests to the backend
1. Create a token by making a **POST** request to:
   ```sh
   /api/user/token
   ```
2. Copy the the token from the response
3. Scroll to the top of the docs screen and click on the **Authorize** button
4. Past the token to the value of the **tokenAuth (apiKey)** section and close that modal
5. Make a **GET** request to:
   ```sh
   /api/recipe/recipes/
   ```
6. The response should be an empty Array since you haven't added a recipe yet
7. Make a **POST** request to add a recipe:
   ```sh
   /api/recipe/recipes/
   ```
8. Repeat step 5 and you'll see the recipe you added
9. Feel free to make additional request

<p align="right">(<a href="#readme-top">back to top</a>)</p>



<!-- USAGE EXAMPLES -->
## Usage

Hey there 👋. Here's what a GIF of my API docs put together using Swagger.

![image](https://drive.google.com/uc?export=view&id=1gQrPbFVrpoXIvFRb5qarj56JZgoysDp7)

## List of Endpoints
### recipe
|Request Type|Endpoint Name|
|---|---|
|GET|​/api​/recipe​/ingredients​/|
|PUT|​/api​/recipe​/ingredients​/{id}​/|
|PATCH|/api​/recipe​/ingredients​/{id}​/|
|DELETE|​/api​/recipe​/ingredients​/{id}​/|
|GET|​/api​/recipe​/recipes​/|
|POST|​/api​/recipe​/recipes​/
|GET|​/api​/recipe​/recipes​/{id}​/|
|PUT|​/api​/recipe​/recipes​/{id}​/|
|PATCH|​/api​/recipe​/recipes​/{id}​/|
|DELETE|/api​/recipe​/recipes​/{id}​/|
|POST|​/api​/recipe​/recipes​/{id}​/upload-image​/|
|GET|​/api​/recipe​/tags​/|
|PUT|​/api​/recipe​/tags​/{id}​/|
|PATCH|​/api​/recipe​/tags​/{id}​/|
|DELETE|​/api​/recipe​/tags​/{id}​/|

### schema
|Request Type|Endpoint Name|
|---|---|
|GET|/api​/schema​/|

### user
|Request Type|Endpoint Name|
|---|---|
|POST|​/api​/user​/create​/|
|GET|/api​/user​/me​/|
|PUT|/api​/user​/me​/|
|PATCH|​/api​/user​/me​/|
|POST|​/api​/user​/token​/|




<p align="right">(<a href="#readme-top">back to top</a>)</p>


<!-- CONTACT -->
## Contact

David Garcia: AnthonyGarcia833@gmail.com

Project Link: [https://github.com/dGarcia-NC/recipe-app-api](https://github.com/dGarcia-NC/recipe-app-api)

<p align="right">(<a href="#readme-top">back to top</a>)</p>




<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/dGarcia-NC/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/dGarcia-NC/recipe-app-api/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/dGarcia-NC/recipe-app-api/forks
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/dGarcia-NC/recipe-app-api/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/dGarcia-NC/recipe-app-api/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/othneildrew/Best-README-Template/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/davidanthonygarcia/
[product-screenshot]: images/screenshot.png
[Next.js]: https://img.shields.io/badge/next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[Vue.js]: https://img.shields.io/badge/Vue.js-35495E?style=for-the-badge&logo=vuedotjs&logoColor=4FC08D
[PostgreSQL-url]: https://www.postgresql.org/
[Angular.io]: https://img.shields.io/badge/Angular-DD0031?style=for-the-badge&logo=angular&logoColor=white
[Angular-url]: https://angular.io/
[Svelte.dev]: https://img.shields.io/badge/Svelte-4A4A55?style=for-the-badge&logo=svelte&logoColor=FF3E00
[Svelte-url]: https://svelte.dev/
[Laravel.com]: https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white
[Laravel-url]: https://laravel.com
[Bootstrap.com]: https://img.shields.io/badge/Bootstrap-563D7C?style=for-the-badge&logo=bootstrap&logoColor=white
[Bootstrap-url]: https://getbootstrap.com
[JQuery.com]: https://img.shields.io/badge/jQuery-0769AD?style=for-the-badge&logo=jquery&logoColor=white
[JQuery-url]: https://jquery.com
