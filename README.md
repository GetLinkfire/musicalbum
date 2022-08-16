# Music Albums Library - Task Description
## Development: 
Develop a microservice to manage music albums library. The service should support the following functionalities:
* Create albums library

  It’s expected that one user can have only one library
  Aside music libraries users have only name
  No authentication is required (but it would be nice to have)

* Search Album by name and artist name
    * Use either Spotify or Deezer API to find albums
    * Found results should include
          * Artist name
          * Album name
          * Album cover (if available)
          * Album URL
* Save one or more found Albums into my library
* Remove Albums from library
* Implement the required unit testing.

Create a Readme file with proper instruction to run the microservice


## Testing 
    Write an API test automation to test one of the end points.Use any of the automation test frameworks that you are familiar with.
    Create a Readme file with proper instruction to set up and run the API test project so that the examiner will be able to set up the project properly.

## Deployment: 

Use one of the following approaches which you familiar most:
    * Publish the microservice into the local folder. Prepare all instructions how to run the application and required infrastructure
    * Deploy the  microservice with Docker and docker-compose to deploy required infrastructure services
    * Deploy the microservice and infrastructure  in a kubernetes cluster
        * You can use available local kubernetes clusters like Microk8s or Minikube.
        * Share the yaml files and a Readme file with proper instruction to deploy the application.
      
      
## Prerequisites:
  .NET + IDE of your choice. You can use VS 2022, VS for Mac, or VS Code
  If you a go with deployment into container then you need to have one of the following:
      Docker
      Kubernetes
      Local or cloud kubernetes cluster
      
## Requirements:

  * Use .NET 6
  * You are allowed to use any technology/third party you would like to use.
  * Solution should be testable, we are not looking for 100% code coverage but show examples of how you make parts unit-testable.
  
We want to get a better understanding of:

* The code you produce
* How do you go about architecting a scalable solution. Let’s imagine that you support not one but both integrations and planning to add more in future.

## Notes:
We would like to see a piece of code as you would do on your normal working day.
You can use any technology for API Testing.
Please send us whatever you have done before the deadline even if it is an uncompleted task.

Don't hesitate to contact us for questions and support while working on the task.

## Reference:
  * [Spotify Web API](https://myoctocat.com/assets/images/base-octocat.svg](https://developer.spotify.com/documentation/web-api/reference/#/)
  * Deezer Web API
  * Visual Studio 2022
  * Visual Studio for Mac
  * Visual Studio Code
  * Microk8s
  * Minikube





