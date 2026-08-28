# On developers machine

docker --version

  docker build -t my-submission .

  docker run my-submission:latest

  docker images

  docker save -o my-submission.tar my-submission:latest



# On executor machine

  docker load -i my-submission.tar

  docker run my-submission:latest



# tagging versions

docker tag <existing-image-id> my-submission:1.0.0

or 

docker build -t my-submission:1.0.0 .