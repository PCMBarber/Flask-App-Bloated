# Flask-App-Bloated

This is a basic Flask application that serves a simple static website that returns the machine's hostname.

It is directly accessible on port `80` by running the commands:

```bash
docker build -t flask-app-bloated .
docker run -d -p 80:5500 --name f-app-bloated flask-app-bloated
```

This is an example of a container built with files not needed for the app to function.

Add new entries to the .dockerignore file to bring this image to the same size as flask-app-alpine, without deleting any files from the repository.