# DevOps Deployment Repo

## Prerequisites

- Docker

## Configure environment

### Clone the app

```sh
$ git clone --recurse-submodules -b demo https://github.com/ensynAI/devops.git
```

### Environment variables

Create a `.env` file containing your OpenAI API Key in the root directory (devops).

`.env` file structure:

```
OPENAI_API_KEY="your-api-key"
```

## Running the app

To launch the app run the following command. The command builds the docker images and launches the app (this may take some time).

```sh
$ docker-compose up
```

To rebuild everything from scratch use:

```sh
$ docker-compose up --build --force-recreate --no-deps
```

## Using the app

To use the app go to [localhost:3000](http://localhost:3000/)

- Fronend app: [localhost:3000](http://localhost:3000/)

- Backend server: [localhost:8000](http://localhost:8000/)
