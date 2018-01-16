Simple docker image for Drupal

base on the blog post from https://circleci.com/blog/continuous-drupal-p1-maintaining-with-docker-git-composer/

Step to use
* Create folder app inside it. App folder will contain all drupal code base.
* Change ports mapping as per your requiremnet in Docker
* Build container  "docker-compose up -d --build"

Run following command to get the ip of Mariab db container 
docker inspect -f '{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' container_id
