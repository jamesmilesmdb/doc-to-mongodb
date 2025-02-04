# Doc To Mongo Service

This is a Spring Boot java application which does the following:
a) Handles the upload of files
b) Extracts the text content from a file
c) Uploads this information to a MongoDB instance

## How to run
You will need to edit the `application.yaml` file to point to your instance of Atlas. You can also tweak other parameters here such as the server port.
By default the application runs on port 9090

## Uploading files
The skeleton of this project - and all code to handle the uploads - comes from the Spring Boot guide for creating a file upload microservice.
The [Spring Guide](https://spring.io/guides/gs/uploading-files/) is amazing, and can is super easy to understand.

## Extracting data
This project uses the Apache Tika library to extract text from documents.

NB: this has only been tested on a subset of documents, it is not a production grade system.
