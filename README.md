1. Build the Docker image: Open a terminal or command prompt, navigate to the directory containing the Dockerfile, and run the following command to build the Docker image:

   ```shell
   docker build -t your_image_name .
   ```

   The `-t` flag is used to tag the image with a name of your choice. The `.` at the end specifies the build context, which is the current directory.

32 Run the Docker container: Once the image is built, you can run a container based on that image using the following command:

   ```shell
   docker run -p 8080:8080 your_image_name
   ```

   The `-p` flag is used to map the host machine's port 8080 to the container's port 8080, allowing you to access the application running inside the container at `localhost:8080`.

   You can add any additional flags or options as per your requirements. For example, if you want to run the container in the background, you can add the `-d` flag:

   ```shell
   docker run -d -p 8080:8080 your_image_name
   ```

   That's it! The container should now be running, and you should be able to access your application at `localhost:8080`.

Remember to replace `your_image_name` with the desired name for your Docker image. Additionally, make sure you have Docker installed and running on your machine before executing these commands.


---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------

Docker File


1. **docker run**: This command creates and starts a new container based on a specified image.
   ```
   docker run [OPTIONS] IMAGE [COMMAND] [ARG...]
   ```

2. **docker ps**: Lists all running containers.
   ```
   docker ps [OPTIONS]
   ```

3. **docker images**: Lists all available local images on your system.
   ```
   docker images [OPTIONS]
   ```

4. **docker pull**: Downloads an image from a container registry.
   ```
   docker pull [OPTIONS] NAME[:TAG|@DIGEST]
   ```

5. **docker build**: Builds a Docker image from a Dockerfile.
   ```
   docker build [OPTIONS] PATH | URL | -
   ```

6. **docker stop**: Stops one or more running containers.
   ```
   docker stop [OPTIONS] CONTAINER [CONTAINER...]
   ```

7. **docker start**: Starts one or more stopped containers.
   ```
   docker start [OPTIONS] CONTAINER [CONTAINER...]
   ```

8. **docker restart**: Stops and starts one or more containers.
   ```
   docker restart [OPTIONS] CONTAINER [CONTAINER...]
   ```

9. **docker rm**: Removes one or more containers.
   ```
   docker rm [OPTIONS] CONTAINER [CONTAINER...]
   ```

10. **docker rmi**: Removes one or more images.
    ```
    docker rmi [OPTIONS] IMAGE [IMAGE...]
    ```

11. **docker exec**: Runs a command in a running container.
    ```
    docker exec [OPTIONS] CONTAINER COMMAND [ARG...]
    ```

12. **docker logs**: Fetches the logs of a container.
    ```
    docker logs [OPTIONS] CONTAINER
    ```

13. **docker inspect**: Displays detailed information about a container or image.
    ```
    docker inspect [OPTIONS] NAME|ID [NAME|ID...]
    ```

14. **docker network**: Manages Docker networks.
    ```
    docker network [OPTIONS] COMMAND
    ```
