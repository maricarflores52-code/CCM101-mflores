# Reflection

During this checkpoint, I learned how Docker containers make software setup and deployment easier and faster. A Docker container can start in seconds because it uses the host operating system’s kernel, while installing an operating system requires more time, storage, and configuration. This showed me that containers are useful when we need to quickly run applications in a consistent environment.

Port mapping, such as -p 8080:80, is necessary because the web server inside the container uses port 80, but we need a way to access it from the host computer. Port 8080 on the host is connected to port 80 inside the container, allowing me to open the web server through the browser. I also learned that when I use the docker rm command, the container is permanently removed, including the data stored inside its writable container layer. This is why important data should be stored using volumes or other persistent storage.

When a Docker container is removed using the docker rm command, the container itself is deleted. This means the container's writable layer and its configuration are removed. However, Docker images are separate from containers, so removing a container does not automatically remove the image used to create it.

Containerization also changes how software developers and IT operations teams work together. Developers can create applications in the same environment that can be used by the operations team, reducing problems caused by differences in computer setups. This supports DevOps because development, testing, and deployment can become more consistent and efficient.

My GitHub portfolio is also evolving as I complete more cloud computing activities. It now contains documentation, commands, screenshots, and reflections from my laboratory exercises. This activity added practical experience with Docker and helped me understand how cloud-native applications can be deployed and managed.
