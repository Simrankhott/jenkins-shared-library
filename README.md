﻿# jenkins-shared-library
 
﻿# dockerBuild.groovy:
This code defines a function that takes two parameters, project and hubUser. Inside the function, it executes a series of shell commands using the Jenkins sh step to build a Docker image, tag it with the provided parameters, login to a Docker registry using credentials stored in Jenkins, and push the image to the registry.

﻿# dockerCleanup.groovy:
This code defines a function that takes two parameters, project and hubUser. It uses the docker rmi command to remove the specified Docker images from the local Docker engine. This step is typically used to clean up unused or old Docker images after a build or deployment.

﻿# gitCheckout.groovy:
This code defines a function that takes a parameter called stageParams (assumed to be a Map). It uses the Jenkins checkout step to clone or checkout a Git repository specified by the stageParams.url and stageParams.branch parameters. This step is used to fetch the source code from a Git repository for building or deploying an application.
