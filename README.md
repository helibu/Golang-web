# Golang-based-web

This project is the Golang based backend for media sharing web project. [Media sharing web application](https://github.com/helibu/Media-Sharing-web)

<br> Deployed on http://34.73.107.83/api/v1
## Technology Used
### GCE
GCE to host ElasticSearch, which is served as a NoSQL database and geo location based search engine for my project.
### ElasticSearch
ElasticSearch as a NoSQL database to store data posted by users, and to search by Geo-index.
### GCS
GCS as Object Storage to store all media files posted by users.

### Google ML Engine

### BigTable 
BigTable to store user post as backup and to pass data to BigQuery.
### DataFlow 
Use Google DataFlow to extract data from BigTable and Transform to BigQuery.
### BigQuery
Offline analysis
### GKE
Build Go service to docker image and run the image on virual machines managed by GKE cluster.

## Supported Endpoints

### "/signup"
For sign up to the web. 

### "/login"
For log in to the web

### "/post"

Make a image/video post to the server. ElasticSearch will store the post info. If the post is a '.jpeg' image post, the ML model on Google ML Engine will predict whether the image is a human face or not.

### "/search"
To search post with a lat, lon and range.


