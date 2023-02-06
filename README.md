# KANBANBOARD
Having a good productivity system is not only important at work, but also in life in general, as it helps us achieve much more in less time. This will be a visual tool that will allow you to manage activities and tasks.

**KANBANBOARD** is a platform that works under the Kanban board paradigm for the creation, organization and management of activities and tasks and thus improve productivity in any type of project.

![](https://github.com/Nor01/KanbanBoard/blob/main/kanban2_cover.gif)

## Environment Variables
To run this project, you will need to add the following environment variables to your `.env` file:
#### Backend
`JWT_SECRET`
`POSTGRES_USERNAME`
`POSTGRES_DBNAME`
`POSTGRES_DBPASSWORD`
`POSTGRES_DBPORT`
#### Frontend
`API_PROXY`

## Tech
**KANBANBOARD** uses a number of open source projects to work properly:

<div align="center">
  <img src="https://github.com/devicons/devicon/blob/master/icons/fastapi/fastapi-original.svg" title="FastAPI" alt="FastAPI " width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/python/python-original.svg" title="Python" alt="Python" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/bulma/bulma-plain.svg" title="Bulma" alt="Bulma" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/react/react-original.svg" title="React" alt="React" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/postgresql/postgresql-original.svg" title="Postgresql"  alt="Postgresql" width="40" height="40"/>&nbsp;
  <img src="https://github.com/devicons/devicon/blob/master/icons/docker/docker-original.svg" title="Docker"  alt="Docker" width="40" height="40"/>&nbsp;
</div>

- [REACTJS](https://github.com/facebook/react/) - React is a free and open-source front-end JavaScript library for building user interfaces based on UI components.
- [PYTHON 3](https://www.python.org/doc/) - Python is developed under an OSI-approved open source license, making it freely usable and distributable, even for commercial use. Python's license is administered by the Python Software Foundation.
- [FASTAPI](https://fastapi.tiangolo.com/) - FastAPI is a Web framework for developing RESTful APIs in Python. FastAPI is based on Pydantic and type hints to validate, serialize, and deserialize data, and automatically auto-generate OpenAPI documents.
- [BULMA](https://bulma.io/documentation/) - Bulma is a free, open source framework that provides ready-to-use frontend components that you can easily combine to build responsive web interfaces.
- [DOCKER](https://docs.docker.com/) - Docker is a set of platform as a service products that use OS-level virtualization to deliver software in packages called containers.
- [POSTGRESQL](https://www.postgresql.org/docs/) - PostgreSQL, also known as Postgres, is a free and open-source relational database management system emphasizing extensibility and SQL compliance.

## Docker
KABANBOARD is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 8080, so change this within the Dockerfile if necessary. When ready, simply use the Dockerfile to
build the image.

```sh
cd kb_backend
docker build -t <youruser>/kb_backend:${package.json.version}
```

This will create the `kb_backend` image and pull in the necessary dependencies.
Be sure to swap out `${package.json.version}` with the actual version of `kb_backend`.

Once done, run the Docker image and map the port to whatever you wish on your host. In this example, we simply map port 8000 of the host to port 8080 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart=always --name=kb_backend <youruser>/kb_backend:${package.json.version}
```

> Note: you can, *for testing **ONLY*** copy/paste the uploaded file and execute `docker-compose up`

Verify the deployment by navigating to your server address in your preferred browser.

```sh
127.0.0.1:8000
```

## Deployment
#### Backend
To deploy FastAPI

```bash
  pip install -r requirements.txt
  uvicorn main:app --reload
```
#### Frontend
To deploy ReactJS
```bash
  npm install
  npm start
```

## Features
- ...
