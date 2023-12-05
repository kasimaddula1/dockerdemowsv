# dockerdemowsv

## Description
This repo demonstrates how we can leverage the docker to run tests instead of running them on the local machine. It will create a docker image by copying all the necessary files onto image and also downloading Chrome browser to run the tests on

## Getting Started

## Dependencies
* Download the docker desktop from here https://www.docker.com/products/docker-desktop/ and make sure its up and running before running below docker commands
* Also make sure you have node.js and JRE installed on your machine for running it locally

## To run tests on Docker
### To build a docker image
* docker build -t sampledockertest .

### To run the docker and tests
* docker run -t sampledockertest test -- --mochaOpts.grep "@Test1"

Note: 
1. **sampledockertest** is the image name and it can be customised to your needs at the time of docker build
2. Also, make sure you have a script defined in packaje.json like **test** in above example. this docker image can be run with any script that
you ahve define in the package.json by replacing in the place of **test** on top of it you can pick and choose the tests that you wanted to run 
by using the **tags** like **@Test1** in above example

## To run tests on local
Run below cmds

* npm install
* npm run test -- --mochaOpts.grep "@Test1"
