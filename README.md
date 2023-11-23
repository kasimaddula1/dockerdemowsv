# dockerdemowsv

## Description
This repo demonstrates how we can leverage the docker to run tests instead of running them on the local machine. It will create a docker image by copying all the necessary files onto image and also downloading Chrome browser to run the tests on

## Getting Started

## Dependencies
* Download the docker desktop from here https://www.docker.com/products/docker-desktop/ and make sure its up and running before running below docker commands
* Also make sure you have node.js installed on your machine

## To run tests on Docker
### To build a docker image
* docker build -t sampledockertest .

### To run the docker and tests
* docker run sampledockertest

Note: **sampledockertest** is the image name and it can be customised to your needs

## To run tests on local
Run below cmds

* npm install
* npm run test
