# serverless-localstack-lambda
Serverless LocalStack Lambda

# More Details Visit

https://onexlab-io.medium.com/serverless-localstack-lambda-53fd8d46983

docker and aws commands:
    command to setup docker once you make docker-compose file:
    docker-compose up

    command to setup aws:
    aws --endpoint-url=http://localhost:4566 s3 mb s3://localstacktest

    command to look at bucket:
    aws --endpoint-url=http://localhost:4566 s3 ls <your-bucket-name>

    example: aws --endpoint-url=http://localhost:4566 s3 ls localstacktest
    
serverless commands:
    Get serverless up and running
        -serverless deploy --stage local 

    Test hello lambda function
        -serverless invoke local -f hello