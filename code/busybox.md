
# Use the BusyBox image
FROM busybox

# Set the command to print "Hello, World!"
CMD echo "Hello, World!"
```

To build and run this Dockerfile, follow these steps:

1. **Save the Dockerfile**: Create a file named `Dockerfile` and copy the above content into it.

2. **Build the Docker image**:

    ```bash
    docker build -t helloworld-busybox .
    docker build -t my-docker-image -f busybox.dockerfile .
    ```

3. **Run the Docker container**:

    ```bash
    docker run helloworld-busybox
    ```

You should see the output:

```
Hello, World!
```
