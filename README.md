# Containerisation of a simple web application using Docker

## Cloning Repository or Creating an app.js File

1. Clone this repository or create an `app.js` file in your directory or make a basic application named `app.js`.

2. Navigate to the project directory on GitHub.

## Installing Node.js and Express

3. Make sure to install Node.js in the directory using the following commands:
    ```
    npm init -y
    npm install express
    ```

## Creating a Dockerfile

4. Create a `Dockerfile` in the project directory.

5. Use the code provided in the `Dockerfile` in this repository.

## Creating a Docker Compose File

6. Create a `docker-compose.yml` file in the project directory.

7. Copy the code from the `.yml` file in this repository and paste it into your project.

## Building the Docker Image

8. Build the Docker Image by using the following command:
    ```
    docker build -t my-web-app .
    ```
    Replace `<my-web-app>` with your desired name and make sure to put a `.` after space.

## Starting the Build Environment

9. After the image has been created, start the build environment by using the following command:
    ```
    docker-compose up -d
    ```

## Testing the Application

10. Open a web browser and navigate to [http://localhost:3000](http://localhost:3000) (or the ports defined).

11. You should see the message from your `app.js` file.

## Pushing the Docker Image to a Registry

12. Tag the Docker image using the following command:
    ```sh
    docker tag web-app lavyabansal7/task5.1p:tag
    ```
    Replace `web-app` with the name of your Docker image, `username/repository` with your Docker Hub username and the desired repository name and tag

13. Push the Docker image to the registry using the following command:
    ```sh
    docker push username/repository:tag
    ```
    And now once again replace `username/repository:tag` with your Docker Hub username, repository name, and tag name.
