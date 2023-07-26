## ECS CLI V2 Sample App

The ECS CLI is a tool for developers to create, release and manage production ready containerized applications on ECS. From getting started, pushing to staging and releasing to production, the ECS CLI can help manage the entire lifecycle of your application development.

This is a small sample app that can be used to demonstrate the ECS CLI V2. It creates a static website using nginx as the frontend.

## How to section

### How to run Dockerfile locally

- To build image
  `docker build -t aws-ecs-cli-sample-app:v1.0 -f Dockerfile .`
- To run image in the detach mode
  `docker run --name aws-ecs-cli-sample-app -p 3010:80 -d aws-ecs-cli-sample-app:v1.0`
- To list all Dockerfile containers
  `docker ps`
- To stop/start/restart a Dockerfile container
  `docker stop aws-ecs-cli-sample-app`
  `docker start aws-ecs-cli-sample-app`
  `docker restart aws-ecs-cli-sample-app`
- To remove/delete a Dockerfile container (not image)
  `docker docker rm aws-ecs-cli-sample-app`
  `docker rm [OPTIONS] CONTAINER_ID_OR_NAME`
  To stop and remove
  `docker stop aws-ecs-cli-sample-app && docker rm aws-ecs-cli-sample-app`

## License

This library is licensed under the MIT-0 License. See the LICENSE file.
