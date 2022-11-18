# kendra-search

This is a easy file search app where you can pass keywords and it'll pass through the contents of the files. 
The relevant files are returned and if one finds it useful, it can be downloaded.
Built using aws s3 bucket, dynamoDB and Kendra service and Nodejs as the backend language.
Kendra is connected to s3 bucket where all the files are added. ETag and size of the file in s3 bucket is stored in DynamoDB and if the same file is uploaded again
plagirism is checked and response is returned. DynamoDB is used for user authentication as well.
Kendra is a crawling and hashing service which runs once every hour in this project.
