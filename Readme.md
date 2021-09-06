docker-machine start
docker-machine ls

Get Container image                                              docker pull <HUB_IMAGE_NAME>
New container add                                                docker build .
New container add with image name                                docker build -t <REPOSITORY>:<TAGNAME> .
Show images list                                                 docker images (image ls)
Delete images                                                    docker rmi <CONTAINER_ID> <CONTAINER_ID> .....
Deleted images all list                                          docker image prune
Single run mode                                                  docker run <HUB_IMAGE_NAME> or <IMAGE_ID>
Single run mode with in                                          docker run -it <HUB_IMAGE_NAME> or <IMAGE_ID>
Single run bash with in                                          docker run -it <HUB_IMAGE_NAME> or <IMAGE_ID> bush
Show all container (user & unused)                               docker ps -a
Deleted container list                                           docker rm <CONTAINER_ID> <CONTAINER_ID> .....
Deleted container all list                                       docker container prune
Start running container                                          docker start <CONTAINER_ID> or <IMAGE_ID>
Stop running container                                           docker stop <CONTAINER_ID> or <IMAGE_ID>
Docker port configure                                            docker run -p <OUT>:<IN> <CONTAINER_ID> or <IMAGE_ID>
Docker run background                                            docker run -d -p <OUT>:<IN> <CONTAINER_ID> or <IMAGE_ID> or <NAME>
Docker attach                                                    docker attach <CONTAINER_ID> or <IMAGE_ID> or <NAME>
Docker logs                                                      docker logs <CONTAINER_ID> or <IMAGE_ID> or <NAME>
Add same name container                                          docker run -d -p <OUT>:<IN> --name <REPOSITORY>:<TAGNAME> <CONTAINER_ID> or <IMAGE_ID> or <NAME>
Container stop auto deleted                                      docker run -d -p <OUT>:<IN> --rm  --name <REPOSITORY>:<TAGNAME><CONTAINER_ID>
Container+Volume stop auto deleted                               docker run -d -p <OUT>:<IN> -v <VOLUME_NAME>:<PATH_IN_DOCKER> --rm  --name <REPOSITORY>:<TAGNAME><CONTAINER_ID>
Add env list in docker running                                   docker run -d {-e <ENV_NAME>=<ENV_TYPE> ...} -p <OUT>:<IN> --name <REPOSITORY>:<TAGNAME> --rm <CONTAINER_ID> or <IMAGE_ID> or <NAME>
Add env file in docker running                                   docker run -d --nev-file <PATH> -p <OUT>:<IN> --name <REPOSITORY>:<TAGNAME> --rm <CONTAINER_ID> or <IMAGE_ID> or <NAME>
Login Docker server                                              docker login
Tag add in image                                                 docker tag <REPOSITORY> <DOCKER_USERNAME>/<REPOSITORY>
Push Docker server                                               docker push <DOCKER_USERNAME>/<REPOSITORY>:<VERSION>
Show Docker Image information                                    docker image inspect <DOCKER_USERNAME>/<REPOSITORY>
Create Volume directory                                          docker volume create
inspect Volume directory                                         docker volume inspect
Listed Volume directory                                          docker volume ls
Delete Volume directory                                          docker volume rm
Delete all Volume directory                                      docker volume prune