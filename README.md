Getting Started
Clone the Project First, clone the project from the repository:

git clone https://github.com/mizanur090148/link-harvester.git

Build and Run Docker Containers
Navigate to the project directory and run the following command to build and start the Docker containers:

docker-compose build && docker-compose up

Access the Container To access the container, use the following command:

docker exec -it [containerId] /bin/bash
Replace [containerId] with the ID of the container you want to access.

Update Composer Dependencies
Inside the container, run the following command to update Composer dependencies:

composer update

Run Migrations
After updating Composer dependencies, run the migrations to set up the database:

php artisan migrate