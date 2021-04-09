# Guides

1. Import project to Intelij/IDE.

2. Run the application.

3. Use below link to install MySQL DB configured in application.properties file:

    https://dev.mysql.com/doc/mysql-installation-excerpt/5.7/en/
    
    use below query to create data base:
    
    creat database shortenedURLs;
    
    name can be changed under application.properties file -  spring.datasource.url
    
 # APIs invocation using postman
 
 1. For Shortening API use below curl:
 
 curl --location --request PUT 'http://localhost:8080/shortenUrl' \
 --header 'Content-Type: application/json' \
 --data-raw '{
    "originalLongURL": "https://www.tremorvideo.com/"
 }'
 
 originalLongURL value provided as reference.
 
 2. For redirect API use below curl:
 
 curl --location --request GET 'http://localhost:8080/redirectUrl/U'
 
 path variable provided as reference.
 
 3. For Analytics API use below curl:
 
 curl --location --request GET 'http://localhost:8080/shortenedUrlStatistics/U' 
 
 path variable provided as reference.
 
 
