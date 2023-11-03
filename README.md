# Project Setup Guide

Follow these steps to set up and run this project. We need to set up two different projects one for backend and one for frontend.

## Prerequisites

Before you begin, ensure you have the following installed:

- PHP >= 7.3
- Laravel >= 8
- Node >= 16.0
- Docker

## Getting Started

1. Clone the repository:

   ```bash
   git clone https://bitbucket.org/matheenshariff/assignment-19-10-2023.git/

   ```

2. First we will set up backend.

   Make sure `docker` is installed in your system. If not click here [https://docs.docker.com/engine/install/](https://docs.docker.com/engine/install/)

3. Navigate to the backend project directory:

   ```bash
   cd backend
   ```

4. Install project dependencies:

   ```bash
    composer install
   ```

## Configuration

6.  Configure the project by copying the `.env.example` file to `.env` and fill in the required environment variables.
    ```bash
    cp .env.example .env
    ```
7.  Change the database credentials as per your Database

         db_connection
         db_host
         db_port
         db_database
         db_username
         db_password

    Run the following commands

    ```bash
    php artisan migrate
    php artisan db:seed //To insert the default roles
    ```

## Running the Project

8. Start the development server:

   ```bash
   ./vendor/bin/sail up
   ```

9. Now we will set up frontend
   Now come back to root directory and go to
   ```bash
   cd ../
   cd client
   ```
10. Install project dependencies:

    ```bash
     npm install
    ```

## Running the Project

11. ```bash
     npm run dev
    ```

12. Open your web browser and visit [http://127.0.0.1:5174/](http://127.0.0.1:5174/) to see the project in action.

Happy coding!
